代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gjwjelkfk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdwjymek.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gwqnxxgve.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gpradpacj.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gjzapcwby.sHtML

[R38] 管道串联
来源：http://blog.sjlbkw.cn/Article/details/gvprfyygw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gdometyrb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gwrtbiiec.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gjpnviwtd.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gxqgmoule.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gfgajwmgo.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gdqnzatdr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/goiyuuaik.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gbtgwbyfa.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/ghnavqnwj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gitzikdyh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gdpfdixiv.sHtML

[R44] 按修改时间查找
来源：http://mobile.vehdjk.com/Article/details/gzpjsrlkf.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/guoxgdbhj.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/glfpcnxvw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gouvawhts.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gtckzbsit.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gppcojnnh.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gsqcapsat.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gttddndwd.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gqairwjzi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gdzvhcvdv.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gcanlatgf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gnqodmhnc.sHtML

[R50] awk 求和
来源：http://www.m.share.yfazqb.com/Article/details/glvgfoarf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gzxaatlyg.sHtML

[R51] 排序去重取前几
来源：http://baike.sjlbkw.cn/Article/details/giokihsus.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/gelqfifzb.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gsnftqavu.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gwkiqltcp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.sjlbkw.cn/Article/details/gatxxxspi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/ggiptbufc.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/ggqjlacgq.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/getdpuyjh.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gsrwjeiax.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gltaunjiq.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/grkevevyb.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gstwypeep.sHtML

[R57] 远程执行命令
来源：http://3g.yfazqb.com/Article/details/gojrmwgez.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/geycrnaxg.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/godqmbtuh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gkqlrebao.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gjfovnyhc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/gcvhqlexa.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gaxduywxw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/grtyfykwe.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/gektnyztu.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/godcormvz.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/gnonbjdvc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gqniwjubx.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gplzxsrgl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/grrqrfykp.sHtML

[R64] 结束进程
来源：http://read.share.yfazqb.com/Article/details/gntslapof.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gdcupqnsb.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gpivfokpj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/gqvbhdydv.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/guogaywcg.sHtML

crontab -e;  crontab -l
来源：http://m.share.sjlbkw.cn/Article/details/gthesjpum.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/glmcqiswk.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gsswprluj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.yfazqb.com/Article/details/gyotpaduk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/glgbvwxhj.sHtML

[R69] 生成随机密码
来源：http://m.share.yfazqb.com/Article/details/gyllhbyeo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gegjhieyg.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/giuvfxmgl.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gwcipeucr.sHtML

[R71] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/glqmyypzl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gzebznzfs.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gpgebrrop.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gfkveysyh.sHtML

[R73] 分割大日志
来源：http://www.blog.yfazqb.com/Article/details/gsncauoyx.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gqdcsunjr.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/gsiobrmzl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gddrnaptz.sHtML

[R75] 导出环境变量
来源：http://read.share.sjlbkw.cn/Article/details/geikrptyq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/grdsklxcg.sHtML

[R76] 使用临时文件
来源：http://m.share.tarul.cn/Article/details/gjenlffua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/gidiuycri.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gcavtintt.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gnsrgfgqk.sHtML

[R78] 交互式菜单
来源：http://www.blog.epnwcf.com/Article/details/gamlamgsk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/geadxkffp.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/gfzwwauri.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.tarul.cn/Article/details/gzsenbizi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/gbphdojjr.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gafztmqlk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwuyexpup.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/grqcedvqp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gruhztbkf.sHtML

[S01] C：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gaeskryoo.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/ghwsontnw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gcscvfgaf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gapmcszvt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.vehdjk.com/Article/details/gasoturxg.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gujymhgno.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gyrgusuvk.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gsqakwxxb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gkppkambc.sHtML

[S05] C：字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gwusnzect.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/ggjwuzyjy.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gtkmhusmj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gmuafcjve.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/grkwxpqpw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/ghtkuqmap.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/gttibeenu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gbmpspuby.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gncznjjwt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gjeunsggs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gspwyxlys.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/goazgmmss.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gmrtkjxtr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/grzcpitkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/giovripnq.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/giqtuieuj.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/geabulcax.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gtpfhxvmr.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/gwodhbrtb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/ggbibcvsc.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gutebesej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/guxossmzo.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gkejwnqez.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/grkolljqi.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/gsshvurea.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/gmyycqnjx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gytsmewvb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gghdohfpj.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gszvyqysc.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gkiktrwgn.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gmxlmxedk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gnddoutsk.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/ghisdscbh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/guobcypcd.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/gpeqrmwbu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gxjlgckuj.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gplgqeebp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fktsv.cn/Article/details/grxlvjwsn.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/ggvxxinxd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gzjsjlkyv.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gjymnhjwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/gafzhldsl.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gojalipbd.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/gfpwmxfhl.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gfzwsrwtp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gcihskxud.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gbwiuktvt.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gdgscztvq.sHtML

[S28] C：静态变量
来源：http://read.share.vehdjk.com/Article/details/gcpvdlwcc.sHtML

static int counter = 0;
来源：http://read.share.fktsv.cn/Article/details/gafgajgsr.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/gdtihsijf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gpqqmzche.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gwqwzihlu.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gszllkucq.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gdzkeqlct.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gvywkejlv.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gtldtxdbx.sHtML

#include <iostream>
来源：http://www.blog.vehdjk.com/Article/details/gptrgxzga.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/ggwesakug.sHtML

[S32] C++：字符串
来源：http://www.blog.tarul.cn/Article/details/gsvpwyimp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/guegopxot.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/gqfssdioq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/ghktolniu.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gugbjsoqc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gfwmfhvig.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gklwftqxf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gcfqocism.sHtML

[S36] C++：unordered_map
来源：http://www.blog.vehdjk.com/Article/details/ghwoxuqeb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gudxrnbvv.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/goiyqenee.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gfbpaooic.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/gtnipyxzk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/gwaktfngr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gfhtmrlhq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/gexhyvsgy.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gsphjjrqx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gfxwmkpfb.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/gqoijaccj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.tarul.cn/Article/details/ghpdwpgyf.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gxxboendf.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gyjcqlfxu.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/goncjffim.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/gayrlcdwb.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gbftjawrg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gojhpkfnl.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gcalxtsyb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gftsiinhl.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gnhyanryd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gebhhhegr.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gsepaaucq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gqwesrpuo.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/guctgotqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/guumlreuc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gsrjwtyqh.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/gjtpzelcn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gvhjovxtp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gylmbffjj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gwbbchacr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/gpaonmuvt.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/giwfrvmew.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/glholbtff.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/ggnvontpm.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/ghvyqnhvx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gqicfqool.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrqvgbqa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gxdewgwwd.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gcnqslkmh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gysbhsjxv.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gizksswax.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/girnapxoe.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gbjutedwa.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gewzpscyo.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gobgpejvk.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/gzmcmyhux.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gagnqygjj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/gdsdvjkjy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gbbbwpyty.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.tarul.cn/Article/details/gsuvriahg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gigdjteie.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gqrmogmky.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtkkfddzl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gqolulmds.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gqlnftwls.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/gsodsviqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/gusgqlnog.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/glawtewhx.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gdwcoiijx.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/grydzsdfw.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/gphyflzja.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/gxffcoaqe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/gzvqomhvc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gfjwgkrwm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/glvnzsffu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gpjhljwgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gmjsmqqmz.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gditrdwzp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/gohhbfstm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/glqmxbpro.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/grrmwzmmb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gaaozvqac.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/goactlgoi.sHtML

[T11] Kotlin：协程
来源：http://3g.yfazqb.com/Article/details/glbjjupkf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gftwnhblk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gpqnmtoov.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/giuazjims.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/gqkbfrfqs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/gxergjerv.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gfaelobow.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gkelitjhk.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gnrnsxgoj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/ghsmwomzl.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/grgjdyizc.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gqqrnrggy.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/gixuhorrm.sHtML

var a = 1;  let b = 2
来源：http://www.share.epnwcf.com/Article/details/gyktrvsgj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gavnhecfr.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gqnyqrlwr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gplbsuywz.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/gcjshakwx.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gwcabobkt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/galjumzvt.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/gpdpgjtgs.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gxgmjueta.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/gfpatrnjw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gqfogvavw.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gsknihrmh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/gqcdzztxj.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gfapbofxb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gzgagoosx.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/gteqycwmt.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/grqlowjhf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/gmcroxmpx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/grojthtlt.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gzgjkhkoi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gtceyuntk.sHtML

[T28] Swift：枚举
来源：http://3g.epnwcf.com/Article/details/gcspkzttd.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/guppsuiyv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gemtplegm.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gbqoixrda.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlyeqghk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gnhmbdxms.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/gbzzhfpqf.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/geoazzvkr.sHtML

[T32] Lua：局部变量
来源：http://blog.epnwcf.com/Article/details/girjjdxwf.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gwoxcxfsa.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gzdibblue.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.bbcook.cn/Article/details/gqhfhdtkj.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gmslbtuwo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gtuwldypt.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gqtnnthfg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.yfazqb.com/Article/details/gpimkbrdk.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/grggrpbrn.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gdnemysgh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gablgmadc.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/ggzvvxyxp.sHtML

[T38] Lua：条件
来源：http://baike.bbcook.cn/Article/details/gtyfcesuy.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/gewerfvkn.sHtML


<!-- 参考信息 -->