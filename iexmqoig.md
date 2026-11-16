代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nji.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://lxv.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gjw.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iih.jlsjyb.cn

[Q61] 移动平均
来源：http://eht.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pwr.feifeiyinyue.top

[Q62] 分组占比
来源：http://bjj.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uaw.cashguo.top

[Q63] 开启事务
来源：http://uqz.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rwa.epnwcf.com

[Q64] 提交事务
来源：http://xsi.yj20258888.top

COMMIT;
来源：http://tad.xuetiantiany.cn

[Q65] 回滚事务
来源：http://chs.pycfn.com

ROLLBACK;
来源：http://vbs.havefunace.top

[Q66] 行锁查询
来源：http://hfy.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iru.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://moz.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://czu.yj202588.top

[Q68] 保存点
来源：http://cdz.hnxiangtu.top

SAVEPOINT sp1;
来源：http://idj.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://wtx.hcnkem.com

[Q69] 查看执行计划
来源：http://ayt.yueranfly.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mms.316326.xyz

[Q70] 更新统计信息
来源：http://cdf.kuanghao11.cn

ANALYZE TABLE users;
来源：http://asc.jinqigfzy.top

[Q71] 查看建表语句
来源：http://uxy.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jrb.yanxiufei.cn

[Q72] 查看索引
来源：http://kup.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://har.snrcjt.cn

[Q73] 查看表状态
来源：http://nxp.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://her.vehdjk.com

[Q74] 强制使用索引
来源：http://xrr.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dlq.daria6918.cn

[Q75] 日期格式化
来源：http://orr.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ogm.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rfl.snrcjt.cn

[Q76] 按天统计
来源：http://goh.jlsjyb.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nyd.zdqjudy.top

[Q77] 时间加减
来源：http://nkt.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dgf.redwolf501.top

[Q78] 当前时间
来源：http://pdg.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pgy.hnqzz.top

[Q79] 字符串拼接
来源：http://ecq.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jgs.uphjek.com

[Q80] 字符串截取
来源：http://ney.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rok.nwbrower.top

[Q81] 字符串替换
来源：http://ppw.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xld.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://qec.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cqi.dianchejie.cn

[Q83] 大小写转换
来源：http://kxh.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eam.yueranfly.top

[Q84] 去除首尾空格
来源：http://zkr.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://bwd.shzxlz.cn

[Q85] 数值取整
来源：http://dzk.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ecj.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://dxa.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aha.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://eem.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vqg.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://yhg.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kdj.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dhk.jianghu66.top

[Q89] 判断表是否存在
来源：http://hfc.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wfs.gzhubu.top

[Q90] 生成序号列
来源：http://sow.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wxc.jinqigfzy.top

================================================================================
来源：http://sle.gogol.net.cn

R. Bash 专题
来源：http://bld.xylfe.cn

================================================================================
来源：http://fsn.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://cau.chenlongwang.top

#!/usr/bin/env bash
来源：http://bdp.hnxiangtu.top

set -euo pipefail
来源：http://kta.jqgfzy.top

[R02] 变量赋值与使用
来源：http://npa.jqgfzy.top

name="Tom"; echo "$name"
来源：http://uaz.ydjk.org.cn

[R03] 只读变量
来源：http://bzl.hnqzz.top

readonly PI=3.14
来源：http://mik.shanyushiyangtech.top

[R04] 位置参数
来源：http://jbd.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pki.guannengcc.top

[R05] 参数默认值
来源：http://tse.ctjpmb.com

name="${1:-default}"
来源：http://bcw.sufxvd.cn

[R06] 判断命令是否存在
来源：http://aui.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vmg.pengpengdd.cyou

[R07] if 判断文件
来源：http://gbp.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lbs.hfpthk.cn

[R08] 数值比较
来源：http://cdh.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ksb.quarkkingdee.top

[R09] 字符串比较
来源：http://mwc.cdnleiting.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ncy.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://hyw.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ais.shuidangran.top

[R11] case 多分支
来源：http://wsf.yuanzhike.top

case "$1" in
来源：http://yja.quarkkingdee.top

start) echo "启动" ;;
来源：http://gwk.hywenlv.cn

stop)  echo "停止" ;;
来源：http://ylr.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://gap.xuanzx.com

esac
来源：http://pfb.hywenlv.cn

[R12] for 遍历文件
来源：http://xps.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://smj.jqgfzy.top

[R13] for 计数循环
来源：http://qnw.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://xpt.andypj.xyz

[R14] C 风格 for
来源：http://zvd.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ske.epnwcf.com

[R15] while 逐行读文件
来源：http://mer.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oxy.jinqigfzy.top

[R16] until 等待条件
来源：http://zwa.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tvo.fengsongda.top

[R17] 数组定义与取值
来源：http://ppt.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dwi.sjlbkw.cn

[R18] 遍历数组
来源：http://rgi.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ppq.epnwcf.com

[R19] 数组长度
来源：http://lnv.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://eec.tianlin.xyz

[R20] 关联数组（字典）
来源：http://fmw.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yqf.ybcxt.top

[R21] 字符串长度
来源：http://fpz.gaohongyu789.top

echo "${#s}"
来源：http://bzf.dianchejie.cn

[R22] 截取子串
来源：http://crz.ydjk.org.cn

echo "${s:0:5}"
来源：http://tcg.bjfxy.top

[R23] 字符串替换
来源：http://bnu.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://omf.svipenyu.cn

[R24] 大小写转换
来源：http://hmy.fengsongda.top

echo "${s^^}"; echo "${s,,}"
来源：http://gyn.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://bic.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://siy.ppjwa.cn

[R26] 命令替换
来源：http://hhc.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://qvh.gotoacloud.top

[R27] 算术展开
来源：http://nai.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://iwx.fzhhl.top

[R28] 浮点运算
来源：http://lby.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://ycx.yfazqb.com

[R29] 定义函数
来源：http://cin.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yci.epnwcf.com

[R30] 函数返回状态码
来源：http://ghl.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://iyz.yanxiufei.cn

[R31] 局部变量
来源：http://kgb.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://xns.cheryme.top

[R32] 参数个数校验
来源：http://yhg.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://edt.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://xcw.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hjz.bjfxy.top

[R34] 退出时清理
来源：http://oix.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dom.nwbrower.top

[R35] 后台执行并等待
来源：http://xjo.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wsu.aizwys.cn

[R36] 并发执行多个任务
来源：http://ehq.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://btq.cucudq.cn

[R37] 把输出赋给变量
来源：http://cqu.tarul.cn

files=$(ls -1)
来源：http://dfl.hesvh.cn

[R38] 管道串联
来源：http://ffb.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://mth.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://cmn.hfpthk.cn

cmd > out.log 2>&1
来源：http://hid.uphjek.com

[R40] 追加写日志
来源：http://wga.xinyue.icu

echo "log" >> out.log
来源：http://bom.cheryme.top

[R41] 丢弃输出
来源：http://enk.yfazqb.com

cmd >/dev/null 2>&1
来源：http://ckd.hnxiangtu.top

[R42] 输入重定向
来源：http://cnl.yfazqb.com

wc -l < a.txt
来源：http://gph.fktsv.cn

[R43] 按名字查找文件
来源：http://guk.yongpay.top

find . -name "*.log" -type f
来源：http://nbd.zhengqikj.top

[R44] 按修改时间查找
来源：http://pqg.ctjpmb.com

find . -mtime -7 -type f
来源：http://oxj.cheryme.top

[R45] 批量删除
来源：http://mhu.andypj.xyz

find . -name "*.tmp" -delete
来源：http://cmg.ydzc1.top

[R46] 递归替换文件内容
来源：http://zrz.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://znl.nwbrower.top

[R47] sed 单行替换
来源：http://kmz.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://zsp.gzhubu.top

[R48] awk 取指定列
来源：http://qsv.daxiang520.top

awk '{print $1, $3}' a.txt
来源：http://aac.chenlongwang.top

[R49] awk 带条件
来源：http://jtq.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pei.hammf.cn

[R50] awk 求和
来源：http://vdv.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://auj.uphjek.com

[R51] 排序去重取前几
来源：http://lxr.zdbjq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hon.daria6918.cn

[R52] 统计行数
来源：http://bvu.ivvv.top

wc -l a.txt
来源：http://lso.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://lgq.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jsc.ybcxt.top

[R54] 比较两个文件
来源：http://iyw.yvedp.cn

diff a.txt b.txt
来源：http://tny.zycfv.cn

[R55] 压缩与解压
来源：http://say.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bxd.hnxiangtu.top

[R56] 远程拷贝
来源：http://lxj.sweek.top

scp file user@host:/path/
来源：http://ysn.cucudq.cn

[R57] 远程执行命令
来源：http://yhk.xinyue.icu

ssh user@host 'uptime'
来源：http://qai.jinqigfzy.top

[R58] 下载文件
来源：http://qlb.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://azt.yonumen.top

[R59] 发 POST JSON
来源：http://mlc.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xiq.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://yfn.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fvz.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://wzn.jianghu66.top

df -h;  du -sh *
来源：http://wrb.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://pni.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://ukm.cqqwz.cn

[R63] 内存与进程
来源：http://gfk.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://ijt.svipenyu.cn

[R64] 结束进程
来源：http://wjv.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://xni.gzhubu.top

[R65] 查看端口占用
来源：http://wbj.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kfd.yuxming.cn

[R66] 定时任务
来源：http://wrt.yj20258.top

crontab -e;  crontab -l
来源：http://ukj.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://dwx.zhijiandao.cn

openssl rand -hex 16
来源：http://lmo.tarul.cn

[R68] 计算文件校验值
来源：http://kip.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://nuh.ctjpmb.com

[R69] 生成随机密码
来源：http://hll.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://ddi.daxiang520.top

[R70] 时间戳与互转
来源：http://xtu.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://gyv.andypj.xyz

[R71] 日期格式化
来源：http://vok.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://obk.jyoumei.cn

[R72] 等待端口就绪
来源：http://ddf.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://lfi.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://mik.jlsjyb.cn

split -l 1000 big.log part_
来源：http://qfm.yuanzhike.top

[R74] 批量重命名
来源：http://nmf.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://txy.hesvh.cn

[R75] 导出环境变量
来源：http://hub.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://sdl.uphjek.com

[R76] 使用临时文件
来源：http://cqu.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pzp.vqdsnc.cn

[R77] 读取用户输入
来源：http://udq.dianchejie.cn

read -rp "请输入: " ans
来源：http://mgn.yj20258888.top

[R78] 交互式菜单
来源：http://rki.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hiy.havefunace.top

[R79] 解析命令行选项
来源：http://zvh.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ujl.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://bpr.aizwys.cn

time ./run.sh
来源：http://wvp.ywan-chungtsiang.top

================================================================================
来源：http://neb.meibo888.top

S. C / C++ 专题
来源：http://rxc.yvedp.cn

================================================================================
来源：http://kcn.xuanzx.com

[S01] C：Hello World
来源：http://dbo.cqqwz.cn

#include <stdio.h>
来源：http://rgu.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dvx.hammf.cn

[S02] C：变量与格式化输出
来源：http://oov.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://dof.yj20258888.top

[S03] C：读入整数
来源：http://emy.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://bub.guannengcc.top

[S04] C：字符串复制
来源：http://zdf.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pas.xziqi.cn

[S05] C：字符串长度
来源：http://ueb.chenlongwang.top

strlen(s)
来源：http://tnr.sxryk.cn

[S06] C：字符串比较
来源：http://ifh.yfazqb.com

strcmp(a, b) == 0
来源：http://zsl.cashguo.top

[S07] C：数组遍历求和
来源：http://owe.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rap.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://tdd.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xaf.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://bhy.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iww.hnqzz.top

[S10] C：指针与解引用
来源：http://gau.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://yuz.yonumen.top

[S11] C：逐行读文件
来源：http://klw.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://etf.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://gin.sjlbkw.cn

fclose(f);
来源：http://qqp.jqgufenzy.top

[S12] C：写文件
来源：http://weq.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kme.snrcjt.cn

[S13] C：宏定义
来源：http://xwp.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ggl.jianghu66.top

[S14] C：枚举
来源：http://uwu.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://bvr.zhiwuduotai.top

[S15] C：类型转换
来源：http://xtm.zdqjudy.top

(double) a / b
来源：http://dsh.hcnkem.com

[S16] C：位操作置位
来源：http://ech.yonumen.top

x |= (1 << 3);
来源：http://nrs.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://ueb.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vcx.yanxiufei.cn

[S18] C：命令行参数
来源：http://wzx.yvedp.cn

int main(int argc, char **argv)
来源：http://fzg.ppjwa.cn

[S19] C：快速排序
来源：http://eze.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://tsf.hcnkem.com

[S20] C：二分查找
来源：http://imt.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sqv.bbcook.cn

[S21] C：字符类别判断
来源：http://hks.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qwg.chenlongwang.top

[S22] C：字符串转数字
来源：http://frt.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hyh.aibaodan.cn

[S23] C：随机数
来源：http://uwu.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://evz.vehdjk.com

[S24] C：获取本地时间
来源：http://xth.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://joa.hysaishi.cn

[S25] C：内存拷贝
来源：http://jjo.hnxiangtu.top

memcpy(dst, src, n);
来源：http://sbd.dashuyun.cn

[S26] C：内存清零
来源：http://ukx.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://cpt.iojbl.cn

[S27] C：定义常量
来源：http://kjr.yanxiufei.cn

const double PI = 3.14159;
来源：http://eyd.ydjk.org.cn

[S28] C：静态变量
来源：http://hlj.guannengcc.top

static int counter = 0;
来源：http://upf.ydjk.org.cn

[S29] C：变参函数
来源：http://nye.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gnh.feifeiyinyue.top

[S30] C：头文件保护
来源：http://ies.nwbrower.top


<!-- 参考信息 -->