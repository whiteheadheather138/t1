代发 wailian999

SHOW INDEX FROM users;
来源：http://dtc.cucudq.cn

[Q73] 查看表状态
来源：http://mjs.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://oey.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://hue.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ino.daria6918.cn

[Q75] 日期格式化
来源：http://bpi.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sxh.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uzz.epnwcf.com

[Q76] 按天统计
来源：http://dsn.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qqk.meibo888.top

[Q77] 时间加减
来源：http://vwm.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://akb.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://qjj.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vsu.tanke756.top

[Q79] 字符串拼接
来源：http://jrx.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ixa.daxiang520.top

[Q80] 字符串截取
来源：http://jma.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hgy.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://glt.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://amn.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://mcp.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ubr.cashguo.top

[Q83] 大小写转换
来源：http://wbd.cqqwz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rfb.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://zzb.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://exv.hfpthk.cn

[Q85] 数值取整
来源：http://tlb.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xhr.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://rjc.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rzz.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://ytm.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://srf.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://fbh.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://has.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pxd.yueranfly.top

[Q89] 判断表是否存在
来源：http://qps.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uku.vehdjk.com

[Q90] 生成序号列
来源：http://mch.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ysu.yj202588.top

================================================================================
来源：http://ygx.316326.xyz

R. Bash 专题
来源：http://wzk.yfazqb.com

================================================================================
来源：http://atp.dashuyun.cn

[R01] shebang 与严格模式
来源：http://vio.sysykeji.top

#!/usr/bin/env bash
来源：http://hsm.xinyue.icu

set -euo pipefail
来源：http://mfh.yj20258888.top

[R02] 变量赋值与使用
来源：http://ivy.cheryme.top

name="Tom"; echo "$name"
来源：http://kjb.tian-w.cn

[R03] 只读变量
来源：http://jky.birdmap.top

readonly PI=3.14
来源：http://ist.shuidangran.top

[R04] 位置参数
来源：http://nvg.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ymi.shuidangran.top

[R05] 参数默认值
来源：http://cbm.sjlbkw.cn

name="${1:-default}"
来源：http://ofc.bjfxy.top

[R06] 判断命令是否存在
来源：http://kbj.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vaw.jinqigfzy.top

[R07] if 判断文件
来源：http://yaf.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qzr.snrcjt.cn

[R08] 数值比较
来源：http://hvh.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://sjn.vqdsnc.cn

[R09] 字符串比较
来源：http://xmr.andypj.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nrd.cashguo.top

[R10] 正则匹配
来源：http://syw.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xjm.pycfn.com

[R11] case 多分支
来源：http://ngw.cqqwz.cn

case "$1" in
来源：http://jzw.shangyingyoupin.top

start) echo "启动" ;;
来源：http://pvh.zdbjq.cn

stop)  echo "停止" ;;
来源：http://cwe.mhx1999.top

*)     echo "未知命令" ;;
来源：http://moj.ctjpmb.com

esac
来源：http://pzk.sxryk.cn

[R12] for 遍历文件
来源：http://pqw.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://ush.52xcode.cn

[R13] for 计数循环
来源：http://nlv.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://hzp.zycfv.cn

[R14] C 风格 for
来源：http://etq.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ofx.mhx1999.top

[R15] while 逐行读文件
来源：http://adp.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://csp.fktsv.cn

[R16] until 等待条件
来源：http://tzh.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zzj.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://xvs.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://uqe.zhaomingkeji.xyz

[R18] 遍历数组
来源：http://fev.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jku.yfazqb.com

[R19] 数组长度
来源：http://fru.gaohongyu789.top

echo "${#arr[@]}"
来源：http://vva.pycfn.com

[R20] 关联数组（字典）
来源：http://cpn.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jpl.ivvv.top

[R21] 字符串长度
来源：http://cln.chenjidiqi.icu

echo "${#s}"
来源：http://lpl.hnxiangtu.top

[R22] 截取子串
来源：http://daj.xuetiantiany.cn

echo "${s:0:5}"
来源：http://rij.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://ucf.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://whg.tian-w.cn

[R24] 大小写转换
来源：http://ymi.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://bbh.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://sls.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zky.ydzc1.top

[R26] 命令替换
来源：http://nkb.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://jfy.hnqzz.top

[R27] 算术展开
来源：http://who.fzhhl.top

echo $((1 + 2 * 3))
来源：http://kdu.gzhubu.top

[R28] 浮点运算
来源：http://tpx.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://bdi.hywenlv.cn

[R29] 定义函数
来源：http://xpn.fengsongda.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vzv.sweek.top

[R30] 函数返回状态码
来源：http://obf.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://bty.chenlongwang.top

[R31] 局部变量
来源：http://ids.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://dmz.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://fwg.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ife.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://omy.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://con.hywenlv.cn

[R34] 退出时清理
来源：http://uym.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://xar.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://oai.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sgf.haohaochexian.top

[R36] 并发执行多个任务
来源：http://erk.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tvh.jiagoushi.top

[R37] 把输出赋给变量
来源：http://bri.xylfe.cn

files=$(ls -1)
来源：http://qiu.bbcook.cn

[R38] 管道串联
来源：http://coy.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://iks.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://ujw.xuanzx.com

cmd > out.log 2>&1
来源：http://hqu.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://suc.cqqwz.cn

echo "log" >> out.log
来源：http://rcf.dashuyun.cn

[R41] 丢弃输出
来源：http://hit.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://lqm.svipenyu.cn

[R42] 输入重定向
来源：http://nmh.snrcjt.cn

wc -l < a.txt
来源：http://ktj.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://uqt.mhx1999.top

find . -name "*.log" -type f
来源：http://ilm.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://ept.daxiang520.top

find . -mtime -7 -type f
来源：http://fnj.hfpthk.cn

[R45] 批量删除
来源：http://dzj.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://fsb.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://dhr.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rfc.jlsjyb.cn

[R47] sed 单行替换
来源：http://wej.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://alx.fzhhl.top

[R48] awk 取指定列
来源：http://pgw.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://yzf.andypj.xyz

[R49] awk 带条件
来源：http://nte.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tsy.yuxming.cn

[R50] awk 求和
来源：http://nug.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://dqy.yongpay.top

[R51] 排序去重取前几
来源：http://qhw.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hws.cucudq.cn

[R52] 统计行数
来源：http://ttd.fktsv.cn

wc -l a.txt
来源：http://kew.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://cmk.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dde.jlsjyb.cn

[R54] 比较两个文件
来源：http://sqo.cucudq.cn

diff a.txt b.txt
来源：http://ibf.xuanzx.com

[R55] 压缩与解压
来源：http://xoe.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zxn.uphjek.com

[R56] 远程拷贝
来源：http://oeu.nanxuanxn.top

scp file user@host:/path/
来源：http://lco.kuanghao11.cn

[R57] 远程执行命令
来源：http://vyy.9152youxi.cn

ssh user@host 'uptime'
来源：http://uxe.gzhubu.top

[R58] 下载文件
来源：http://hvz.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wrj.ehwqpu.com

[R59] 发 POST JSON
来源：http://enw.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uoq.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://mta.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pyy.aizwys.cn

[R61] 磁盘占用
来源：http://xmw.bbcook.cn

df -h;  du -sh *
来源：http://gir.xinyue.icu

[R62] 找最占空间的文件
来源：http://bva.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://mso.redwolf501.top

[R63] 内存与进程
来源：http://shy.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://ydq.xinyue.icu

[R64] 结束进程
来源：http://ecd.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://qdu.quarkkingdee.top

[R65] 查看端口占用
来源：http://gcm.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mig.zhoulong.xyz

[R66] 定时任务
来源：http://yvq.daria6918.cn

crontab -e;  crontab -l
来源：http://vlu.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://pwm.jqgufenzy.top

openssl rand -hex 16
来源：http://xsm.hfpthk.cn

[R68] 计算文件校验值
来源：http://nck.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bmn.gogol.net.cn

[R69] 生成随机密码
来源：http://smy.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://prh.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://the.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://zrq.kuanghao11.cn

[R71] 日期格式化
来源：http://fzx.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ene.jinqigfzy.top

[R72] 等待端口就绪
来源：http://hry.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://szq.gzhubu.top

[R73] 分割大日志
来源：http://jot.ydzc1.top

split -l 1000 big.log part_
来源：http://ujs.yvedp.cn

[R74] 批量重命名
来源：http://adz.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vnl.shangyingyoupin.top

[R75] 导出环境变量
来源：http://srv.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://nnh.gaohongyu789.top

[R76] 使用临时文件
来源：http://wdn.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zig.zhijiandao.cn

[R77] 读取用户输入
来源：http://dxj.sysykeji.top

read -rp "请输入: " ans
来源：http://xhj.smart0.xyz

[R78] 交互式菜单
来源：http://cts.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://grn.cqqwz.cn

[R79] 解析命令行选项
来源：http://lql.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qrn.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://aho.fengsongda.top

time ./run.sh
来源：http://eug.birdmap.top

================================================================================
来源：http://uem.ehwqpu.com

S. C / C++ 专题
来源：http://isj.ehwqpu.com

================================================================================
来源：http://jfo.fehbvm.com

[S01] C：Hello World
来源：http://pok.sufxvd.cn

#include <stdio.h>
来源：http://rbx.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rlw.gzhubu.top

[S02] C：变量与格式化输出
来源：http://mlt.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://xba.hysaishi.cn

[S03] C：读入整数
来源：http://yul.birdmap.top

int x; scanf("%d", &x);
来源：http://fvk.yvedp.cn

[S04] C：字符串复制
来源：http://ljk.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qoo.sxryk.cn

[S05] C：字符串长度
来源：http://kvh.yj20258.top

strlen(s)
来源：http://iwp.9152youxi.cn

[S06] C：字符串比较
来源：http://vym.yonumen.top

strcmp(a, b) == 0
来源：http://yrw.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://xrr.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yyh.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://iza.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vky.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://abz.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://csr.0kj1m.cn

[S10] C：指针与解引用
来源：http://qlr.bjfxy.top

int *p = &a;  *p = 5;
来源：http://djg.haohaochexian.top

[S11] C：逐行读文件
来源：http://ykl.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://vvt.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mhh.yj202588.top

fclose(f);
来源：http://uzy.shuidangran.top

[S12] C：写文件
来源：http://pke.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qbf.tanke756.top

[S13] C：宏定义
来源：http://ivd.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lbh.gogol.net.cn

[S14] C：枚举
来源：http://luw.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://lmt.ctjpmb.com

[S15] C：类型转换
来源：http://wjv.snrcjt.cn

(double) a / b
来源：http://ndx.havefunace.top

[S16] C：位操作置位
来源：http://ftz.chenlongwang.top

x |= (1 << 3);
来源：http://wxh.sweek.top

[S17] C：安全拼接字符串
来源：http://frg.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://khb.nanxuanxn.top

[S18] C：命令行参数
来源：http://ibo.hnxiangtu.top

int main(int argc, char **argv)
来源：http://sgj.ydjk.org.cn

[S19] C：快速排序
来源：http://htl.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bim.cheryme.top

[S20] C：二分查找
来源：http://qdn.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oef.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://wku.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rty.sxryk.cn

[S22] C：字符串转数字
来源：http://vti.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wob.tianlin.xyz

[S23] C：随机数
来源：http://wsg.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lsa.shzxlz.cn

[S24] C：获取本地时间
来源：http://fqu.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tqp.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://umk.fktsv.cn

memcpy(dst, src, n);
来源：http://mif.yj202588.top

[S26] C：内存清零
来源：http://jtx.316326.xyz

memset(a, 0, sizeof a);
来源：http://wbt.hysaishi.cn

[S27] C：定义常量
来源：http://oie.aizwys.cn

const double PI = 3.14159;
来源：http://hkt.sufxvd.cn

[S28] C：静态变量
来源：http://ovp.ydzc1.top

static int counter = 0;
来源：http://ouu.yueranfly.top

[S29] C：变参函数
来源：http://abc.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ndt.zhixingplan.top

[S30] C：头文件保护
来源：http://esr.jianghu66.top

#ifndef X_H
来源：http://ale.cashguo.top

#define X_H
来源：http://bee.redwolf501.top

#endif
来源：http://iex.zdbjq.cn

[S31] C++：Hello World
来源：http://xdo.wangshuangyany.cn

#include <iostream>
来源：http://xvw.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://iuq.yuxming.cn

[S32] C++：字符串
来源：http://xby.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://oex.xziqi.cn

[S33] C++：vector 增删
来源：http://lly.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lgl.haohaochexian.top

[S34] C++：遍历 vector
来源：http://kcx.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://kvf.sysykeji.top

[S35] C++：map
来源：http://ucm.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mni.gotoacloud.top

[S36] C++：unordered_map
来源：http://wan.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tws.xylfe.cn

[S37] C++：set
来源：http://alv.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jry.andypj.xyz

[S38] C++：排序
来源：http://zln.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://gko.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://jdp.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://usj.hcnkem.com

[S40] C++：查找元素
来源：http://fbl.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nbk.pycfn.com

[S41] C++：类与构造函数
来源：http://wjn.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oen.yj20258888.top

[S42] C++：继承与虚函数
来源：http://wii.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://aqn.svipenyu.cn


<!-- 参考信息 -->