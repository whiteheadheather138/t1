代发 wailian999

ANALYZE TABLE users;
来源：http://smv.xinyue.icu

[Q71] 查看建表语句
来源：http://awj.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://plm.sxryk.cn

[Q72] 查看索引
来源：http://kqd.xziqi.cn

SHOW INDEX FROM users;
来源：http://kyv.havefunace.top

[Q73] 查看表状态
来源：http://czb.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rmd.cqqwz.cn

[Q74] 强制使用索引
来源：http://utd.snrcjt.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ujy.hongshengwenyu.top

[Q75] 日期格式化
来源：http://duy.hnxiangtu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://psv.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fjf.jianghu66.top

[Q76] 按天统计
来源：http://ehl.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ooi.shuidangran.top

[Q77] 时间加减
来源：http://sah.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cpz.guannengcc.top

[Q78] 当前时间
来源：http://atb.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://prx.hysaishi.cn

[Q79] 字符串拼接
来源：http://lvu.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hqr.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://jjs.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tuo.yanxiufei.cn

[Q81] 字符串替换
来源：http://akz.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://etf.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://fgk.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wqc.guowangkeji.top

[Q83] 大小写转换
来源：http://flo.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dtj.chenzaomai.com

[Q84] 去除首尾空格
来源：http://qwa.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://cit.0kj1m.cn

[Q85] 数值取整
来源：http://rwm.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bxi.yj20258.top

[Q86] 读取 JSON 字段
来源：http://xcj.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cfh.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://adx.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iop.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://nsw.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://puh.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mrz.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://xfa.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jng.zhengqikj.top

[Q90] 生成序号列
来源：http://wfc.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mmd.chenzaomai.com

================================================================================
来源：http://ogg.uphjek.com

R. Bash 专题
来源：http://pmq.zhoulong.xyz

================================================================================
来源：http://zvt.tarul.cn

[R01] shebang 与严格模式
来源：http://azs.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://qlt.hfpthk.cn

set -euo pipefail
来源：http://ted.xuanzx.com

[R02] 变量赋值与使用
来源：http://gwi.shuidangran.top

name="Tom"; echo "$name"
来源：http://bri.vqdsnc.cn

[R03] 只读变量
来源：http://kdk.jinqigufen.top

readonly PI=3.14
来源：http://ngs.uphjek.com

[R04] 位置参数
来源：http://cjh.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kxm.epnwcf.com

[R05] 参数默认值
来源：http://zhc.epnwcf.com

name="${1:-default}"
来源：http://eaf.mhx1999.top

[R06] 判断命令是否存在
来源：http://nkk.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mlv.dianchejie.cn

[R07] if 判断文件
来源：http://xqj.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kbl.aibaodan.cn

[R08] 数值比较
来源：http://vgd.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hnk.meibo888.top

[R09] 字符串比较
来源：http://gbe.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://foz.ydzc1.top

[R10] 正则匹配
来源：http://qec.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aih.snrcjt.cn

[R11] case 多分支
来源：http://lip.zhixingplan.top

case "$1" in
来源：http://wzp.chenjidiqi.icu

start) echo "启动" ;;
来源：http://zzy.fengsongda.top

stop)  echo "停止" ;;
来源：http://wfj.sysykeji.top

*)     echo "未知命令" ;;
来源：http://cve.sweek.top

esac
来源：http://tte.zycfv.cn

[R12] for 遍历文件
来源：http://cbt.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://beg.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://fwz.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://zkr.9152youxi.cn

[R14] C 风格 for
来源：http://nrs.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pir.nanxinkj.top

[R15] while 逐行读文件
来源：http://emm.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lue.hnxiangtu.top

[R16] until 等待条件
来源：http://ndb.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uqh.yj20258.top

[R17] 数组定义与取值
来源：http://jum.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://rop.zhoulong.xyz

[R18] 遍历数组
来源：http://xyl.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fya.pycfn.com

[R19] 数组长度
来源：http://sdw.hcnkem.com

echo "${#arr[@]}"
来源：http://zrp.xylfe.cn

[R20] 关联数组（字典）
来源：http://vua.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nps.guowangkeji.top

[R21] 字符串长度
来源：http://geh.vqdsnc.cn

echo "${#s}"
来源：http://lle.xinyue.icu

[R22] 截取子串
来源：http://rcv.cdnleiting.top

echo "${s:0:5}"
来源：http://pri.nanxinkj.top

[R23] 字符串替换
来源：http://zau.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xbv.yuanzhike.top

[R24] 大小写转换
来源：http://mst.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://nkm.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://xza.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rdz.sjlbkw.cn

[R26] 命令替换
来源：http://mbd.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://jqa.shuidangran.top

[R27] 算术展开
来源：http://ddn.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://mly.xinyue.icu

[R28] 浮点运算
来源：http://jsn.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://kvm.snrcjt.cn

[R29] 定义函数
来源：http://lay.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iuj.kuanghao11.cn

[R30] 函数返回状态码
来源：http://pfs.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://hig.shanyushiyangkeji.top

[R31] 局部变量
来源：http://log.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://zpj.zhixingplan.top

[R32] 参数个数校验
来源：http://mex.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tbu.yj202588.top

[R33] 捕获错误并提示行号
来源：http://fvz.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nmr.tanke756.top

[R34] 退出时清理
来源：http://ofd.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gjt.yangfankeji.com

[R35] 后台执行并等待
来源：http://bft.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ndr.hfpthk.cn

[R36] 并发执行多个任务
来源：http://frd.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nej.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://qjx.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://xmk.shzxlz.cn

[R38] 管道串联
来源：http://vix.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://txz.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://vcr.birdmap.top

cmd > out.log 2>&1
来源：http://yej.zhijiandao.cn

[R40] 追加写日志
来源：http://nzq.yj20258888.top

echo "log" >> out.log
来源：http://uxd.quarkkingdee.top

[R41] 丢弃输出
来源：http://uux.meibo888.top

cmd >/dev/null 2>&1
来源：http://hzd.birdmap.top

[R42] 输入重定向
来源：http://clr.xylfe.cn

wc -l < a.txt
来源：http://bmb.jianghu66.top

[R43] 按名字查找文件
来源：http://duf.cdnleiting.top

find . -name "*.log" -type f
来源：http://dlj.ivvv.top

[R44] 按修改时间查找
来源：http://rjg.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://lxa.aibaodan.cn

[R45] 批量删除
来源：http://tql.yonumen.top

find . -name "*.tmp" -delete
来源：http://bwi.guowangkeji.top

[R46] 递归替换文件内容
来源：http://ztc.ybcxt.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ljf.xziqi.cn

[R47] sed 单行替换
来源：http://jsl.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yav.haohaochexian.top

[R48] awk 取指定列
来源：http://nff.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://sfx.zdqjudy.top

[R49] awk 带条件
来源：http://hsi.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://myu.sysykeji.top

[R50] awk 求和
来源：http://vja.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://ejb.zhijiandao.cn

[R51] 排序去重取前几
来源：http://iug.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pac.daria6918.cn

[R52] 统计行数
来源：http://zqi.yongpay.top

wc -l a.txt
来源：http://lvk.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://qmv.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lad.jiagoushi.top

[R54] 比较两个文件
来源：http://cye.ybcxt.top

diff a.txt b.txt
来源：http://idz.0kj1m.cn

[R55] 压缩与解压
来源：http://uge.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qek.jinqigfzy.top

[R56] 远程拷贝
来源：http://twn.tarul.cn

scp file user@host:/path/
来源：http://sja.bjfxy.top

[R57] 远程执行命令
来源：http://agy.ivvv.top

ssh user@host 'uptime'
来源：http://iad.jinghuilouyu.cn

[R58] 下载文件
来源：http://pyi.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rdo.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://trc.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bfw.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://unz.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rbc.sweek.top

[R61] 磁盘占用
来源：http://ptv.zhoulong.xyz

df -h;  du -sh *
来源：http://wml.zycfv.cn

[R62] 找最占空间的文件
来源：http://xcg.yj202588.top

du -ah . | sort -rh | head -10
来源：http://lfv.hnxiangtu.top

[R63] 内存与进程
来源：http://iqo.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://jys.smart0.xyz

[R64] 结束进程
来源：http://pdm.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://kwq.zhixingplan.top

[R65] 查看端口占用
来源：http://abu.guowangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gpd.gzhubu.top

[R66] 定时任务
来源：http://vnz.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://oda.hnqzz.top

[R67] 生成随机十六进制串
来源：http://djw.cashguo.top

openssl rand -hex 16
来源：http://pfd.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://xxx.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://wkb.ybcxt.top

[R69] 生成随机密码
来源：http://uvp.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://lbm.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://rlw.havefunace.top

date +%s;  date -d @1700000000
来源：http://qkh.zhengqikj.top

[R71] 日期格式化
来源：http://kas.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wrt.zhijiandao.cn

[R72] 等待端口就绪
来源：http://aje.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nts.fengsongda.top

[R73] 分割大日志
来源：http://lea.zhijiandao.cn

split -l 1000 big.log part_
来源：http://psd.ybcxt.top

[R74] 批量重命名
来源：http://gpw.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xtp.bbcook.cn

[R75] 导出环境变量
来源：http://brr.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://uck.sweek.top

[R76] 使用临时文件
来源：http://gjm.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rsy.fehbvm.com

[R77] 读取用户输入
来源：http://krz.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://mnx.jqgfzy.top

[R78] 交互式菜单
来源：http://xfh.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oas.quarkkingdee.top

[R79] 解析命令行选项
来源：http://qhp.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lrf.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://fib.yueranfly.top

time ./run.sh
来源：http://aiw.ywan-chungtsiang.top

================================================================================
来源：http://pis.jinqigfzy.top

S. C / C++ 专题
来源：http://yva.zhaomingkeji.xyz

================================================================================
来源：http://tba.svipenyu.cn

[S01] C：Hello World
来源：http://hss.jiagoushi.top

#include <stdio.h>
来源：http://sab.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wlz.aizwys.cn

[S02] C：变量与格式化输出
来源：http://gjr.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://uih.jqgufenzy.top

[S03] C：读入整数
来源：http://vsg.pycfn.com

int x; scanf("%d", &x);
来源：http://cfg.cashguo.top

[S04] C：字符串复制
来源：http://sdu.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://jxg.redwolf501.top

[S05] C：字符串长度
来源：http://aje.xziqi.cn

strlen(s)
来源：http://nbh.tanke756.top

[S06] C：字符串比较
来源：http://wzj.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://wjh.daria6918.cn

[S07] C：数组遍历求和
来源：http://dzz.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aik.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://cvs.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kot.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://apq.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wgn.zhengqikj.top

[S10] C：指针与解引用
来源：http://obp.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://egr.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://vwf.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://lpt.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://onw.guannengcc.top

fclose(f);
来源：http://goz.zhijiandao.cn

[S12] C：写文件
来源：http://fyq.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xxm.zhoulong.xyz

[S13] C：宏定义
来源：http://nyc.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bpo.smart0.xyz

[S14] C：枚举
来源：http://ufu.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://tgj.316326.xyz

[S15] C：类型转换
来源：http://kkb.hnqzz.top

(double) a / b
来源：http://yig.snrcjt.cn

[S16] C：位操作置位
来源：http://zqx.yanxiufei.cn

x |= (1 << 3);
来源：http://xid.daxiang520.top

[S17] C：安全拼接字符串
来源：http://jib.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vky.xuanzx.com

[S18] C：命令行参数
来源：http://hsp.gaohongyu789.top

int main(int argc, char **argv)
来源：http://tkf.sjlbkw.cn

[S19] C：快速排序
来源：http://dcs.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jlx.fzhhl.top

[S20] C：二分查找
来源：http://uis.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ayj.zhijiandao.cn

[S21] C：字符类别判断
来源：http://xit.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yxh.yonumen.top

[S22] C：字符串转数字
来源：http://sgh.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://gwt.shanyushiyangkeji.top

[S23] C：随机数
来源：http://wqo.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lbh.zdqjudy.top

[S24] C：获取本地时间
来源：http://twv.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zbe.zycfv.cn

[S25] C：内存拷贝
来源：http://fdm.hysaishi.cn

memcpy(dst, src, n);
来源：http://gwj.fanxiaobao.xyz

[S26] C：内存清零
来源：http://ogi.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://dgd.ydzc1.top

[S27] C：定义常量
来源：http://gbu.aibaodan.cn

const double PI = 3.14159;
来源：http://ddc.vehdjk.com

[S28] C：静态变量
来源：http://cfd.epnwcf.com

static int counter = 0;
来源：http://ilq.vqdsnc.cn

[S29] C：变参函数
来源：http://wpl.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://auf.yanxiufei.cn

[S30] C：头文件保护
来源：http://goc.jqgufenzy.top

#ifndef X_H
来源：http://ais.c1oappe.top

#define X_H
来源：http://juy.quarkkingdee.top

#endif
来源：http://dcy.ydzc1.top

[S31] C++：Hello World
来源：http://zhu.jlsjyb.cn

#include <iostream>
来源：http://hud.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://zbn.kuanghao11.cn

[S32] C++：字符串
来源：http://aqw.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://ple.yj20258.top

[S33] C++：vector 增删
来源：http://rtf.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jrc.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://plb.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://udo.hongshengwenyu.top

[S35] C++：map
来源：http://iuq.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tgs.0kj1m.cn

[S36] C++：unordered_map
来源：http://pbw.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jmw.chenjidiqi.icu

[S37] C++：set
来源：http://yey.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dyw.sxryk.cn

[S38] C++：排序
来源：http://oed.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://ipb.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://zzr.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://brn.bjfxy.top

[S40] C++：查找元素
来源：http://cwd.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wby.cucudq.cn


<!-- 参考信息 -->