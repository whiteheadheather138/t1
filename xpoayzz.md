代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gibrzfglg.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gevcbyjxp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gdkkjhtuv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gbwjhujsr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gfkunkonq.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gmnvhrtfx.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gmsubesrv.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gsplcfvrr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gvdyfdxze.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gwwdzikrl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gylwxsnnz.sHtML

[R29] 定义函数
来源：http://m.share.tarul.cn/Article/details/gauecujvg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/golibhhfc.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/giizsiwck.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/ghvkdpdyv.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/grxnunxin.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/gbcgsapop.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gestwojlj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gzivpnrml.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gtddpqlbv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gdibwdijd.sHtML

[R34] 退出时清理
来源：http://mobile.bbcook.cn/Article/details/gtqufowgs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gfdsbimhd.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/grpsewrix.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gulhuxtta.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/givfezlzq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.epnwcf.com/Article/details/gjobtvwzt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/gjybbhyqi.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gsbslutvo.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gweapjzbg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/geflbjsxw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnczsihu.sHtML

cmd > out.log 2>&1
来源：http://baike.epnwcf.com/Article/details/gcfsjbnmy.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gbkhnmlhp.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/grenlsalw.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/ggmxuhltz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/gaixlolor.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/gurojhnjb.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gkqcnlctu.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/gygptoluw.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gdcybvnph.sHtML

[R44] 按修改时间查找
来源：http://3g.sjlbkw.cn/Article/details/gazkjucfi.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/gfpcyijsy.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gthqksran.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gvpjhzozw.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gonhtsamk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gyibscuxp.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gcyszunmn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gvdenzyph.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gnmfocyiy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gulwpqybu.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gvjpaowln.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/grynwwgbz.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/ghneajwjl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gztdggauq.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gyzfkxlyr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gjkllakis.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gitomxymu.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gxbvniirp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/gjuewslaw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/gkrkdwirm.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gkujgrudg.sHtML

diff a.txt b.txt
来源：http://www.m.share.yfazqb.com/Article/details/gulknodry.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gljtnbuao.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gmyepyiul.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gnuxtazkf.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/gfhltdran.sHtML

[R57] 远程执行命令
来源：http://www.m.share.epnwcf.com/Article/details/gfscnpmzt.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gqqjezhpi.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/goymhipaf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/gzbeiunzf.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/gnytgjemw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gsdawnvbw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gnpnmprdu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/goqcwinzl.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gmohvokom.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gwbpggadl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.yfazqb.com/Article/details/gekivuvic.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/gpabclhrj.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gspoppkii.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/gluaubxip.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gmzmqnggy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gmgmlmeme.sHtML

[R65] 查看端口占用
来源：http://blog.epnwcf.com/Article/details/gtwohwbux.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gftvbfohr.sHtML

[R66] 定时任务
来源：http://www.blog.fktsv.cn/Article/details/gpojyovsp.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gthfnnvfp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gwmsexmjc.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gytzgvndo.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gmjbdmqav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gyqhpuokx.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/giyueydwa.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gbcdajznc.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/ghzlzrksw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gdxirpxmk.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gtfgkhmvn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/glmwhcrao.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gabqxrter.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gikjeffvb.sHtML

[R73] 分割大日志
来源：http://baike.tarul.cn/Article/details/gcaxuyofx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/gkdumelse.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/goivphroi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/ghetynibg.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gzlsoxxoc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gcekzdgin.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gvciiyezd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gkpxhmjbr.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gckwivblr.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gtyrlpqsk.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gwafvkiid.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/goyjdeodm.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gtdncrons.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gysdzaqtu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gmxfwtqux.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gyqukooak.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/giqspccbi.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/ghtqjlukp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gaxdihjbs.sHtML

[S01] C：Hello World
来源：http://mobile.epnwcf.com/Article/details/geyujnzzw.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gmhvsyssc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/grazzpwrv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/glqmdhnzn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gwidodtrj.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gtjcbnvcb.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gdqwgbqen.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/grrfskrrl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gdxlzfedy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gqvzfkzye.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gwlybtbxv.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gjjkyxofk.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gzwqgtatk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.epnwcf.com/Article/details/gnvmsqimw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gxzbmcndw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gcplguvoz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/grxetnpur.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gatyuujqi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/guwiauovi.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gbxgzilpn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/ginkoohab.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gfkxsytnx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gnznoaevn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gpmyfqxrp.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gmqfszips.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gdhcbppxy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gdeinison.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/guhlxveuk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gkeuowelg.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gkvvwndlw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.vehdjk.com/Article/details/gdkxxcymi.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gyggplcrf.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/gkfydlkkh.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gpojkwrtr.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gtjdfnumw.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gpdsmizcb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gpecsjteb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/grkhxiigj.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gvxiudpfu.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gzgodivpl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gomdvegph.sHtML

[S20] C：二分查找
来源：http://mobile.bbcook.cn/Article/details/ggvlpquyo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/ghhsbdfgk.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gbddhhpbd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/gztzevlty.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gfaankygv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gvesstdlk.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/gukicdfif.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gbdhmvnry.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/ggqhkokdd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gwdcklsje.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gxtkcfygi.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gdhzbpxxz.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gykqcvobl.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gczhhljzv.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/gcrqggmjo.sHtML

const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gtwztfaru.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gxsjeyugq.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/gtgpghary.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gmgfrwcaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gqvbwhvwq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.vehdjk.com/Article/details/gfwxckbhx.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/geczaoftl.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gddxqhweg.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/ghagctmha.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gboxczjqs.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gsovvdiun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/ghxdvtqgg.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/guoryxvsu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gmruplrch.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gflgwnnnq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gxgyziahr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/gjkivjvsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.epnwcf.com/Article/details/glhvnxdkx.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/gnxdkbrdu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gwuvjkyna.sHtML

[S36] C++：unordered_map
来源：http://m.share.tarul.cn/Article/details/gfljmjclj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/goyfqxkuo.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gyqcwnzde.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gqxdcnbgv.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gvxyaijsw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/ghloehvqx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/gbddtmedr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/glnwsgfho.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/gamqxqkeo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gvvpenysd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/gwqxqfgxx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/gzfsovjvn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gieqchmxm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gzfodeoma.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/gyckahxll.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gafixjkhr.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/guwjpassl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfqnyyuzx.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gzmymfkhv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gzncqrlpx.sHtML

[S46] C++：函数模板
来源：http://m.share.epnwcf.com/Article/details/gidioxcew.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/gcliwnqma.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.yfazqb.com/Article/details/gdpfddemd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gvuydmtui.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/guutbwfof.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gqrxxyigc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/grfkmizfp.sHtML

[S49] C++：写文件
来源：http://3g.fktsv.cn/Article/details/gbopdxgsv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/ghzxadmlz.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gtisepazj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gelbasast.sHtML

[S51] C++：显式类型转换
来源：http://wap.sjlbkw.cn/Article/details/ghfferwdy.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/ghxdqaqek.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gyrbpoqqv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/gfjgrswaq.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gtlatpmgx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gusbndoiy.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gvaqgrxcp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/grkmnqvic.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gpnuwgubq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gqktsvcoc.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gyijyglga.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gjjndqbzu.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gfpimsepp.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/gbcnrcqak.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gpxexcimp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.epnwcf.com/Article/details/gtlffvlex.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gmeykloqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/ginipwejn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gtbhvuicl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.sjlbkw.cn/Article/details/grmpqkrlm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxebhhizi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/glqkahmin.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzduqeucb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gxzgvayws.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gmqjeviqr.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/grbgoxnhv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gtkzttxyk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gqpvmvxlu.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gmcajwxlk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.tarul.cn/Article/details/gkhjsjdev.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gpvijsjeu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/grrnwaxsr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gmzjayrfe.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gywrxhxax.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gqhdggobb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gfupuzjrv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gknrucyde.sHtML

[T08] Kotlin：数据类
来源：http://blog.epnwcf.com/Article/details/gndjhtpxf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gsvfogmlj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gnipwcmkw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/grkbdpcoo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gaygivcxm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/gixcnjawf.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gvcylauid.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/gsnsshgag.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gbrbqzmpn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/geekvgliv.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gjgadtmrf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/gfislkfmd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ggghwdhpj.sHtML

for (i in 1..10) println(i)
来源：http://wap.fktsv.cn/Article/details/gmzpmdpjk.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gbwyjhhiq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gaisivmzc.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gfphharmp.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gvgqvlich.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/gcwuuzycl.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gsvfkwplh.sHtML

[T18] Swift：字符串插值
来源：http://baike.tarul.cn/Article/details/gzejivmyo.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gxxwjndzx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gcgwkykeb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/guljpzpkk.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gyybkaacm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gxnruvfla.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gebbvvnhv.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gbaywjriq.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/gdujkzkxe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/geqazyxds.sHtML

[T23] Swift：函数
来源：http://www.m.share.bbcook.cn/Article/details/gkwdwkaih.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gfnbkvnvh.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/gfhqzpnhe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gamsbrsjb.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gcbolosxt.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/glwsuzyuk.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gogbiomuv.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gjuczudqd.sHtML


<!-- 参考信息 -->