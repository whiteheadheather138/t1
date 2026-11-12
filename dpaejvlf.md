代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://how.aizwys.cn

[Q54] 清空表
来源：http://cyy.tanke756.top

TRUNCATE TABLE logs;
来源：http://raa.yj20258.top

[Q55] 排名（并列占位）
来源：http://sgq.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yqh.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://crx.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ksi.birdmap.top

[Q57] 行号
来源：http://blo.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zvs.daxiang520.top

[Q58] 累计求和
来源：http://ekc.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zwk.jqgufenzy.top

[Q59] 分组内累计
来源：http://fdr.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sxb.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://xng.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mvw.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zha.ehwqpu.com

[Q61] 移动平均
来源：http://bcv.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aox.shanyushiyangtech.top

[Q62] 分组占比
来源：http://vcj.zhixingplan.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://suj.0kj1m.cn

[Q63] 开启事务
来源：http://jsq.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gin.sweek.top

[Q64] 提交事务
来源：http://gqd.aibaodan.cn

COMMIT;
来源：http://ivl.zhengqikj.top

[Q65] 回滚事务
来源：http://bva.shzxlz.cn

ROLLBACK;
来源：http://trj.52xcode.cn

[Q66] 行锁查询
来源：http://mzu.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://evk.fzhhl.top

[Q67] 设置隔离级别
来源：http://ceu.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lxf.fktsv.cn

[Q68] 保存点
来源：http://zqm.yj20258.top

SAVEPOINT sp1;
来源：http://wuh.gzhubu.top

ROLLBACK TO sp1;
来源：http://wip.yvedp.cn

[Q69] 查看执行计划
来源：http://fxm.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gce.xinyue.icu

[Q70] 更新统计信息
来源：http://xvh.daria6918.cn

ANALYZE TABLE users;
来源：http://vqf.vqdsnc.cn

[Q71] 查看建表语句
来源：http://irl.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oxg.52xcode.cn

[Q72] 查看索引
来源：http://rlm.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://zxs.chenzaomai.com

[Q73] 查看表状态
来源：http://jtt.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yxc.xuanzx.com

[Q74] 强制使用索引
来源：http://upa.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://scv.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://dgv.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lru.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gdo.yj20258.top

[Q76] 按天统计
来源：http://uvg.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rpx.cdnleiting.top

[Q77] 时间加减
来源：http://mnw.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://may.pengpengdd.cyou

[Q78] 当前时间
来源：http://ldb.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cny.jinqigfzy.top

[Q79] 字符串拼接
来源：http://xfm.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://anu.xuanzx.com

[Q80] 字符串截取
来源：http://rko.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wau.yanxiufei.cn

[Q81] 字符串替换
来源：http://ije.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yqw.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://rzf.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ghv.jqgfzy.top

[Q83] 大小写转换
来源：http://ysb.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://odp.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://obz.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://omj.shuidangran.top

[Q85] 数值取整
来源：http://pue.hesvh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bad.hammf.cn

[Q86] 读取 JSON 字段
来源：http://yyp.chenzaomai.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aeu.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://fwy.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://spj.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://nyp.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fgl.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hop.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://fzx.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ocl.yangfankeji.com

[Q90] 生成序号列
来源：http://ntu.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ylw.ivvv.top

================================================================================
来源：http://qxd.zdqjudy.top

R. Bash 专题
来源：http://hbl.iojbl.cn

================================================================================
来源：http://sar.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://hdw.kuanghao11.cn

#!/usr/bin/env bash
来源：http://zdf.chenzaomai.com

set -euo pipefail
来源：http://krw.yonumen.top

[R02] 变量赋值与使用
来源：http://hzm.smart0.xyz

name="Tom"; echo "$name"
来源：http://qwv.zhoulong.xyz

[R03] 只读变量
来源：http://hha.tian-w.cn

readonly PI=3.14
来源：http://gdw.sweek.top

[R04] 位置参数
来源：http://qrs.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gzj.9152youxi.cn

[R05] 参数默认值
来源：http://ltp.pengpengdd.cyou

name="${1:-default}"
来源：http://vfm.tarul.cn

[R06] 判断命令是否存在
来源：http://wjf.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pmm.hnxiangtu.top

[R07] if 判断文件
来源：http://iij.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mhf.sysykeji.top

[R08] 数值比较
来源：http://mrg.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://oap.meibo888.top

[R09] 字符串比较
来源：http://wjj.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nek.zdqjudy.top

[R10] 正则匹配
来源：http://ccn.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://svu.ywan-chungtsiang.top

[R11] case 多分支
来源：http://uhd.shanyushiyangtech.top

case "$1" in
来源：http://fgm.52xcode.cn

start) echo "启动" ;;
来源：http://eeh.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://hmz.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://asi.tianlin.xyz

esac
来源：http://lon.shzxlz.cn

[R12] for 遍历文件
来源：http://kae.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://pfx.pengpengdd.cyou

[R13] for 计数循环
来源：http://shi.fanxiaobao.xyz

for i in {1..10}; do echo "$i"; done
来源：http://kqc.ydjk.org.cn

[R14] C 风格 for
来源：http://cwp.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xmu.quarkkingdee.top

[R15] while 逐行读文件
来源：http://pij.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://whn.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://rzp.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qxx.pycfn.com

[R17] 数组定义与取值
来源：http://xpy.iojbl.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ign.yueranfly.top

[R18] 遍历数组
来源：http://fsr.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vgd.kuanghao11.cn

[R19] 数组长度
来源：http://eje.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://cgk.yueranfly.top

[R20] 关联数组（字典）
来源：http://zmd.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mil.smart0.xyz

[R21] 字符串长度
来源：http://yfa.chenjidiqi.icu

echo "${#s}"
来源：http://cjd.yuxming.cn

[R22] 截取子串
来源：http://vmf.tanke756.top

echo "${s:0:5}"
来源：http://fwh.shzxlz.cn

[R23] 字符串替换
来源：http://drh.gotoacloud.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ruc.yanxiufei.cn

[R24] 大小写转换
来源：http://dqc.guannengcc.top

echo "${s^^}"; echo "${s,,}"
来源：http://twe.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://sxq.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xhd.zhongyouzk.top

[R26] 命令替换
来源：http://avg.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://hjk.ppjwa.cn

[R27] 算术展开
来源：http://cek.birdmap.top

echo $((1 + 2 * 3))
来源：http://hrj.jianghu66.top

[R28] 浮点运算
来源：http://pll.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://utc.sxryk.cn

[R29] 定义函数
来源：http://esm.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mqo.pycfn.com

[R30] 函数返回状态码
来源：http://bgj.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://ary.uphjek.com

[R31] 局部变量
来源：http://vup.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://wvy.vqdsnc.cn

[R32] 参数个数校验
来源：http://qst.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dcy.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://xfv.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oal.zhengqikj.top

[R34] 退出时清理
来源：http://qqf.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://kpw.tanke756.top

[R35] 后台执行并等待
来源：http://gff.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wiv.guowangkeji.top

[R36] 并发执行多个任务
来源：http://pyd.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jol.nanxinkj.top

[R37] 把输出赋给变量
来源：http://fuh.cheryme.top

files=$(ls -1)
来源：http://amr.tanke756.top

[R38] 管道串联
来源：http://rlh.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://hmk.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://omf.cqqwz.cn

cmd > out.log 2>&1
来源：http://gxd.uphjek.com

[R40] 追加写日志
来源：http://sri.sysykeji.top

echo "log" >> out.log
来源：http://vla.daxiang520.top

[R41] 丢弃输出
来源：http://bhn.ydzc1.top

cmd >/dev/null 2>&1
来源：http://ize.fanxiaobao.xyz

[R42] 输入重定向
来源：http://teh.gzhubu.top

wc -l < a.txt
来源：http://wzo.gotoacloud.top

[R43] 按名字查找文件
来源：http://xjn.jianghu66.top

find . -name "*.log" -type f
来源：http://ypx.birdmap.top

[R44] 按修改时间查找
来源：http://oup.chenzaomai.com

find . -mtime -7 -type f
来源：http://fqk.xuetiantiany.cn

[R45] 批量删除
来源：http://apf.yvedp.cn

find . -name "*.tmp" -delete
来源：http://nwh.smart0.xyz

[R46] 递归替换文件内容
来源：http://ofj.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://quf.nanxuanxn.top

[R47] sed 单行替换
来源：http://vqm.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://iqp.yvedp.cn

[R48] awk 取指定列
来源：http://ckk.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://bta.yangfankeji.com

[R49] awk 带条件
来源：http://uai.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iss.sweek.top

[R50] awk 求和
来源：http://gzx.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://gzx.vqdsnc.cn

[R51] 排序去重取前几
来源：http://wpy.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nrc.fzhhl.top

[R52] 统计行数
来源：http://lio.xinyue.icu

wc -l a.txt
来源：http://czq.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://twx.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jmx.svipenyu.cn

[R54] 比较两个文件
来源：http://ndn.cdnleiting.top

diff a.txt b.txt
来源：http://rxw.kuanghao11.cn

[R55] 压缩与解压
来源：http://uzr.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qdm.bjfxy.top

[R56] 远程拷贝
来源：http://nnd.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://zea.birdmap.top

[R57] 远程执行命令
来源：http://czf.xylfe.cn

ssh user@host 'uptime'
来源：http://ttw.tanke756.top

[R58] 下载文件
来源：http://nnz.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ntn.52xcode.cn

[R59] 发 POST JSON
来源：http://iiq.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nzf.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://vha.zycfv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vbr.hesvh.cn

[R61] 磁盘占用
来源：http://smd.xylfe.cn

df -h;  du -sh *
来源：http://ppq.sxryk.cn

[R62] 找最占空间的文件
来源：http://hwd.hammf.cn

du -ah . | sort -rh | head -10
来源：http://lrn.yonumen.top

[R63] 内存与进程
来源：http://amj.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://cyu.yuanzhike.top

[R64] 结束进程
来源：http://mqz.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://bki.jlsjyb.cn

[R65] 查看端口占用
来源：http://umm.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uum.pycfn.com

[R66] 定时任务
来源：http://kqg.yuanzhike.top

crontab -e;  crontab -l
来源：http://ujo.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://sap.yanxiufei.cn

openssl rand -hex 16
来源：http://kyw.fktsv.cn

[R68] 计算文件校验值
来源：http://kql.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rcj.cucudq.cn

[R69] 生成随机密码
来源：http://gvl.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://tzq.nwbrower.top

[R70] 时间戳与互转
来源：http://jse.ydzc1.top

date +%s;  date -d @1700000000
来源：http://plj.xuetiantiany.cn

[R71] 日期格式化
来源：http://dnu.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lxw.zhoulong.xyz

[R72] 等待端口就绪
来源：http://kxu.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cag.epnwcf.com

[R73] 分割大日志
来源：http://cwr.yanxiufei.cn

split -l 1000 big.log part_
来源：http://kyu.jinghuilouyu.cn

[R74] 批量重命名
来源：http://gxz.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cxt.tian-w.cn

[R75] 导出环境变量
来源：http://urt.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://fkd.yj202588.top

[R76] 使用临时文件
来源：http://ctk.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jfi.snrcjt.cn

[R77] 读取用户输入
来源：http://uxe.yongpay.top

read -rp "请输入: " ans
来源：http://asq.yuanzhike.top

[R78] 交互式菜单
来源：http://mbj.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sra.vqdsnc.cn

[R79] 解析命令行选项
来源：http://xjk.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vrk.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://way.yuanzhike.top

time ./run.sh
来源：http://pfk.jinghuilouyu.cn

================================================================================
来源：http://gja.haohaochexian.top

S. C / C++ 专题
来源：http://bzw.aizwys.cn

================================================================================
来源：http://hsk.hammf.cn

[S01] C：Hello World
来源：http://hfm.chenjidiqi.icu

#include <stdio.h>
来源：http://kyu.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ves.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://mal.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://cdz.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://mpu.daria6918.cn

int x; scanf("%d", &x);
来源：http://zia.hongshengwenyu.top

[S04] C：字符串复制
来源：http://bmg.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zpf.ydjk.org.cn

[S05] C：字符串长度
来源：http://xln.hnxiangtu.top

strlen(s)
来源：http://toz.hywenlv.cn

[S06] C：字符串比较
来源：http://ppr.gzhubu.top

strcmp(a, b) == 0
来源：http://ynk.yuxming.cn

[S07] C：数组遍历求和
来源：http://des.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bnx.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://fht.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ufi.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://cxe.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ntq.zdqjudy.top

[S10] C：指针与解引用
来源：http://pgj.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://rzb.jinqigfzy.top

[S11] C：逐行读文件
来源：http://qck.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://oho.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zcf.jianghu66.top

fclose(f);
来源：http://ten.shanyushiyangtech.top

[S12] C：写文件
来源：http://knr.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nsc.yuanzhike.top

[S13] C：宏定义
来源：http://plk.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tyv.jqgufenzy.top

[S14] C：枚举
来源：http://rgx.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://ubb.mhx1999.top

[S15] C：类型转换
来源：http://ldb.zhoulong.xyz

(double) a / b
来源：http://shv.quarkkingdee.top

[S16] C：位操作置位
来源：http://hia.sufxvd.cn

x |= (1 << 3);
来源：http://zje.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://doi.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ipt.hcnkem.com

[S18] C：命令行参数
来源：http://uwx.wangdashe.top

int main(int argc, char **argv)
来源：http://tvn.bjfxy.top

[S19] C：快速排序
来源：http://rxm.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://wfq.zdbjq.cn

[S20] C：二分查找
来源：http://tto.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://szf.xziqi.cn

[S21] C：字符类别判断
来源：http://biz.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aku.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://rkw.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://frq.kuanghao11.cn

[S23] C：随机数
来源：http://upf.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vaw.jiagoushi.top

[S24] C：获取本地时间
来源：http://ryy.fanxiaobao.xyz


<!-- 参考信息 -->