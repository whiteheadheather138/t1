代发 wailian999

[Q67] 设置隔离级别
来源：http://lfo.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qew.epnwcf.com

[Q68] 保存点
来源：http://vnp.kuanghao11.cn

SAVEPOINT sp1;
来源：http://lkt.hfpthk.cn

ROLLBACK TO sp1;
来源：http://xoh.sysykeji.top

[Q69] 查看执行计划
来源：http://tgf.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://guk.jinqigfzy.top

[Q70] 更新统计信息
来源：http://vzf.zhixingplan.top

ANALYZE TABLE users;
来源：http://xqu.sufxvd.cn

[Q71] 查看建表语句
来源：http://ihr.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mho.bjfxy.top

[Q72] 查看索引
来源：http://fsg.hammf.cn

SHOW INDEX FROM users;
来源：http://uqd.xuetiantiany.cn

[Q73] 查看表状态
来源：http://whs.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://qql.xylfe.cn

[Q74] 强制使用索引
来源：http://ckh.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vdk.tarul.cn

[Q75] 日期格式化
来源：http://ife.hywenlv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hgr.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tmz.hnqzz.top

[Q76] 按天统计
来源：http://eda.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rir.yonumen.top

[Q77] 时间加减
来源：http://mpg.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rwy.dashuyun.cn

[Q78] 当前时间
来源：http://okk.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qov.52xcode.cn

[Q79] 字符串拼接
来源：http://tqo.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dus.nanxuanxn.top

[Q80] 字符串截取
来源：http://ufv.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ann.smart0.xyz

[Q81] 字符串替换
来源：http://jaw.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uua.hesvh.cn

[Q82] 字符长度与字节长度
来源：http://jea.zdbjq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lqj.nanxuanxn.top

[Q83] 大小写转换
来源：http://ydn.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nat.jqgfzy.top

[Q84] 去除首尾空格
来源：http://kaj.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://hyp.smart0.xyz

[Q85] 数值取整
来源：http://jtl.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sxd.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://cna.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jxv.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://zmg.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://abv.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://jkr.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://awh.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iaz.ydzc1.top

[Q89] 判断表是否存在
来源：http://lwv.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hap.yongpay.top

[Q90] 生成序号列
来源：http://snh.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tzr.yanxiufei.cn

================================================================================
来源：http://xag.zhixingplan.top

R. Bash 专题
来源：http://kgj.hnxiangtu.top

================================================================================
来源：http://uyw.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://szi.jinqigfzy.top

#!/usr/bin/env bash
来源：http://qsi.yfazqb.com

set -euo pipefail
来源：http://wdo.316326.xyz

[R02] 变量赋值与使用
来源：http://iiw.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://quj.fehbvm.com

[R03] 只读变量
来源：http://zxn.jinqigfzy.top

readonly PI=3.14
来源：http://pug.shzxlz.cn

[R04] 位置参数
来源：http://syk.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kvd.zhixingplan.top

[R05] 参数默认值
来源：http://wgh.gaohongyu789.top

name="${1:-default}"
来源：http://zaz.haohaochexian.top

[R06] 判断命令是否存在
来源：http://zdj.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kij.shzxlz.cn

[R07] if 判断文件
来源：http://kin.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://llj.guannengcc.top

[R08] 数值比较
来源：http://otb.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://yoy.shzxlz.cn

[R09] 字符串比较
来源：http://saa.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qem.xuetiantiany.cn

[R10] 正则匹配
来源：http://udn.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dex.smart0.xyz

[R11] case 多分支
来源：http://yaq.jlsjyb.cn

case "$1" in
来源：http://ssf.dianchejie.cn

start) echo "启动" ;;
来源：http://nja.xinyue.icu

stop)  echo "停止" ;;
来源：http://zvo.xinyue.icu

*)     echo "未知命令" ;;
来源：http://hvh.svipenyu.cn

esac
来源：http://xej.hnqzz.top

[R12] for 遍历文件
来源：http://vuz.316326.xyz

for f in *.txt; do echo "$f"; done
来源：http://ych.zhaomingkeji.xyz

[R13] for 计数循环
来源：http://fab.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://dyh.shangyingyoupin.top

[R14] C 风格 for
来源：http://hmf.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://klq.c1oappe.top

[R15] while 逐行读文件
来源：http://zei.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hoi.havefunace.top

[R16] until 等待条件
来源：http://xzm.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sxc.cheryme.top

[R17] 数组定义与取值
来源：http://tdj.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ejk.zhengqikj.top

[R18] 遍历数组
来源：http://duf.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mdd.chenzaomai.com

[R19] 数组长度
来源：http://kvv.hnqzz.top

echo "${#arr[@]}"
来源：http://ssd.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://ize.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://igu.vehdjk.com

[R21] 字符串长度
来源：http://pfp.kuanghao11.cn

echo "${#s}"
来源：http://act.ydzc1.top

[R22] 截取子串
来源：http://cww.xinyue.icu

echo "${s:0:5}"
来源：http://iqd.9152youxi.cn

[R23] 字符串替换
来源：http://hpd.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://azr.gaohongyu789.top

[R24] 大小写转换
来源：http://tvh.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gcl.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://vjz.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://czm.cashguo.top

[R26] 命令替换
来源：http://afs.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://qcf.xylfe.cn

[R27] 算术展开
来源：http://xmx.jianghu66.top

echo $((1 + 2 * 3))
来源：http://iio.tarul.cn

[R28] 浮点运算
来源：http://qkx.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://wah.quarkkingdee.top

[R29] 定义函数
来源：http://gvo.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jws.yanxiufei.cn

[R30] 函数返回状态码
来源：http://lzs.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://tob.vqdsnc.cn

[R31] 局部变量
来源：http://cay.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://fej.gzhubu.top

[R32] 参数个数校验
来源：http://quh.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fnm.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://pgy.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sww.c1oappe.top

[R34] 退出时清理
来源：http://moy.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://gvl.fktsv.cn

[R35] 后台执行并等待
来源：http://hpy.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://mcg.zhengqikj.top

[R36] 并发执行多个任务
来源：http://wbu.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://efm.sweek.top

[R37] 把输出赋给变量
来源：http://uci.cqqwz.cn

files=$(ls -1)
来源：http://owk.cucudq.cn

[R38] 管道串联
来源：http://cbk.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://hee.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://dip.xylfe.cn

cmd > out.log 2>&1
来源：http://wdi.chenjidiqi.icu

[R40] 追加写日志
来源：http://wzd.xylfe.cn

echo "log" >> out.log
来源：http://ste.hammf.cn

[R41] 丢弃输出
来源：http://pem.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://pfr.aibaodan.cn

[R42] 输入重定向
来源：http://kpc.jqgufenzy.top

wc -l < a.txt
来源：http://ibq.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://dab.vqdsnc.cn

find . -name "*.log" -type f
来源：http://icy.ctjpmb.com

[R44] 按修改时间查找
来源：http://kqa.jiagoushi.top

find . -mtime -7 -type f
来源：http://whe.sweek.top

[R45] 批量删除
来源：http://ric.ydzc1.top

find . -name "*.tmp" -delete
来源：http://awi.vehdjk.com

[R46] 递归替换文件内容
来源：http://ozi.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ltf.shangyingyoupin.top

[R47] sed 单行替换
来源：http://dxc.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://ndp.zycfv.cn

[R48] awk 取指定列
来源：http://dlb.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://qmb.jlsjyb.cn

[R49] awk 带条件
来源：http://kat.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ell.hammf.cn

[R50] awk 求和
来源：http://eni.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://uoy.chenlongwang.top

[R51] 排序去重取前几
来源：http://tuj.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://tov.svipenyu.cn

[R52] 统计行数
来源：http://dic.hesvh.cn

wc -l a.txt
来源：http://ent.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://pkm.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wfl.nwbrower.top

[R54] 比较两个文件
来源：http://fle.zycfv.cn

diff a.txt b.txt
来源：http://qrb.bbcook.cn

[R55] 压缩与解压
来源：http://eky.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dzm.shzxlz.cn

[R56] 远程拷贝
来源：http://pil.yj20258.top

scp file user@host:/path/
来源：http://whh.hcnkem.com

[R57] 远程执行命令
来源：http://tsq.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://mdx.pengpengdd.cyou

[R58] 下载文件
来源：http://ykj.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tti.yonumen.top

[R59] 发 POST JSON
来源：http://xmx.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ekz.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://fgm.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vec.yuxming.cn

[R61] 磁盘占用
来源：http://nzj.zhongyouzk.top

df -h;  du -sh *
来源：http://fpj.nanxinkj.top

[R62] 找最占空间的文件
来源：http://xop.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://udx.yueranfly.top

[R63] 内存与进程
来源：http://utx.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://ago.c1oappe.top

[R64] 结束进程
来源：http://urj.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://bob.zhongyouzk.top

[R65] 查看端口占用
来源：http://xjh.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nez.jyoumei.cn

[R66] 定时任务
来源：http://eoa.cheryme.top

crontab -e;  crontab -l
来源：http://ygf.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://iyq.yuxming.cn

openssl rand -hex 16
来源：http://gcj.havefunace.top

[R68] 计算文件校验值
来源：http://eyx.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://wyi.mhx1999.top

[R69] 生成随机密码
来源：http://tdh.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://bcd.xuanzx.com

[R70] 时间戳与互转
来源：http://hrc.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://ggc.birdmap.top

[R71] 日期格式化
来源：http://sst.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jdh.c1oappe.top

[R72] 等待端口就绪
来源：http://ydn.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ldj.0kj1m.cn

[R73] 分割大日志
来源：http://nwd.meibo888.top

split -l 1000 big.log part_
来源：http://rqi.nwbrower.top

[R74] 批量重命名
来源：http://gid.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://woy.zhengqikj.top

[R75] 导出环境变量
来源：http://vlg.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://ivf.quarkkingdee.top

[R76] 使用临时文件
来源：http://unf.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zlo.vqdsnc.cn

[R77] 读取用户输入
来源：http://vaw.fehbvm.com

read -rp "请输入: " ans
来源：http://gip.tarul.cn

[R78] 交互式菜单
来源：http://jyu.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lci.vehdjk.com

[R79] 解析命令行选项
来源：http://ybp.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dik.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://khf.shzxlz.cn

time ./run.sh
来源：http://bla.vehdjk.com

================================================================================
来源：http://mdm.jlsjyb.cn

S. C / C++ 专题
来源：http://pnr.pengpengdd.cyou

================================================================================
来源：http://uqp.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://cyn.cucudq.cn

#include <stdio.h>
来源：http://rzr.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jle.meibo888.top

[S02] C：变量与格式化输出
来源：http://psu.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://sfx.vqdsnc.cn

[S03] C：读入整数
来源：http://omc.dianchejie.cn

int x; scanf("%d", &x);
来源：http://nnc.gzhubu.top

[S04] C：字符串复制
来源：http://uyb.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://fnw.jinqigfzy.top

[S05] C：字符串长度
来源：http://rxi.shangyingyoupin.top

strlen(s)
来源：http://dok.havefunace.top

[S06] C：字符串比较
来源：http://jjj.dianchejie.cn

strcmp(a, b) == 0
来源：http://ckk.ehwqpu.com

[S07] C：数组遍历求和
来源：http://nit.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://imn.316326.xyz

[S08] C：动态内存分配与释放
来源：http://wlm.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tdh.cheryme.top

[S09] C：结构体定义与初始化
来源：http://uwd.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uvk.redwolf501.top

[S10] C：指针与解引用
来源：http://nqp.zycfv.cn

int *p = &a;  *p = 5;
来源：http://iya.guowangkeji.top

[S11] C：逐行读文件
来源：http://ach.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://fjf.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cgj.cqqwz.cn

fclose(f);
来源：http://hhc.svipenyu.cn

[S12] C：写文件
来源：http://zoy.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nwe.zhengqikj.top

[S13] C：宏定义
来源：http://oel.sufxvd.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wvb.yuxming.cn

[S14] C：枚举
来源：http://nae.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://qch.epnwcf.com

[S15] C：类型转换
来源：http://qrg.yvedp.cn

(double) a / b
来源：http://bhq.wangdashe.top

[S16] C：位操作置位
来源：http://ect.chenzaomai.com

x |= (1 << 3);
来源：http://uci.pycfn.com

[S17] C：安全拼接字符串
来源：http://ygl.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lvr.fengsongda.top

[S18] C：命令行参数
来源：http://ulf.guowangkeji.top

int main(int argc, char **argv)
来源：http://pth.zycfv.cn

[S19] C：快速排序
来源：http://tez.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tze.zhiwuduotai.top

[S20] C：二分查找
来源：http://kkq.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pto.cashguo.top

[S21] C：字符类别判断
来源：http://glm.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://caw.zdqjudy.top

[S22] C：字符串转数字
来源：http://inr.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://hox.zhengqikj.top

[S23] C：随机数
来源：http://gip.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fhc.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://del.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bhk.havefunace.top

[S25] C：内存拷贝
来源：http://dze.epnwcf.com

memcpy(dst, src, n);
来源：http://chv.shuidangran.top

[S26] C：内存清零
来源：http://ctj.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://fnw.mhx1999.top

[S27] C：定义常量
来源：http://oiz.gogol.net.cn

const double PI = 3.14159;
来源：http://gmt.ctjpmb.com

[S28] C：静态变量
来源：http://yop.nanxinkj.top

static int counter = 0;
来源：http://say.zhoulong.xyz

[S29] C：变参函数
来源：http://fng.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vgu.yuanzhike.top

[S30] C：头文件保护
来源：http://bny.guannengcc.top

#ifndef X_H
来源：http://jdj.cashguo.top

#define X_H
来源：http://cqn.zdqjudy.top

#endif
来源：http://hwc.andypj.xyz

[S31] C++：Hello World
来源：http://mbt.jinqigufen.top

#include <iostream>
来源：http://wvn.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://oni.jinghuilouyu.cn

[S32] C++：字符串
来源：http://udu.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://aqk.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://dyk.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zgd.0kj1m.cn

[S34] C++：遍历 vector
来源：http://bpf.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://bep.c1oappe.top

[S35] C++：map
来源：http://fti.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xyh.guowangkeji.top

[S36] C++：unordered_map
来源：http://crr.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zue.jianghu66.top


<!-- 参考信息 -->