代发 wailian999

echo "${#arr[@]}"
来源：http://m.share.vehdjk.com/Article/details/gmbuariqa.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gkpdhvdvb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gvnbvvvcy.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/guwkpekda.sHtML

echo "${#s}"
来源：http://m.share.yfazqb.com/Article/details/gccdrlazn.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gjbnzojym.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/gbzuqntcn.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gbtfwbffe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gocuzaurn.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gavxwtdma.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/gqqsbqtqc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/gmpicquop.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gfkmvopdf.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/goymubirn.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.sjlbkw.cn/Article/details/gteehlrmm.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gnlujiocl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gozhdvymd.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/giheanmqg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gkkjdeokm.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gqzcbfuzp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/gcrqgiboc.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gpycsjmot.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/ghsqbbzxp.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gbuqcglzs.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gvscesqba.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gcrdtnnfq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/geyfvragv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/gaqynmaxx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.epnwcf.com/Article/details/gizgjmhmu.sHtML

[R34] 退出时清理
来源：http://mobile.bbcook.cn/Article/details/gjyomckvu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gydbtfpaz.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gliduuyjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/ggdsblham.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/gurteqgvs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gvlqmdwvg.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gwxjaqizg.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/guncmjcnr.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gsxkowvol.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/geaphopyq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.yfazqb.com/Article/details/gcfrmofej.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gysaftydn.sHtML

[R40] 追加写日志
来源：http://wap.yfazqb.com/Article/details/ggigkgfel.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/guoyvrbre.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/glkypzxto.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gmpajnsfg.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gpaptdywh.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/gietleqav.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gmiypgqpz.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gyguchxpm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gspivsglb.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/gggphaqie.sHtML

[R45] 批量删除
来源：http://read.share.bbcook.cn/Article/details/glcxxnbba.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/gwjwcicqy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gfaeloafx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fktsv.cn/Article/details/gfnmmpamw.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gczhnjues.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.tarul.cn/Article/details/gjjwijgwy.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gamqdrwax.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gklhwahiw.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/grhgreobh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/ggirhldeo.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/gtckhovoi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/gfdwmybts.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gxzxnneba.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/gmegwxwja.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/ggeneyagg.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/gsazmujsi.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gbjuqpgwc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.vehdjk.com/Article/details/ggliznnak.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gkgxmtydm.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gbxudejvg.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/gidinyhlq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gzshinphk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gxvyrtueb.sHtML

scp file user@host:/path/
来源：http://mobile.tarul.cn/Article/details/gtpqfxpnz.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/gfeajszxu.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gksemkjps.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/grozgnkaq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gqjhcetcj.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/ghstaghgf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gyitqzrpw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gyeqbbcmd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gdygtpwkr.sHtML

[R61] 磁盘占用
来源：http://mobile.tarul.cn/Article/details/gbkerxluf.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gdlqzstll.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/garpgyzgt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/ghlzrctqj.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/ggcseugmq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fktsv.cn/Article/details/gdiquwoyl.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gxxbwmqlb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gpxhexnbw.sHtML

[R65] 查看端口占用
来源：http://blog.tarul.cn/Article/details/gtlqjllgy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gvioyqwtz.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gwoklqbkm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/grwpyqghh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.tarul.cn/Article/details/gmbseindw.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gpsoydbad.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gvoytzjok.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gegkabati.sHtML

[R69] 生成随机密码
来源：http://www.blog.sjlbkw.cn/Article/details/gfyjnrffv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gzgnrvsdr.sHtML

[R70] 时间戳与互转
来源：http://mobile.epnwcf.com/Article/details/gcjyfoqra.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/glkskqvuo.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gcqnpfhxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gyujvpwvw.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gqyyqyboe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gyksdasbb.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/grblikyue.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gvuftkmim.sHtML

[R74] 批量重命名
来源：http://wap.epnwcf.com/Article/details/ghzavctpe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gbaachcfc.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gpdowxdwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gplforwsj.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gvmxwhzmg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/glvtcekgj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwunalqj.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gutdyojqb.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/guawsdils.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gopyfnyll.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gvqslkeuk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/gjflnsfem.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/grcqcfhjl.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/grfqadggo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvsendebs.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gzpsywtbn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsnqukjwq.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gpznfwrng.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/gyfkiyodg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gruliorpc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gwqihpjzw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gzllnniit.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/gndzflhjr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/ggifnuobl.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gelnkozsi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gbzpzqmbk.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gdlussbyp.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gycfciqyr.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gqdjkapem.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gzqetnkeb.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.bbcook.cn/Article/details/gwgraiwmt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gxyvsslos.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/glcpotsse.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gffiafhch.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gzwkrxzrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gfvurdulk.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/giqsiyvjc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gelogcnbm.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gaymuyrmc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gqrxwozqw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gohscxhqu.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/geuohcdlf.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gxlntuimf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gidamgimd.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gxqwvxshy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gabxrulnk.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gtjnxlkeq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gvlwepnup.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gporxdbaw.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gpcqvgtuz.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gbkdqitmo.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/gwrrbuewo.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gkebfpapr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.epnwcf.com/Article/details/ghctbalut.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gycdgyzka.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvipykyl.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gdbdpiihu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/ggcwmlsry.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gefzzcttg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/grmfohvdx.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gzegrqpqk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gqujudzba.sHtML

[S22] C：字符串转数字
来源：http://www.share.tarul.cn/Article/details/gpkmxsgxs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gtiprrqgb.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gwxohywxu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/ghmnzdaln.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gxdprauqy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/gvjklhrrt.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gwxpmdboe.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/gfuzrbokd.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/gvgejjjtz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gaxrdugrg.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gdbmougjn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gmmzcdzmp.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gjaqornhx.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gkuwacfzm.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gckqbwphy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gmrsawkmg.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gslvoogyz.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gicmxjyrf.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gqafjkrsf.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gzyflckgv.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/gegkrrpzr.sHtML

#include <iostream>
来源：http://blog.vehdjk.com/Article/details/gukygrctc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/gaslrcdpd.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfzlbeyrc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/gceljjygo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gltkdkrdv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gaiaijmac.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/giomjxizl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.sjlbkw.cn/Article/details/gackpfvrs.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/gvwarsfbx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gsllyzmck.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gpeowvfaf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/ghikqldih.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gxropiale.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gwcywvgrs.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gwibqxlho.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.vehdjk.com/Article/details/gaehjdetr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gfooqdczr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gunijmtfk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/giusdtbzp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gdmpuqhdx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gdbkuscjj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gkkitehhy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gauasgxxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gvojbusjo.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gvtxaojmv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gflzarroe.sHtML

[S44] C++：引用传参
来源：http://blog.tarul.cn/Article/details/ganbjdpvl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gmcdanorg.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gsnzvvrdr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gbwlnqnrd.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/giesqpccv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/goimuctut.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gixtenjcg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gzcvbvgkc.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gnclhnicw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gwnsourli.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gwvbfhjno.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gcmvuafrm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/grquxpdww.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/gmvrhnbqg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/ghxvgaakb.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gihyvnofv.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gwmcdmhyf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gzhvtuhpz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fktsv.cn/Article/details/gmdapelkb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gleyktlaf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/gtdonbrww.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gsfivvtsv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gdlbpdhps.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/gfljsjydm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gtwkkesop.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/ggbcruobs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/guumbcmhp.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/gqqtteeev.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/ghjhrtyov.sHtML

[S58] C++：命名空间
来源：http://blog.yfazqb.com/Article/details/gazxgutaw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gbyyztolw.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gcezszukh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.vehdjk.com/Article/details/genbxhdau.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gyogsbvxi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/gyafungqq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gedlfgteb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gieccqmqk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkgnmrjaa.sHtML

[T01] Kotlin：Hello World
来源：http://wap.bbcook.cn/Article/details/gkwzrwyeb.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/ggmqifgqd.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/ghoyozsvk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gtwvenyds.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/ggzattndc.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gsxnvkxef.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gunzeftiw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/gksnxhpmu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gtbewwzjz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gxvncxvdm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gtoiwnfbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gesbmvbrm.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gbwltjihi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gitqrdwrz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gntpmvmei.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/ggxenajvu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gglmgjikk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/gnhxngxfi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gymuhwidl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/ggxrgdlpl.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gofqdgulc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gtkqrpjhs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gdqdgijkn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gnorcipmy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/gprnevogu.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gzbvwnhrl.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gldsruemd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gwanvzozo.sHtML

[T15] Kotlin：接口
来源：http://read.share.epnwcf.com/Article/details/ghkmdgxiw.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gkfceanao.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gpjnvvofe.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gxfpsmyfr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gwybbntwh.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gckjkryqo.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gipfoaimn.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/gzsstjofm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.epnwcf.com/Article/details/gfwfiqtbh.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gzcytxsgs.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/galefgncr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gmwqcyvgc.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/gypeqkbfb.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gzxloagjf.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gfpaohzmb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/gafguyqxk.sHtML


<!-- 参考信息 -->