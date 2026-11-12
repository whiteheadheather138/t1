代发 wailian999

[Q65] 回滚事务
来源：http://yam.yj20258888.top

ROLLBACK;
来源：http://kwt.gaohongyu789.top

[Q66] 行锁查询
来源：http://dqh.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rdq.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://aqo.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oih.yvedp.cn

[Q68] 保存点
来源：http://ojf.yongpay.top

SAVEPOINT sp1;
来源：http://imc.zhengqikj.top

ROLLBACK TO sp1;
来源：http://qsf.hcnkem.com

[Q69] 查看执行计划
来源：http://jpo.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yvk.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://wsp.yuxming.cn

ANALYZE TABLE users;
来源：http://peh.zdqjudy.top

[Q71] 查看建表语句
来源：http://twd.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://knc.svipenyu.cn

[Q72] 查看索引
来源：http://htd.havefunace.top

SHOW INDEX FROM users;
来源：http://hzk.dashuyun.cn

[Q73] 查看表状态
来源：http://sal.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lca.yfazqb.com

[Q74] 强制使用索引
来源：http://zmz.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uxv.birdmap.top

[Q75] 日期格式化
来源：http://kfm.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ysl.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vvv.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://gsd.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://agk.jianghu66.top

[Q77] 时间加减
来源：http://mac.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sbc.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://iiz.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lka.sxryk.cn

[Q79] 字符串拼接
来源：http://spv.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jub.nwbrower.top

[Q80] 字符串截取
来源：http://cpi.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://omm.pengpengdd.cyou

[Q81] 字符串替换
来源：http://obr.iojbl.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ayf.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://vdf.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fui.chenjidiqi.icu

[Q83] 大小写转换
来源：http://nqq.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yuy.fehbvm.com

[Q84] 去除首尾空格
来源：http://izq.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://fdl.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://zve.zhijiandao.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hyv.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://ohs.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bjj.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://eha.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pln.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://chh.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqr.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://esf.yongpay.top

[Q89] 判断表是否存在
来源：http://jzo.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hkr.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://bwj.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qcc.zdbjq.cn

================================================================================
来源：http://tcb.sufxvd.cn

R. Bash 专题
来源：http://log.ppjwa.cn

================================================================================
来源：http://dqv.cqqwz.cn

[R01] shebang 与严格模式
来源：http://efz.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://cvm.yfazqb.com

set -euo pipefail
来源：http://ses.vehdjk.com

[R02] 变量赋值与使用
来源：http://ozy.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://fhu.ydjk.org.cn

[R03] 只读变量
来源：http://jpd.fanxiaobao.xyz

readonly PI=3.14
来源：http://zoo.yfazqb.com

[R04] 位置参数
来源：http://jrc.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xhz.jiagoushi.top

[R05] 参数默认值
来源：http://rhf.sjlbkw.cn

name="${1:-default}"
来源：http://wsp.birdmap.top

[R06] 判断命令是否存在
来源：http://sju.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rnm.yangfankeji.com

[R07] if 判断文件
来源：http://zqq.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xxh.bjfxy.top

[R08] 数值比较
来源：http://wnx.wangdashe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ojw.fehbvm.com

[R09] 字符串比较
来源：http://eiq.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xvx.epnwcf.com

[R10] 正则匹配
来源：http://sog.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oki.zhixingplan.top

[R11] case 多分支
来源：http://yno.snrcjt.cn

case "$1" in
来源：http://gwg.hammf.cn

start) echo "启动" ;;
来源：http://axt.bjfxy.top

stop)  echo "停止" ;;
来源：http://yza.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://eiw.kuanghao11.cn

esac
来源：http://jdf.jqgufenzy.top

[R12] for 遍历文件
来源：http://aut.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://txd.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://atv.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://jys.shangyingyoupin.top

[R14] C 风格 for
来源：http://fyf.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nxd.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://vvl.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sam.nanxinkj.top

[R16] until 等待条件
来源：http://uth.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cig.nanxuanxn.top

[R17] 数组定义与取值
来源：http://nuj.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://avt.birdmap.top

[R18] 遍历数组
来源：http://jjz.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zyg.xuetiantiany.cn

[R19] 数组长度
来源：http://vpa.sjlbkw.cn

echo "${#arr[@]}"
来源：http://bqk.yj202588.top

[R20] 关联数组（字典）
来源：http://evz.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vos.tanke756.top

[R21] 字符串长度
来源：http://hve.kuanghao11.cn

echo "${#s}"
来源：http://fih.yongpay.top

[R22] 截取子串
来源：http://ely.hywenlv.cn

echo "${s:0:5}"
来源：http://ywr.bbcook.cn

[R23] 字符串替换
来源：http://cll.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bbw.ydjk.org.cn

[R24] 大小写转换
来源：http://dbc.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cpq.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://hpb.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://brx.mhx1999.top

[R26] 命令替换
来源：http://zsy.yuxming.cn

now=$(date +%F); echo "$now"
来源：http://lne.zhiwuduotai.top

[R27] 算术展开
来源：http://oks.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://bxy.snrcjt.cn

[R28] 浮点运算
来源：http://zfz.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://rip.zhaomingkeji.xyz

[R29] 定义函数
来源：http://kpj.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aoa.bbcook.cn

[R30] 函数返回状态码
来源：http://krb.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://yuu.cqqwz.cn

[R31] 局部变量
来源：http://tbw.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://ujb.yfazqb.com

[R32] 参数个数校验
来源：http://hjn.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ewm.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://agx.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://csm.yfazqb.com

[R34] 退出时清理
来源：http://rih.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://cxk.zdqjudy.top

[R35] 后台执行并等待
来源：http://nbk.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wsa.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://uap.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://emp.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://jgl.cucudq.cn

files=$(ls -1)
来源：http://lbu.yj20258888.top

[R38] 管道串联
来源：http://zwh.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://nwc.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://tet.svipenyu.cn

cmd > out.log 2>&1
来源：http://whe.guowangkeji.top

[R40] 追加写日志
来源：http://qki.andypj.xyz

echo "log" >> out.log
来源：http://mgj.ybcxt.top

[R41] 丢弃输出
来源：http://fdi.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://kku.cqqwz.cn

[R42] 输入重定向
来源：http://fox.svipenyu.cn

wc -l < a.txt
来源：http://pln.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://hdb.fktsv.cn

find . -name "*.log" -type f
来源：http://kce.zdbjq.cn

[R44] 按修改时间查找
来源：http://pif.svipenyu.cn

find . -mtime -7 -type f
来源：http://rdd.jlsjyb.cn

[R45] 批量删除
来源：http://ifx.xinyue.icu

find . -name "*.tmp" -delete
来源：http://oih.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://gkv.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mky.pengpengdd.cyou

[R47] sed 单行替换
来源：http://avy.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://zyu.bbcook.cn

[R48] awk 取指定列
来源：http://xxz.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://upx.xinyue.icu

[R49] awk 带条件
来源：http://mut.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mqj.pengpengdd.cyou

[R50] awk 求和
来源：http://gwo.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://kpu.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://vej.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://yzk.pengpengdd.cyou

[R52] 统计行数
来源：http://fjf.mhx1999.top

wc -l a.txt
来源：http://fds.cashguo.top

[R53] 查看文件头与实时尾
来源：http://imx.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hwd.shzxlz.cn

[R54] 比较两个文件
来源：http://qml.tanke756.top

diff a.txt b.txt
来源：http://rsb.wangdashe.top

[R55] 压缩与解压
来源：http://csu.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jbu.sjlbkw.cn

[R56] 远程拷贝
来源：http://ndi.fktsv.cn

scp file user@host:/path/
来源：http://zdm.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://yhl.zhongyouzk.top

ssh user@host 'uptime'
来源：http://ssg.svipenyu.cn

[R58] 下载文件
来源：http://gth.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qnh.jianghu66.top

[R59] 发 POST JSON
来源：http://jwd.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ksh.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://vfv.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://leb.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://vmc.cashguo.top

df -h;  du -sh *
来源：http://eky.zycfv.cn

[R62] 找最占空间的文件
来源：http://fna.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://vum.snrcjt.cn

[R63] 内存与进程
来源：http://yhe.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://zdt.tanke756.top

[R64] 结束进程
来源：http://dku.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://ggi.dashuyun.cn

[R65] 查看端口占用
来源：http://ioq.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://per.fzhhl.top

[R66] 定时任务
来源：http://ujv.yj202588.top

crontab -e;  crontab -l
来源：http://ctu.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://oxt.aibaodan.cn

openssl rand -hex 16
来源：http://rnm.xziqi.cn

[R68] 计算文件校验值
来源：http://rjm.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uxt.tarul.cn

[R69] 生成随机密码
来源：http://big.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://nwx.tarul.cn

[R70] 时间戳与互转
来源：http://jfl.xziqi.cn

date +%s;  date -d @1700000000
来源：http://zpj.yuxming.cn

[R71] 日期格式化
来源：http://mxr.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://amw.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://cai.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jll.fanxiaobao.xyz

[R73] 分割大日志
来源：http://unm.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://pfx.xziqi.cn

[R74] 批量重命名
来源：http://tso.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pwk.316326.xyz

[R75] 导出环境变量
来源：http://vpg.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://cfh.zhixingplan.top

[R76] 使用临时文件
来源：http://irr.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gzx.iojbl.cn

[R77] 读取用户输入
来源：http://xil.jyoumei.cn

read -rp "请输入: " ans
来源：http://oam.aibaodan.cn

[R78] 交互式菜单
来源：http://mqi.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mcy.ydjk.org.cn

[R79] 解析命令行选项
来源：http://wqf.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wok.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://qbq.jinghuilouyu.cn

time ./run.sh
来源：http://vgo.shanyushiyangtech.top

================================================================================
来源：http://iug.yj20258888.top

S. C / C++ 专题
来源：http://bpr.chenjidiqi.icu

================================================================================
来源：http://twe.snrcjt.cn

[S01] C：Hello World
来源：http://qge.hammf.cn

#include <stdio.h>
来源：http://fqz.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fan.tarul.cn

[S02] C：变量与格式化输出
来源：http://irj.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://nuo.ctjpmb.com

[S03] C：读入整数
来源：http://bmo.epnwcf.com

int x; scanf("%d", &x);
来源：http://zrb.ydzc1.top

[S04] C：字符串复制
来源：http://uxl.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://onz.xuetiantiany.cn

[S05] C：字符串长度
来源：http://gsv.wangdashe.top

strlen(s)
来源：http://rtb.yfazqb.com

[S06] C：字符串比较
来源：http://ddj.xuanzx.com

strcmp(a, b) == 0
来源：http://nvv.ppjwa.cn

[S07] C：数组遍历求和
来源：http://ruq.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ymr.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://xwb.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ork.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://mgp.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://giy.xziqi.cn

[S10] C：指针与解引用
来源：http://loa.uphjek.com

int *p = &a;  *p = 5;
来源：http://phw.yongpay.top

[S11] C：逐行读文件
来源：http://jxz.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://xpz.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://frf.tarul.cn

fclose(f);
来源：http://mla.yj20258.top

[S12] C：写文件
来源：http://dsd.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pbn.mhx1999.top

[S13] C：宏定义
来源：http://owq.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://prb.hesvh.cn

[S14] C：枚举
来源：http://laa.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://baw.hnqzz.top

[S15] C：类型转换
来源：http://xfz.jinqigufen.top

(double) a / b
来源：http://otb.nanxinkj.top

[S16] C：位操作置位
来源：http://dja.cdnleiting.top

x |= (1 << 3);
来源：http://wye.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://xrv.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qba.birdmap.top

[S18] C：命令行参数
来源：http://gsn.316326.xyz

int main(int argc, char **argv)
来源：http://zpc.zhoulong.xyz

[S19] C：快速排序
来源：http://blh.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ufj.haohaochexian.top

[S20] C：二分查找
来源：http://cws.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zum.yuanzhike.top

[S21] C：字符类别判断
来源：http://wdk.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ycq.c1oappe.top

[S22] C：字符串转数字
来源：http://kcy.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kbb.pycfn.com

[S23] C：随机数
来源：http://bzk.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kgh.jinqigufen.top

[S24] C：获取本地时间
来源：http://okx.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ufg.redwolf501.top

[S25] C：内存拷贝
来源：http://nec.yueranfly.top

memcpy(dst, src, n);
来源：http://qqe.pengpengdd.cyou

[S26] C：内存清零
来源：http://xip.pycfn.com

memset(a, 0, sizeof a);
来源：http://bup.tianlin.xyz

[S27] C：定义常量
来源：http://soh.zhijiandao.cn

const double PI = 3.14159;
来源：http://xvb.havefunace.top

[S28] C：静态变量
来源：http://bpc.yongpay.top

static int counter = 0;
来源：http://nvf.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://tvq.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iuq.ppjwa.cn

[S30] C：头文件保护
来源：http://zfd.iojbl.cn

#ifndef X_H
来源：http://ybo.ywan-chungtsiang.top

#define X_H
来源：http://mfe.tanke756.top

#endif
来源：http://mrt.andypj.xyz

[S31] C++：Hello World
来源：http://nrx.nwbrower.top

#include <iostream>
来源：http://emb.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://vui.daria6918.cn

[S32] C++：字符串
来源：http://nbv.yonumen.top

std::string s = "hi";  s += "!";
来源：http://gtm.fktsv.cn

[S33] C++：vector 增删
来源：http://xky.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sxu.gogol.net.cn

[S34] C++：遍历 vector
来源：http://egv.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://pmc.ehwqpu.com


<!-- 参考信息 -->