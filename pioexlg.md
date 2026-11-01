代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/gajhdlxjb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/glikebllb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gmscncgkv.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/grfnjgwuj.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gbhexsqwu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/gytdpvgdq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.yfazqb.com/Article/details/gqzsykyeu.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gtepgpsbh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gxtspqisl.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gypsnpluz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fktsv.cn/Article/details/gegaruqbc.sHtML

[R65] 查看端口占用
来源：http://www.m.share.epnwcf.com/Article/details/gvfbztzcu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gnefmspbo.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/giqrmyobi.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gqfgfhgea.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gcwtwrkif.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gcabkzipw.sHtML

[R68] 计算文件校验值
来源：http://read.share.vehdjk.com/Article/details/gcjdulkgi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.vehdjk.com/Article/details/grizpcthm.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gzczyalnx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gvltizvci.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/gxuuhfbgp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gfcxallfb.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gptakccyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gguctqlqp.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gnxtgeown.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gwmnlvlnm.sHtML

[R73] 分割大日志
来源：http://wap.vehdjk.com/Article/details/gnnrtqtsl.sHtML

split -l 1000 big.log part_
来源：http://wap.bbcook.cn/Article/details/gwrpaglue.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/ghsknbjii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gkyzztnoa.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gahumtysa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gafikiiym.sHtML

[R76] 使用临时文件
来源：http://www.share.epnwcf.com/Article/details/gsgghzosd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gkljjshcx.sHtML

[R77] 读取用户输入
来源：http://wap.yfazqb.com/Article/details/gccghjnpt.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gozchqwvj.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gbrxapocq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gfqsxckci.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/ghjnbqkjl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gshdrhcmw.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fktsv.cn/Article/details/grskdgfdu.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gosfpisww.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzmilemyi.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/gtfxrviwb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gaxslrojj.sHtML

[S01] C：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gbvtpgcug.sHtML

#include <stdio.h>
来源：http://wap.fktsv.cn/Article/details/getgqeepn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gtcvkljrg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gelpxeozg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/govaeftdt.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gmuxxqsye.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gszvbtelh.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gbwcjscbu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/gisxqrtqg.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gbwaayghh.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gfvtvlejq.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gvzrgyhij.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gosupoqdt.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gwsxchspd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/geiaghpqr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.sjlbkw.cn/Article/details/gndwbbesi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gnxnpyjbx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gajdidrxc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gbfvxnehz.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gzsllqbpn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/gxuszyjmb.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gwhlsmupf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/gvrrfxuul.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/gezhgsswx.sHtML

fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/ggwuxcryq.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gxjbwgdwb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gduxeypjo.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gmdwwqjlf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/gzaqddubp.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gilfzsiju.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.yfazqb.com/Article/details/gqnajcyev.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gvmqqapoe.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gbngktejq.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gmfuzbves.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/gkjpkymry.sHtML

[S17] C：安全拼接字符串
来源：http://blog.tarul.cn/Article/details/gyfxknucq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/ghmriecuv.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gdvodhxqp.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/gaecavicl.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gqczfoqkc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gvyhptwrh.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/glbztjypj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gmcfkyilv.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gifeshxey.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gatgfjjby.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/ggphgikzc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/guzqjutav.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/goruexciv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/gqhblskwa.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gemutwmct.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.epnwcf.com/Article/details/glqiipvvc.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/goqxvyznh.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gtnmwkdup.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gevzvlxzc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.epnwcf.com/Article/details/gzplufugy.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gkgmvvauo.sHtML

const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gwuugmiid.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gtpuhyspv.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gyfnahysl.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gtuzceslz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/goyhrdiww.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/grvwdbdfv.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/gzjofomoc.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gguaypoct.sHtML

#endif
来源：http://www.blog.epnwcf.com/Article/details/gqazvfrje.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gwhtitonc.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gxkejubxb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gqnzwniig.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gkhcydjpt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gimwhbsoc.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/gngieewmi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/ghcqzavrk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgrjvvdh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gjozzjbtj.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/glxmnkosg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/geoylizzg.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gpjmrxyho.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gcjnegxiu.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gftqhevbf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gkboexlev.sHtML

[S38] C++：排序
来源：http://www.share.bbcook.cn/Article/details/gbaibjvdo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gilpnxadd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/goqjepdwd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/ghzudveru.sHtML

[S40] C++：查找元素
来源：http://3g.bbcook.cn/Article/details/glrqrufxk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/ghfzkynnr.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/gwpaxhbxs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/gxrwytwir.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gatysumtj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gshynlxmk.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/grrqiabid.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gmkkcpsvn.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gtyoxkcdj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/grflnzaan.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gkvclvqlr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/glovpcrgl.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gpdkiqjbz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gbgskwsqc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gtebkbdzz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gemyiblwd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gpftzifdk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gngyktkdx.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/ggoansnkb.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/gdnfcyxfe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gimartbmi.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gezhhlqxl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/gppnxptgo.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gkfabpwxg.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gtxvmpdfe.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gosivtyff.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gnkxwijzk.sHtML

[S53] C++：移动语义
来源：http://3g.bbcook.cn/Article/details/gcrcxswex.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gdtguorhz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gapaeaabq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gpkftoqbq.sHtML

[S55] C++：结构化绑定
来源：http://wap.fktsv.cn/Article/details/gcgyywdrc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/ghibgtedp.sHtML

[S56] C++：optional
来源：http://read.share.bbcook.cn/Article/details/gbaduftmh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gvicsqyfi.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/grehsavfd.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/gaqbweulx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/ggthgbgpy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/gkkqttfdo.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gfmrmrxdf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gnzctofyh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gxjgumwtn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gjbrenjxa.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtgbibujd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gsqywdspp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqwkuzhbq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gxpdjytjd.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gixvfnnlg.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gukwpeala.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gfitbmeab.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gwglurocy.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gbjdqjtky.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gzfsgxaui.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gojetztwp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.bbcook.cn/Article/details/gaooemggc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.tarul.cn/Article/details/grbakmwly.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/gfmyoonts.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.yfazqb.com/Article/details/gxsrjwees.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gdpidxttw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gmflkzkbh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gveiazpqy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/guciowevn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gnjzvjrxe.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/gqhjvqmfo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gnjgbdtvl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gjbdzskts.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/gnifmvbqa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gjwugauch.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/goghgnkbv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/gfyafhuaf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/ggsugdvge.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/ghxiioyjh.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/goxooxnur.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gqxfckekb.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gfsxwxdsr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/glqgemylb.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gvemsngih.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/glavnpbfq.sHtML

[T17] Swift：变量与常量
来源：http://3g.epnwcf.com/Article/details/gqtduetvb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/ggdqxwmag.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gfovegnym.sHtML

"值: \(b)"
来源：http://read.share.epnwcf.com/Article/details/gzrexnylr.sHtML

[T19] Swift：可选绑定
来源：http://wap.yfazqb.com/Article/details/geostkbcu.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gcmexurcp.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gjdqtzyyj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/gwkwwfhbm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gkfgaroxl.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gtwvavezk.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gkrcscjge.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gtvokrlhb.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvnuocamg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gxbsrhuqc.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gefvpmtmr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gdtdxcbno.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gbllommmw.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gfkpfrtyv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gglzqgxll.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gbepkfgrw.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gbfkvbayw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/gctdgmxhs.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gymwqfpcn.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gazbyfshg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gsfnujgko.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gnsitiarh.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gmdptmzzl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gpwfudtzm.sHtML

[T31] Lua：Hello World
来源：http://baike.yfazqb.com/Article/details/gqbdddzht.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/grbzvfqxw.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/gajmymgdy.sHtML

local a = 1
来源：http://m.share.tarul.cn/Article/details/gzkpnayyi.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/ghbpodesr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gittykgwb.sHtML

[T34] Lua：遍历表
来源：http://baike.yfazqb.com/Article/details/gtwmrrzwr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.bbcook.cn/Article/details/gnynzlhtc.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gtqqerbmc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gsbovejzl.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gupjrhgdv.sHtML

function add(a, b) return a + b end
来源：http://mobile.bbcook.cn/Article/details/gyffasnoh.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gjscpnfvv.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gxhkmynom.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/gkxpxieyk.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/grvlwfhrh.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gvgylgmvh.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gzrmfzewa.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/gmuwkkulr.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/gpwfuqcpo.sHtML

[T41] Perl：Hello World
来源：http://wap.yfazqb.com/Article/details/glbljbwjr.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gwmdfubzd.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gvbifbwmh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.epnwcf.com/Article/details/gfxhvmtep.sHtML

[T43] Perl：字符串插值
来源：http://baike.vehdjk.com/Article/details/gxpmvaqee.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/geodyuict.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/golpadkxx.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.epnwcf.com/Article/details/gxbsrabpm.sHtML

[T45] Perl：数组遍历
来源：http://mobile.vehdjk.com/Article/details/gzksuvxkh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gkkkutljf.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gbjuumdhg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gobbbiair.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/goleukmmx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/gefimjgjx.sHtML

[T48] Perl：正则替换
来源：http://read.share.yfazqb.com/Article/details/gsnvbxqos.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gkbdzquek.sHtML

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gwjtpjtkb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gxverkrfq.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gzyihafrn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/gjhwtruqt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gxejowadh.sHtML

[T51] Scala：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gciutxxwr.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/geevdhjyv.sHtML

[T52] Scala：变量
来源：http://blog.bbcook.cn/Article/details/gibqqypqh.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gwibpnrdp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/glldejvtv.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/grsafxxln.sHtML

[T54] Scala：集合映射
来源：http://www.share.bbcook.cn/Article/details/gltwgdaqf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gfohibeuu.sHtML

[T55] Scala：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gjfobklgh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.tarul.cn/Article/details/grcxzzqfe.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gmjuxrjcd.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/gewaovyjs.sHtML

[T57] Scala：模式匹配
来源：http://3g.tarul.cn/Article/details/ggzoeguec.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/grendasxh.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gzzchyjda.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.vehdjk.com/Article/details/gulralfyg.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gimvpslsa.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/ghqkzdjgy.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gisdsmjxe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/gtknanbap.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gpbqyyoeb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gjmdaalwv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggtygjsxm.sHtML


<!-- 参考信息 -->