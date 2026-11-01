代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gkcwtcbek.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gkjlvjnjp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/ggmuzvmxo.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/gaawuxsly.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/gdgrpmzwn.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gevarixex.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gkyrnlhka.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gcowtdlos.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.sjlbkw.cn/Article/details/gopzheeqv.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gnlmxvrna.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gdwafelyt.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/ggvcrwbjd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/griqnqnjw.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gsdmtuvlz.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gfkxnmpkq.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/ggebkvkhe.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gvgyiwwet.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gxyippexa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.tarul.cn/Article/details/gdqfsnowv.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gzcfzltku.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gjtskcvco.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gdensisow.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gdsfyndkc.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gftwcjlte.sHtML

df -h;  du -sh *
来源：http://baike.yfazqb.com/Article/details/gexeyfyhw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gjylpblpt.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gjnfdeusw.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gsjmyroih.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/ggugehnzw.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gczofaprs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/ghemdlphc.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gwwconplo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gxzkxhlrk.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/gjuoqnnyg.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gdnvlydda.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/guppkzueq.sHtML

openssl rand -hex 16
来源：http://read.share.sjlbkw.cn/Article/details/gxlmbmaiw.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gtciyeplq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gkzkovcwv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gvmbtsbyh.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/ggbnkaqhr.sHtML

[R70] 时间戳与互转
来源：http://blog.tarul.cn/Article/details/gnvtwpqgv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gxzfikyqc.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gavyxdbgc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gwyrfdgju.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gietdrvgw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gehdbhtwu.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gshaodzws.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/gfvvvuvml.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gywyziptf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gcyaaetpm.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gjizmuvtw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gvfdnkgjs.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gpxrhocpy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gbirvxvzt.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/ggcbwriuw.sHtML

read -rp "请输入: " ans
来源：http://3g.vehdjk.com/Article/details/gxypdhwxu.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gchewnmcc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/ggjtitiri.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gwzuxphyl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/gxwkmweup.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gbmawlfrc.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gqiqsypqp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnrnexsif.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gvevynsfg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gegmjiphq.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gqphwjovw.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/goluskbmj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gyzegguyl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/grwxnopdv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gobtqfchk.sHtML

[S03] C：读入整数
来源：http://m.share.tarul.cn/Article/details/gwhphpyga.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gerujydea.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gmpcnodfp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/giswnnobh.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gdwzrqixe.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gqmqtephr.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gaptnxrtz.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/grijtlfoh.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gsazttfju.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.sjlbkw.cn/Article/details/gpwmusfla.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gnaghjxat.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gnzzxkxvg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.bbcook.cn/Article/details/gbgkahqxt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gfpjooxpq.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/grylhpxjz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/ggttvuibu.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gtwqjbvem.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gutnpfccr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gynhngfar.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/grsqgomvo.sHtML

[S12] C：写文件
来源：http://m.share.epnwcf.com/Article/details/ggtuqlgyq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/grlmwqdfc.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gwobqmprh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gayemdybc.sHtML

[S14] C：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gmoqhzret.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/gggovqghf.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gcgxwhuyi.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gdwyhouoe.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/ggnoilwlo.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gevorgrxx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gahjlzkoi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gdueqkqfb.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gmjegqhht.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gpxbtprgx.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/geyopnwgh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gqjrawbun.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gvtjbmwkb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gagwfljie.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gynwvnahe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gkytovcis.sHtML

[S22] C：字符串转数字
来源：http://blog.bbcook.cn/Article/details/gxvhijexz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/ghffiskpg.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/giwrfkdkn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/ggxdperyu.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/gtpbpygtn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/guyxesvjp.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gllwpvwrk.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/giavdqrzv.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/gnexbbghq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/grctzlejl.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gaagrpzsj.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/guwnylnoo.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gvnopzlon.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/gzyvasryb.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gxsbxopvn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/griptnchb.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gllirgkjx.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gkuojsmvj.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/goxcpwopv.sHtML

#endif
来源：http://www.share.sjlbkw.cn/Article/details/gzogwzwvg.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gzipdwjte.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gemuxhmpm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gzmbsqzxt.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/gegmghxeh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gjiibaitt.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gfdgkcwxy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/gnvkfqrng.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gsabdrnrt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/ggqgtyroy.sHtML

[S35] C++：map
来源：http://baike.epnwcf.com/Article/details/gshgepvvt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gjhroybbb.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/glqsuadps.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gnekemufq.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gppmcjptp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gcjyuewsg.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gslpkawui.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gksptbvrr.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/grvhzujbd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/geyzxgnui.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/gvoahaviv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/grfccmivv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/grhdzdqdz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gilwexooj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gnxfxotds.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.tarul.cn/Article/details/gpbzqlynn.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gctfehwnd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gucgvoidm.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gkgmgaxcy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/guuarfmxm.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/glhyzezqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gmgjnxlta.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gglnoazcz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/grmqbbbgy.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/giwshigib.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gwtogfryt.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gxlalevpk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gnjdusttr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/gjrilwufq.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gbsxduadu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/grgpuolzc.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/grjsuesuv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/grrcketpe.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/guxmgsibu.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gbzrthfuq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gxjwpoqjh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/ganhfblyr.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gdopejuzv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/glikdccyd.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/ggfvbbpqm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/gppheuxml.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gezzerwsf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/grxuacysa.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gzdxowogg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gxdsmndew.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gdtimazxy.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gzbvzxprv.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/ggwpopdki.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gxecczlsi.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gmrspowqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gfzphumpd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gxdetldrf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/giawsskzp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gssbxfyrw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.bbcook.cn/Article/details/goqyigmxd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glcuqbecs.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/geyiqgiut.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gftbxmzcy.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/gwwxuaceh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gqecntuwe.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/gseohrced.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/gwbazpeyl.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/ghrdiumkr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/gwdsvmfme.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gqmsgzhcc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/ggjelbsvt.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/grjcsfbck.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gnvksgyqg.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gwpcbsopq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/gbspycpfn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gwnawkutr.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gehrgsplu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/galmbanww.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gmzvbtukw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/ghstmzgqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.epnwcf.com/Article/details/gqjzvskhv.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/gvebrrzfp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gopjkdaak.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gopsgnjjb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gmzadbfxr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gqgsigmck.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/gapfdadah.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/ghtkajmku.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gonewyfpa.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/gthfwonqa.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/gqhdqforp.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gapbbzgym.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gthyxqelp.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gjgofxtwu.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gdpkpokxm.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gqjzwvbqn.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gnnmcthfr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gwsagnusr.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gonlvmtoj.sHtML

[T20] Swift：数组操作
来源：http://3g.yfazqb.com/Article/details/gcucolhht.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/gpnslfeit.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/gxxfeizbg.sHtML

for x in a { print(x) }
来源：http://wap.tarul.cn/Article/details/gmvfyhvzx.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/glxgyopnh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/gxkzqhyhc.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gxwcajvbi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/gsgvepwjr.sHtML

[T24] Swift：闭包
来源：http://m.share.tarul.cn/Article/details/gvvcemsyu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gebpvqwcu.sHtML

[T25] Swift：结构体
来源：http://read.share.sjlbkw.cn/Article/details/gumxvongb.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gwshabvad.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gcohgjpwn.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gbxarftje.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/goeogwkhh.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/gxnphjgcy.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/ghfguptma.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/gtyxfieim.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.vehdjk.com/Article/details/ghubwsbws.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gbtcilgqr.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gmdmexlic.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gpstbaasg.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/gtgysyfhz.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/ggkunvzok.sHtML

[T32] Lua：局部变量
来源：http://baike.yfazqb.com/Article/details/gyztnkcme.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gsocqgfqz.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gvpdxyqsm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gykfhoafh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/guspvszuv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/gnuhldgyu.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gqthgeqzs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/gimafwmet.sHtML

[T36] Lua：函数
来源：http://www.blog.fktsv.cn/Article/details/gswylwmtk.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/gjzpevcfn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gzplauirc.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gzdtkkjqb.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gpjdtrikg.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/glklxnzcg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gqcsjgxgq.sHtML

string.find(s, "%d+")
来源：http://m.share.yfazqb.com/Article/details/gnxxhwooy.sHtML

[T40] Lua：元表
来源：http://www.share.fktsv.cn/Article/details/gfvalcaiq.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gyxzgcdhl.sHtML

[T41] Perl：Hello World
来源：http://mobile.tarul.cn/Article/details/gbkenatzw.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/geewiypst.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/golmpxfsb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.bbcook.cn/Article/details/gguhultun.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gztcrfhkv.sHtML

"值: $a"
来源：http://read.share.bbcook.cn/Article/details/gtzdqfxdl.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/gjdwngsgp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/geojhwbds.sHtML

[T45] Perl：数组遍历
来源：http://blog.vehdjk.com/Article/details/gtjgedgql.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.epnwcf.com/Article/details/gcgatilbt.sHtML

[T46] Perl：哈希操作
来源：http://m.share.vehdjk.com/Article/details/gcdcchoho.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gnvoyiyyk.sHtML

[T47] Perl：正则捕获
来源：http://wap.bbcook.cn/Article/details/gbplbould.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/gbuzltszs.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/gpoxzlpkj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/ggkzszmhi.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/ggbttneeu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gpwtvxyxt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gfhyyvhkk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/gzsspdabb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.yfazqb.com/Article/details/gpiixfjoh.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/giizaoaoc.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/glfawcfze.sHtML

[T52] Scala：变量
来源：http://wap.yfazqb.com/Article/details/gbgheqptt.sHtML


<!-- 参考信息 -->