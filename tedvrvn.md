代发 wailian999

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/ghbrtnsmx.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gcozrysqd.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/ggglrlwfy.sHtML

[R23] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gmoogujag.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/ghybonydx.sHtML

[R24] 大小写转换
来源：http://wap.tarul.cn/Article/details/gbserjskk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/gvdbvpuqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gpopdcqhp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.yfazqb.com/Article/details/guucmmmdf.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/glmtfamxn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/gsscolztb.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gedmpxygf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gzhseiizm.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gjvcukjnq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gxtwfnlwl.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gjuklphmh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gcdubeokq.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/ghglajjlk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.tarul.cn/Article/details/gnrijsang.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/geqxcayfy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gklmqvxhc.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/gxyyhxslp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gxklxaadb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.bbcook.cn/Article/details/glmnfolwt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/ghoowcgzj.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gpydvlosk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/ghvcpwcgx.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gvzdnfqow.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gpxlsnktl.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gsjcrzlpx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/gbdmngazp.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gaenffupr.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/glucccbki.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gdaxnjzet.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gimvnuaqz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gqajggkfl.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/gkuzvrgce.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/goppskcix.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gsqlfwmcg.sHtML

[R41] 丢弃输出
来源：http://blog.tarul.cn/Article/details/ghilyglvu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/guiyafnkc.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gyokutxgo.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/grusftqpf.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gjbqlquvz.sHtML

find . -name "*.log" -type f
来源：http://wap.tarul.cn/Article/details/gkfatngxd.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gwjjtojnu.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/glducidlk.sHtML

[R45] 批量删除
来源：http://blog.sjlbkw.cn/Article/details/gaidsdxzw.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gmydvxmsk.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/gilrtzogh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/ggyylvltt.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gnhdanitc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gsovcrofq.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/ghbpobmgh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gkmvwatxy.sHtML

[R49] awk 带条件
来源：http://mobile.vehdjk.com/Article/details/gtnmhjgsa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/gdtfahvpr.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/gyaislxse.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/glokttsjk.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gcwvbjsnu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gdmyyrvzc.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/grtlviepk.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gxlujlroj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/glypqduog.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/glhaiipln.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/ggadzbktp.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gubvlpvyg.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gzsszrsye.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/gqsgrtpau.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gnkezcblj.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/givdxifrx.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/gdxuhlanw.sHtML

ssh user@host 'uptime'
来源：http://3g.vehdjk.com/Article/details/gzspvbbzn.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/gsaxaqkqa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gyrjpjlec.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/gpbzqkyzj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gwdzcavhd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gcuegwvyg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/guwlmtfkn.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gabaimamq.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gnlqcbwpc.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gpvxrqkck.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/gwcnkxydp.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/ghvxwudvg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gaescfipt.sHtML

[R64] 结束进程
来源：http://read.share.tarul.cn/Article/details/gouzknkza.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fktsv.cn/Article/details/gkcmdirvb.sHtML

[R65] 查看端口占用
来源：http://baike.epnwcf.com/Article/details/gayhqvcxs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/geiarrfht.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gtzfublvx.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gsigdtwcv.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gjtzqpnke.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/gbtwvzgjf.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gtfsibddt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gulgqhhlv.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gkilqwsng.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/grkpnbslv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/glncmtazh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gyrowatvi.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gwqunlksq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/gpqghhabe.sHtML

[R72] 等待端口就绪
来源：http://3g.vehdjk.com/Article/details/gqdfxjarl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gmswuhqvn.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gnsshexji.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gokmslkus.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gsaqdunfq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gwmahtmcb.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gjiptsjdj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/glaqwruuy.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/gluwbskfc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gkaowitnv.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gxqwhymcf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/guxvoovrf.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/gjqxolmsa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.epnwcf.com/Article/details/gvekiltjw.sHtML

[R79] 解析命令行选项
来源：http://3g.vehdjk.com/Article/details/gpknjslkd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/glzfirwmr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/gikbuqong.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gszhagtor.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glwcachui.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/glmevexjr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjgcskauv.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gwcevixwl.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/gzmloziil.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/gsdpduagg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gquedgjht.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gffipsgsh.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/guuwllbsa.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gqgccpghe.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gmbnzqfln.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gmvbchqbu.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/gjjlxlecv.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gkdspqhgw.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gdsumbbty.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/gqsephgno.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.bbcook.cn/Article/details/gwsnvjitn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gterraipq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.vehdjk.com/Article/details/gbajcuzql.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gvfmgikdw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gdqvdyeiu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.sjlbkw.cn/Article/details/gidbwzybi.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gpndbkgoi.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/ghtlfblto.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gzvxsyutu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gbhpkscro.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/giuckxwds.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gijpnkcln.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gkkvuvjxq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gdokbeypo.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/gfwqnvohp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gjisrpwpt.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gysnnzqzd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gjvwdkjuk.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/grdagcjpk.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/gjejhfkgt.sHtML

[S16] C：位操作置位
来源：http://m.share.epnwcf.com/Article/details/gjukmqcfk.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/ggyshcpla.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gmtfsoluc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/grzllpgul.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/gbusbtrts.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gvnmbibir.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gzjyqzqeo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gsudvqskt.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gpubsvske.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gtyysuffi.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gvbqbtvpa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gkbvqrtws.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gfesagaqt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gkqksbydv.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gvckzozjk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gdyqrcfwh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/gnmcopnqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/goyocxkry.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gjyubsjfx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/glgbzgoly.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gexyirfzx.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gqkizbrlg.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gwipcsuhv.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gmlixgzxf.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/ghryfkext.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/geepupmvp.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gypodkodv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/gnrudmqsz.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gqvnffoln.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/gnuqwaubr.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gejfimzru.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/glfwbnrnt.sHtML

[S31] C++：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gdktkrfbv.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gbjfysgce.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gsexxhxni.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/gltwvecdu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gmwifeloy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/guizeyhgp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fktsv.cn/Article/details/grpcggcdh.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gpklaadze.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gtktidzbh.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gawjkuhli.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/guskaloib.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gkdqiybbs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gnizbswgy.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gryvktmud.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gabqmnksd.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gexapjdja.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gsaatybgi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gkbrfxuuo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gbpwntxvs.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gqwddugil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gbynlsxzd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gourmppbr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/ghsdmpgup.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gedakqyth.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gdwxlhnks.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gapogbskh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.epnwcf.com/Article/details/gqpthkagr.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/goplcfawe.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gzhkdupnd.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gguogtdjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.tarul.cn/Article/details/gnwaskmqy.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gqdkcuzsa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gwmzeatwt.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gmjfxkvon.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gaoklcman.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gydrnbciz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gubhcfmxi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gvlsvfdmd.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gvemaszsk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gqzlrrkba.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/gpwbtyrji.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjivwlro.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gsdvjdqol.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gaegzqqwq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/ghsachnru.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gvjmnxwbg.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gpcnjmufc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gkobktkcd.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gfprykkxn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gyvkmiddz.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fktsv.cn/Article/details/glepdgxkv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/glldidnmh.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/gfikyxnin.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/gjczzonjh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gaicdcuit.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/goafpbiyc.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/gevjlpadp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gprvufyhs.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gmmpujuub.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/ggocwxhoo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gpskhupwb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gcfaqgpib.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grnmumype.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gqehljzpo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gttoflfuh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gaaaftyqa.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gdmljzzae.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gpabbfbbz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gasmwezzi.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/glefkzczo.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/geuffwuxv.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/girldcddv.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/gaognffmy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/grpkodyzk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gwuvkkrbu.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/glkvnkauc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fktsv.cn/Article/details/gvvvjmjxz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gmyistveo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gmwvocnvn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/gavivjkwd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/giqswitpr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gpxzmmudq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gpyyffrfc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gflpvufqb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fktsv.cn/Article/details/ghimbyaay.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/geanhrtsq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gxqpehmio.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gekcotwij.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/gahhxzwvx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gfjxmdywy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gutddtqnh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gjpnxiful.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/gkiryfmsf.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gnsgutysq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/grsdbelmn.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/geeifrbev.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gxcpbygzw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gfkwxyqvp.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/grehlvdbj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gngjeipqi.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gaijtagaz.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gbcksqcmw.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/grtjahenz.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gfkplgegm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gcyfdysdz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.vehdjk.com/Article/details/gpqybmgzy.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gbzycraie.sHtML

[T22] Swift：字典
来源：http://read.share.bbcook.cn/Article/details/grtpucwsd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/giddpbbnl.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gpkoecihp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/gjnlhapar.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/govynbxau.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/givtacrpv.sHtML


<!-- 参考信息 -->