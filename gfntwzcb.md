代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xal.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://vah.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bsd.shuidangran.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rrf.quarkkingdee.top

[Q61] 移动平均
来源：http://vlu.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zkv.gaohongyu789.top

[Q62] 分组占比
来源：http://ans.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jle.andypj.xyz

[Q63] 开启事务
来源：http://myp.zycfv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tfw.epnwcf.com

[Q64] 提交事务
来源：http://bif.cdnleiting.top

COMMIT;
来源：http://gbm.mhx1999.top

[Q65] 回滚事务
来源：http://dqh.aibaodan.cn

ROLLBACK;
来源：http://ymo.gzhubu.top

[Q66] 行锁查询
来源：http://rmb.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ska.tarul.cn

[Q67] 设置隔离级别
来源：http://rkr.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zzs.xuetiantiany.cn

[Q68] 保存点
来源：http://lgo.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://zyn.hcnkem.com

ROLLBACK TO sp1;
来源：http://pxb.yongpay.top

[Q69] 查看执行计划
来源：http://ned.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bzr.epnwcf.com

[Q70] 更新统计信息
来源：http://cjq.yj20258.top

ANALYZE TABLE users;
来源：http://wij.hfpthk.cn

[Q71] 查看建表语句
来源：http://scz.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bmm.yueranfly.top

[Q72] 查看索引
来源：http://bhr.iojbl.cn

SHOW INDEX FROM users;
来源：http://yia.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://law.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zda.zdqjudy.top

[Q74] 强制使用索引
来源：http://fhd.cheryme.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zbs.yuxming.cn

[Q75] 日期格式化
来源：http://lyv.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yuu.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iad.xziqi.cn

[Q76] 按天统计
来源：http://iap.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oaa.jinqigfzy.top

[Q77] 时间加减
来源：http://qdx.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://isn.jyoumei.cn

[Q78] 当前时间
来源：http://ypt.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xqi.sxryk.cn

[Q79] 字符串拼接
来源：http://jsr.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wyo.zhixingplan.top

[Q80] 字符串截取
来源：http://ymu.zhongyouzk.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xzi.ivvv.top

[Q81] 字符串替换
来源：http://xzt.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nep.9152youxi.cn

[Q82] 字符长度与字节长度
来源：http://srj.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://irt.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://yri.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gcv.fengsongda.top

[Q84] 去除首尾空格
来源：http://ciw.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://oaq.jqgufenzy.top

[Q85] 数值取整
来源：http://ecv.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xjo.nanxinkj.top

[Q86] 读取 JSON 字段
来源：http://pik.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hzs.yueranfly.top

[Q87] JSON 字段做条件
来源：http://bpl.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rhw.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://ylg.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ttj.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://izp.sysykeji.top

[Q89] 判断表是否存在
来源：http://net.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dcs.zhijiandao.cn

[Q90] 生成序号列
来源：http://shk.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jeq.zhaomingkeji.xyz

================================================================================
来源：http://lbz.zhiwuduotai.top

R. Bash 专题
来源：http://qxw.zhiwuduotai.top

================================================================================
来源：http://uhe.hfpthk.cn

[R01] shebang 与严格模式
来源：http://qrx.ydjk.org.cn

#!/usr/bin/env bash
来源：http://jtg.tian-w.cn

set -euo pipefail
来源：http://agg.ctjpmb.com

[R02] 变量赋值与使用
来源：http://iwp.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://zxr.fehbvm.com

[R03] 只读变量
来源：http://ndx.fktsv.cn

readonly PI=3.14
来源：http://dow.ydzc1.top

[R04] 位置参数
来源：http://bia.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gyo.cdnleiting.top

[R05] 参数默认值
来源：http://qis.gogol.net.cn

name="${1:-default}"
来源：http://ffw.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://ads.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cry.shuidangran.top

[R07] if 判断文件
来源：http://tom.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://osw.sjlbkw.cn

[R08] 数值比较
来源：http://hbd.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uqu.shangyingyoupin.top

[R09] 字符串比较
来源：http://dbj.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mbp.ivvv.top

[R10] 正则匹配
来源：http://qvb.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://unf.havefunace.top

[R11] case 多分支
来源：http://opr.wangdashe.top

case "$1" in
来源：http://rae.vqdsnc.cn

start) echo "启动" ;;
来源：http://put.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://rol.c1oappe.top

*)     echo "未知命令" ;;
来源：http://wig.smart0.xyz

esac
来源：http://kgt.yvedp.cn

[R12] for 遍历文件
来源：http://ppd.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://ldd.dashuyun.cn

[R13] for 计数循环
来源：http://eho.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://tfa.gotoacloud.top

[R14] C 风格 for
来源：http://smv.smart0.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://now.cdnleiting.top

[R15] while 逐行读文件
来源：http://pks.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kch.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://aak.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://acj.xinyue.icu

[R17] 数组定义与取值
来源：http://wnf.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://xyt.daria6918.cn

[R18] 遍历数组
来源：http://cup.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://msv.gzhubu.top

[R19] 数组长度
来源：http://aok.yongpay.top

echo "${#arr[@]}"
来源：http://txj.xziqi.cn

[R20] 关联数组（字典）
来源：http://bjj.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mcn.tianlin.xyz

[R21] 字符串长度
来源：http://mgw.yangfankeji.com

echo "${#s}"
来源：http://pcc.gaohongyu789.top

[R22] 截取子串
来源：http://xew.nanxinkj.top

echo "${s:0:5}"
来源：http://hpv.yueranfly.top

[R23] 字符串替换
来源：http://afl.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gqe.sysykeji.top

[R24] 大小写转换
来源：http://cxg.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sav.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://sof.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kqc.daxiang520.top

[R26] 命令替换
来源：http://xso.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://cev.zhiwuduotai.top

[R27] 算术展开
来源：http://udd.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://int.shzxlz.cn

[R28] 浮点运算
来源：http://cer.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://gkm.shzxlz.cn

[R29] 定义函数
来源：http://bwu.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yut.tianlin.xyz

[R30] 函数返回状态码
来源：http://crt.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://izi.vehdjk.com

[R31] 局部变量
来源：http://vhb.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://lwi.hfpthk.cn

[R32] 参数个数校验
来源：http://ovc.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oqm.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://bmw.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lzr.yueranfly.top

[R34] 退出时清理
来源：http://kii.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dvh.hfpthk.cn

[R35] 后台执行并等待
来源：http://acn.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ncu.birdmap.top

[R36] 并发执行多个任务
来源：http://smj.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://spw.xuanzx.com

[R37] 把输出赋给变量
来源：http://fio.ybcxt.top

files=$(ls -1)
来源：http://qip.havefunace.top

[R38] 管道串联
来源：http://gca.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://dyi.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://wcr.jqgfzy.top

cmd > out.log 2>&1
来源：http://sle.redwolf501.top

[R40] 追加写日志
来源：http://aox.zdqjudy.top

echo "log" >> out.log
来源：http://jbu.guannengcc.top

[R41] 丢弃输出
来源：http://hao.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://gaz.guannengcc.top

[R42] 输入重定向
来源：http://jun.cucudq.cn

wc -l < a.txt
来源：http://etd.jiagoushi.top

[R43] 按名字查找文件
来源：http://hoh.tian-w.cn

find . -name "*.log" -type f
来源：http://fhq.nanxuanxn.top

[R44] 按修改时间查找
来源：http://bkz.jianghu66.top

find . -mtime -7 -type f
来源：http://luv.meibo888.top

[R45] 批量删除
来源：http://mhd.pycfn.com

find . -name "*.tmp" -delete
来源：http://kjh.bbcook.cn

[R46] 递归替换文件内容
来源：http://qre.ybcxt.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mme.tianlin.xyz

[R47] sed 单行替换
来源：http://kbh.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://jhp.zhongyouzk.top

[R48] awk 取指定列
来源：http://kiy.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://ppz.jqgfzy.top

[R49] awk 带条件
来源：http://kjr.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://msw.sweek.top

[R50] awk 求和
来源：http://gaj.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uns.tarul.cn

[R51] 排序去重取前几
来源：http://xcq.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qil.cheryme.top

[R52] 统计行数
来源：http://fxf.epnwcf.com

wc -l a.txt
来源：http://bhp.yj20258.top

[R53] 查看文件头与实时尾
来源：http://vnq.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cqg.xinyue.icu

[R54] 比较两个文件
来源：http://qyd.jinghuilouyu.cn

diff a.txt b.txt
来源：http://ewv.zhongyouzk.top

[R55] 压缩与解压
来源：http://qgb.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://egs.xinyue.icu

[R56] 远程拷贝
来源：http://ogi.fanxiaobao.xyz

scp file user@host:/path/
来源：http://zvg.fengsongda.top

[R57] 远程执行命令
来源：http://guv.jinqigufen.top

ssh user@host 'uptime'
来源：http://lht.chenzaomai.com

[R58] 下载文件
来源：http://naf.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sde.daria6918.cn

[R59] 发 POST JSON
来源：http://fvc.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://soz.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://njb.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tkl.guannengcc.top

[R61] 磁盘占用
来源：http://xky.fengsongda.top

df -h;  du -sh *
来源：http://eua.jqgfzy.top

[R62] 找最占空间的文件
来源：http://vei.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://dfj.ydjk.org.cn

[R63] 内存与进程
来源：http://vxz.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://vmw.hnqzz.top

[R64] 结束进程
来源：http://lbf.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://hew.52xcode.cn

[R65] 查看端口占用
来源：http://awf.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tak.sufxvd.cn

[R66] 定时任务
来源：http://ijb.jinqigfzy.top

crontab -e;  crontab -l
来源：http://mpj.cashguo.top

[R67] 生成随机十六进制串
来源：http://gew.jlsjyb.cn

openssl rand -hex 16
来源：http://kkg.redwolf501.top

[R68] 计算文件校验值
来源：http://wof.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://jns.gaohongyu789.top

[R69] 生成随机密码
来源：http://rby.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://qvf.iojbl.cn

[R70] 时间戳与互转
来源：http://bfk.yonumen.top

date +%s;  date -d @1700000000
来源：http://iko.ydjk.org.cn

[R71] 日期格式化
来源：http://nzp.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dfi.wangdashe.top

[R72] 等待端口就绪
来源：http://jsw.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zsw.cdnleiting.top

[R73] 分割大日志
来源：http://ueq.316326.xyz

split -l 1000 big.log part_
来源：http://ecx.xuetiantiany.cn

[R74] 批量重命名
来源：http://hnz.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mwi.jiagoushi.top

[R75] 导出环境变量
来源：http://vgw.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://fob.shuidangran.top

[R76] 使用临时文件
来源：http://jbb.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hih.zhijiandao.cn

[R77] 读取用户输入
来源：http://kay.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://joh.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://iqj.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pqz.daria6918.cn

[R79] 解析命令行选项
来源：http://qch.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fmy.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://gqn.ctjpmb.com

time ./run.sh
来源：http://jua.dianchejie.cn

================================================================================
来源：http://rcc.hywenlv.cn

S. C / C++ 专题
来源：http://exv.tian-w.cn

================================================================================
来源：http://ixw.hnxiangtu.top

[S01] C：Hello World
来源：http://tsl.xuanzx.com

#include <stdio.h>
来源：http://zpf.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mgl.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://yjt.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://zqq.hysaishi.cn

[S03] C：读入整数
来源：http://ops.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://ylx.birdmap.top

[S04] C：字符串复制
来源：http://efy.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tnn.jianghu66.top

[S05] C：字符串长度
来源：http://dfv.jqgfzy.top

strlen(s)
来源：http://wiy.xylfe.cn

[S06] C：字符串比较
来源：http://dae.epnwcf.com

strcmp(a, b) == 0
来源：http://shr.zdbjq.cn

[S07] C：数组遍历求和
来源：http://mri.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://odg.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://fwr.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bok.hongshengwenyu.top

[S09] C：结构体定义与初始化
来源：http://qnz.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ccq.gzhubu.top

[S10] C：指针与解引用
来源：http://xgn.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://nlx.ybcxt.top

[S11] C：逐行读文件
来源：http://xle.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://cry.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pgo.hcnkem.com

fclose(f);
来源：http://ylp.cucudq.cn

[S12] C：写文件
来源：http://hgw.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sme.ivvv.top

[S13] C：宏定义
来源：http://yfv.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ntz.haohaochexian.top

[S14] C：枚举
来源：http://hbv.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://gql.birdmap.top

[S15] C：类型转换
来源：http://fts.jianghu66.top

(double) a / b
来源：http://flc.sufxvd.cn

[S16] C：位操作置位
来源：http://uqp.hnqzz.top

x |= (1 << 3);
来源：http://slt.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://gzt.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://njy.zdbjq.cn

[S18] C：命令行参数
来源：http://fub.hnqzz.top

int main(int argc, char **argv)
来源：http://tsi.chenjidiqi.icu

[S19] C：快速排序
来源：http://esg.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://tjo.ppjwa.cn

[S20] C：二分查找
来源：http://cag.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://run.hnxiangtu.top

[S21] C：字符类别判断
来源：http://oud.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oxm.cheryme.top

[S22] C：字符串转数字
来源：http://ttx.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sft.nanxinkj.top

[S23] C：随机数
来源：http://izy.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oac.haohaochexian.top

[S24] C：获取本地时间
来源：http://nde.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eiw.yongpay.top

[S25] C：内存拷贝
来源：http://bdu.yj20258888.top

memcpy(dst, src, n);
来源：http://ctx.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://bhb.tarul.cn

memset(a, 0, sizeof a);
来源：http://pec.redwolf501.top

[S27] C：定义常量
来源：http://hhh.hesvh.cn

const double PI = 3.14159;
来源：http://ylg.dianchejie.cn

[S28] C：静态变量
来源：http://ywx.shzxlz.cn

static int counter = 0;
来源：http://fhf.fengsongda.top

[S29] C：变参函数
来源：http://bci.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eju.svipenyu.cn

[S30] C：头文件保护
来源：http://mht.tian-w.cn


<!-- 参考信息 -->