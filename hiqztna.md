代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gpdwhnwoj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.bbcook.cn/Article/details/gxwkpzshe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gpfgvjnzw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gnikezuov.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/gdgwlitby.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/gntdskmep.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/ggjxaoitb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/geqzyvhec.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gzkbcfxye.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/gvsngmhhx.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/glxnfuzrq.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gnzdkqalt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/ggnksgaip.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/gzgumgcqw.sHtML

wc -l < a.txt
来源：http://mobile.bbcook.cn/Article/details/gvxycfooa.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gqimhazke.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/glqyviyds.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/gcwgkdhju.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/gcoaetlbn.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gtgpdktdj.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gjxtcmybo.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/gqnvbbpya.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gelwjcxun.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gjttusxnc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gyhkcoawn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gyuahqwuo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gesboldhf.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gdojljexh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gvkcwcdlx.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gtphuxuxl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/guiikspak.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/gohqvmsll.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gelzdisco.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gvnxkxxtd.sHtML

wc -l a.txt
来源：http://3g.yfazqb.com/Article/details/gttjvudhs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gmabwjsyq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfylzked.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/grlngypzd.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gnmgkguoc.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/gweovnwlr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/gcmhmrezs.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gvshlrohw.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gwlnypxzb.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/govqikwps.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gozwdugnm.sHtML

[R58] 下载文件
来源：http://m.share.fktsv.cn/Article/details/gpnxrllpz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gtvvjtjei.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/gakqnzuqq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gjwtkvjtj.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gqwfwtzcg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/gcijbreho.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/galxexbsc.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gbhvanmzk.sHtML

[R62] 找最占空间的文件
来源：http://blog.fktsv.cn/Article/details/gyfivizic.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gytyvywam.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/giukeplrm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/grtxknjoe.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gjullooze.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/ggyhtwygq.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/gisgaaayf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/ggiizidgw.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/grkjptpuy.sHtML

crontab -e;  crontab -l
来源：http://www.share.tarul.cn/Article/details/glxpjzrtw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/gibxjxnyt.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gyqgbwynm.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gjygmqvjv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/gkqesiutu.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/gkjjxiwfr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/ggwsffpql.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/goneqfbuq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gpsntrbfw.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gxybbiqli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gkbmytmdy.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gzmwmhktw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gaszhmofu.sHtML

[R73] 分割大日志
来源：http://www.m.share.tarul.cn/Article/details/glonwyzoh.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gcqsisccm.sHtML

[R74] 批量重命名
来源：http://www.share.epnwcf.com/Article/details/gdtrxxvuo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gabjobswt.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gdxdaieua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gzzatspyc.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gbnrmqahy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gijxbwaof.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gwvpyivtp.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gvjyfrqwm.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/glbdbizxm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gldbauhik.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gyjbjczbg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fktsv.cn/Article/details/gfqltimny.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.tarul.cn/Article/details/gnqjbouyv.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gkxmbdpqr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnmjzfone.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/ghllzfqir.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grlqnimxv.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/glkiqdbrb.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/gnanqwcwf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.tarul.cn/Article/details/gzjvryhcz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/ghzrmszdg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gqzjnaqqj.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gujtycbap.sHtML

int x; scanf("%d", &x);
来源：http://read.share.tarul.cn/Article/details/gvzyvelai.sHtML

[S04] C：字符串复制
来源：http://3g.epnwcf.com/Article/details/gdaxvabmi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/giqgwaciq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gawfhfkfb.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/ggnzmeews.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gvexlshzk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gljpzlvyj.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/gsfapxvar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gvtjqjlme.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fktsv.cn/Article/details/gbjytuzxd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/ghhfvjrws.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gzbkflsio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gksacvpdr.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/grlrakyrg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/ghuatmqzb.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/goyruurrr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/gqaieqdvz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/giaxjgqya.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gagckaytk.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/gfyyfzrxo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gjanbirqi.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gluvwpxsu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gmhzcxgig.sHtML

[S14] C：枚举
来源：http://read.share.yfazqb.com/Article/details/gdmcbrwoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.tarul.cn/Article/details/geybhbhkq.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/ghrbjzprs.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gzhqkxknz.sHtML

[S16] C：位操作置位
来源：http://baike.tarul.cn/Article/details/gcxbpwhad.sHtML

x |= (1 << 3);
来源：http://blog.yfazqb.com/Article/details/gzxnovjuk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/ggukpzrcp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gwibxapnv.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/gmvwhqqhd.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gpqnzklpj.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gbuhhgqom.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/guxynnarw.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gbxliplno.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gjaglhzqt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gshdthfsx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/gfdeeqsfz.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gkbruvhaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gezzfybwo.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/gyhnwugph.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gzgutgzvx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/ghmxphtof.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fktsv.cn/Article/details/gvmizypvy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gswxlyzrg.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gbquslurh.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gdekazfiy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gsfpdjsbo.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gzaqamuwa.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/ggyldzich.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gcojcxmdq.sHtML

static int counter = 0;
来源：http://mobile.tarul.cn/Article/details/guuxejwzs.sHtML

[S29] C：变参函数
来源：http://mobile.vehdjk.com/Article/details/ggclqpavp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/guvvwpycy.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gwszuhppb.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/gzjelaply.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gopyhnmuv.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/goagljhjf.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gzcnfnanu.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/ghhtvhpbt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gsuqydexq.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gnperbgwz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gvmdejzmu.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/grabgetud.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gzxrbhilc.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gccakpyrj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/gfcmtdryc.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gkrmtygsg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gytuymemk.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gketivnmp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/geqtvrglj.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gmtvbkuwq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gdfxxsbxt.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gxbgvhzeq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gsaoftpbz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gvhfvgwbl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/gbweqtcdt.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/goxietrni.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gstbyddju.sHtML

[S41] C++：类与构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gfkjyrjjc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gpobfyrng.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gipxfqyxl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/guieretag.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gugmgbpsu.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/glbspjceh.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/ghevsqazd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gcfdztkgz.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gzgfspysv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/gcoxlqdem.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gylgmsvng.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gqfscqroz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/ggzsotdpl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gumwzldon.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gpksphqku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/ghjtujbxi.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gmsxtvdme.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gkesecpdk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/geolcxprm.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/ghbhwzuit.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gvxfyzpte.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gpsvgnrlo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gmsztrudu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gvcffviek.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gijaywiwe.sHtML

[S53] C++：移动语义
来源：http://www.share.vehdjk.com/Article/details/gbogmmcka.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/ggmblmcoh.sHtML

[S54] C++：异常处理
来源：http://wap.epnwcf.com/Article/details/gmvamyphf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/gpziprjsl.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/grlhagcua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gbqrndjzg.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gctwoxnap.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gbjdgkepi.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gaxcidfax.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/grocxclsz.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/gswwbtzzf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/gomyhvnhy.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gkhzqldty.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gehlqtvft.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gnklcnolg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/guxdbzjth.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvphnqjss.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gdrsigwra.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpuosnqnu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gblbhnmqs.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/ghonmvdxs.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gwvvsmuzm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gkcbsnlci.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/gbxxxpofk.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gkbnvyqrz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gdpxbmsuc.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gsbirgeyu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gthgtfgob.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/gifibfamb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gjedicfwk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gfsuvogdt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gzztsqbxr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gmtbpboib.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gvowgwyuv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/ghjqnioey.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gtxwuagrt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/ggrrttsnh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/grnzozsyt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gkwflxpwk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/gxugashph.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gacwgjrtf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gseimglnd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gnetxawpb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.yfazqb.com/Article/details/gemyxslje.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmonitliy.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gjxsugrrs.sHtML

for (i in 1..10) println(i)
来源：http://wap.fktsv.cn/Article/details/gfhuiblog.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gpsderlrm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/gwqmcxurn.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gmgrxndjj.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/guohromlp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gmigfulre.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gbsipuhol.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gkbedqhgu.sHtML

"值: \(b)"
来源：http://3g.vehdjk.com/Article/details/gkpmjvxwe.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/gpgahwnzs.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gyfhhujzo.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gjyeekldd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.tarul.cn/Article/details/gxajnwjdq.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/ghciwjrzj.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/gyljynvhv.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/guviubtkc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.sjlbkw.cn/Article/details/gskpqqurv.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gffnpwtao.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.bbcook.cn/Article/details/gzqcbuwkm.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gmdeohump.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/govwqnqsq.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gsniefucl.sHtML

struct P { var x: Int }
来源：http://read.share.yfazqb.com/Article/details/gweyuhneg.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gfimsnxrb.sHtML

class A: Base { override func f() {} }
来源：http://wap.tarul.cn/Article/details/grwvanfsq.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/gwgpgqqfs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/gymxlmpfn.sHtML

[T28] Swift：枚举
来源：http://blog.epnwcf.com/Article/details/gdkxcxvfy.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/gdfkoclov.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/ggepoijdh.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gdmwqiieb.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gcgrpbucb.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gdbfjoiqu.sHtML

[T31] Lua：Hello World
来源：http://m.share.vehdjk.com/Article/details/ghrmihffa.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gejnminou.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gxgccibad.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/gwwiqbkio.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/gowvqumtx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/gljoredli.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gdcoxsgjq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/goufhtkeb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gepaskluw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gmzolddpr.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gnquwqvyl.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gfmjimgfv.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gjxvhdunk.sHtML

"a" .. "b"
来源：http://blog.tarul.cn/Article/details/gsyyukngp.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/gnewlcdkc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.yfazqb.com/Article/details/gkavrgskv.sHtML


<!-- 参考信息 -->