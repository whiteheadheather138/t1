代发 wailian999

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkimpzqc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwarxyang.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gdvqhgccf.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gnvxlzknb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/gpbzkjwwv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/gjdtkrlpx.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/gcwusvqbi.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gkuuglavr.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gyggamjbd.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gqlrekzuv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gpublstjl.sHtML

[S05] C：字符串长度
来源：http://mobile.epnwcf.com/Article/details/gslelnwvc.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gttjxjqlt.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/gwcoqqrrs.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gpfxlptyi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/gmrkyntgf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/grhxorrzp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gezkhahxq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.tarul.cn/Article/details/glvvctsqx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/ggytdzjht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/gzdtzflyz.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/goctdzfij.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/gsopduqxp.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gwsjaslfq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gujnvwozv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyadyuglg.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/ghtuzsuir.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gvfhqczrt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.epnwcf.com/Article/details/gjqocwzfl.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gkfvkrgzc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gbcoolokz.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gdslxljuy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/ggwqzdxsd.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/guyfaeokc.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gqkksdgoz.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gakpehzzs.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gpynhdvqy.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gepkuvjzp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.yfazqb.com/Article/details/gsisnlvao.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/gypkyxgwh.sHtML

int main(int argc, char **argv)
来源：http://blog.epnwcf.com/Article/details/gilrnfcbq.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/gybwatten.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gllvawrvq.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gibjbpvkc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gyynkuhok.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gfqyhqgqp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/goepbfljf.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gdzvjsgtg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/gvchrrmuv.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gcfdaehvg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gdmwdfbkt.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gdykkwozy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/goppxdduq.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gornyyejp.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gixhotgtf.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gvokovmgu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/gxihliukl.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gejqsvzhp.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/ghbmdmomx.sHtML

[S28] C：静态变量
来源：http://www.share.fktsv.cn/Article/details/giselqkrd.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gmvpxamzo.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gaupyhnuc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fktsv.cn/Article/details/gokpujmie.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gxqziwwdl.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gcvkkfguh.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gcdgkmvno.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gfonxzgjm.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gvoqlsfza.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gwfzyllrm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/gtflzuyjd.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gudcqbnaw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/gqaqbxase.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gayhikbpq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gjzmbpyvs.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gqxxnipvi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gbbtovibw.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gnkqedqyg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/goeiihveg.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/gdihyyaxb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/giegxtvrq.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/gupybsriw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gnynrrspn.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gvndhsxcd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gwlugowcq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.tarul.cn/Article/details/gikzrojtm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gurympxkm.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gfrnmvvvz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gfdblpwiz.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gmynrdbfb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gqgrfmlnl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gezosjakc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/guevwpozb.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gzhxbejbq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gtxbcpdbq.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gxlxjnygd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gfaipjbsa.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/gzikhbqem.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gvqalxgkg.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/grozpmobm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gjeebjilg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/guckwbsoa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gyhzobqgx.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/ghjcprcdf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gwmwvtpkj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gotypbekt.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/glsoxjocy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpaigwwf.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gmgmhsnpi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gcnjnltps.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gyeajpqss.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gvoyckyzu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fktsv.cn/Article/details/gdyiokcvr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gngsbygfh.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/glvivkiml.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gfzphfunw.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/ghfgkqirf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gizeuqnus.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gjwyqzwkv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gefmyfhzt.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gzgcrffkt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gccdyybla.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gesaqxkos.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gijpvfjbg.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/gusvwlsmj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gvgokhwek.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gilmhvwcd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gttycsxul.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gzzppazmj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/ghjqufuoz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ginltntpp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gqvkcwcqk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqjsigdpt.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gbmseyuyk.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gidgutjao.sHtML

[T02] Kotlin：变量
来源：http://mobile.epnwcf.com/Article/details/gjrsbupcp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gxhyfdjnl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gihmorzni.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gxdbhukhp.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gvzhyzmtv.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gpykgllgs.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/greuvgiku.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gkjdyxzif.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gypoxhaqm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gdgvcbiuj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gpibjfbnv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gmnwvouhp.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gcyjegqvp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gllujhmjs.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/ghfjaonhj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gfvbcybif.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gonoyyqha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gbctlqqlu.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/gfqslbzlc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gygjxwwif.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/glshfpkmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.yfazqb.com/Article/details/gmywnnovq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gehqvinzs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gxwelublg.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gwbsksehw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gbztwipwe.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.tarul.cn/Article/details/gethtvpxy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/gotzukplm.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gzpaubvqc.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gqhumhpiw.sHtML

[T17] Swift：变量与常量
来源：http://3g.yfazqb.com/Article/details/gfxkimoiu.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gyavxmvrx.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/gqbpynqey.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/guvniewzx.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gqhlkdgrq.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gvujtgshb.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gujzqtghk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gbczwvlpb.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/gzezilihw.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/ggfwsdcjg.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/ghyriyzwh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/gwhrodbvs.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/glwbnrwwm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/gvgkwbswl.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gcqpgxany.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.vehdjk.com/Article/details/gffhxvdxc.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/gprqsbagr.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/gxqoaonpy.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/gejkywmls.sHtML

class A: Base { override func f() {} }
来源：http://www.share.epnwcf.com/Article/details/gsjdbgdae.sHtML

[T27] Swift：错误处理
来源：http://mobile.epnwcf.com/Article/details/gncpxongl.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.sjlbkw.cn/Article/details/gdjrjltnv.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gezeryosu.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gbthnkmhv.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gfvezqwen.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/ghosyhoqq.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/grqawofuu.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.sjlbkw.cn/Article/details/glxawbttq.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/gytqaftxv.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/godpcvloe.sHtML

[T32] Lua：局部变量
来源：http://blog.epnwcf.com/Article/details/ggzilvwav.sHtML

local a = 1
来源：http://blog.epnwcf.com/Article/details/gdtvaiaby.sHtML

[T33] Lua：表（数组）
来源：http://wap.sjlbkw.cn/Article/details/gafhltvau.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gihpuhzaq.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gacoghhgd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gryerdypq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/gmfvafupu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gypwdrxgx.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gpqwhiyub.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/giwlsqxmz.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gmmzqsooc.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gaoqemjmr.sHtML

[T38] Lua：条件
来源：http://wap.yfazqb.com/Article/details/ggtxhpecq.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/glqauderd.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gvcozlunq.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/gapcpftgl.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/gzxzujnim.sHtML

setmetatable({}, { __index = base })
来源：http://baike.vehdjk.com/Article/details/gwxfsdcds.sHtML

[T41] Perl：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/giqqenwnl.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gshnzhnjl.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gcjmaiqde.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/gmbqxvilv.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gturbyjrx.sHtML

"值: $a"
来源：http://baike.epnwcf.com/Article/details/gffwopple.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gstzkmzjw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gugmytxht.sHtML

[T45] Perl：数组遍历
来源：http://mobile.bbcook.cn/Article/details/gympekrad.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/ghkicqlnb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/gfjlwoxjt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/gvhwsojww.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/gtlacjabh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.vehdjk.com/Article/details/gozaaznyy.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/gazvqcsof.sHtML

$s =~ s/old/new/g;
来源：http://read.share.vehdjk.com/Article/details/gfjoaezhe.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/garnbyuwz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gpagvyygt.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gjjqcfllt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gfeglvpop.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fktsv.cn/Article/details/gbfahyxno.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gkpsermel.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gpaauyrge.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gftuxtpkc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/gwvwfulan.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gstgasjdv.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/glrydehex.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gpyhrntmz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gwutjoowg.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/gexpoezoq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gfimohzxs.sHtML

[T56] Scala：样例类
来源：http://read.share.fktsv.cn/Article/details/gjozqqdhu.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/guyrtznrb.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gsouqgnrx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.vehdjk.com/Article/details/gqfzsdzqp.sHtML

[T58] Scala：函数定义
来源：http://read.share.tarul.cn/Article/details/gkvrduhrc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/gyyifxtav.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/gvuojlqnc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gzllafxal.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/gambkmcmk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/geelcjgbv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gifrtphnw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gpukxxshm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gizykbzdz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gfbmzixfk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.vehdjk.com/Article/details/gergdmesg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.epnwcf.com/Article/details/gcxafquwb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gtryfaoed.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.vehdjk.com/Article/details/grjvdxehw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gyofcsnvb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gzeeivqla.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gmjwkdlha.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/gegqpmdmt.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gmyzxztfu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gcmhpagvp.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/gocjroxue.sHtML

[U07] Py：反转字典键值
来源：http://3g.tarul.cn/Article/details/gwwbuwivl.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/ghbjovnmw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fktsv.cn/Article/details/gdsvmwboy.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/ggtxzaxsw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.vehdjk.com/Article/details/gfecxvcim.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/gzdeqgnmt.sHtML

[U10] Py：按值排序字典
来源：http://mobile.bbcook.cn/Article/details/gigtgzlnf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fktsv.cn/Article/details/gwaktqzhg.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/gfpsjosjn.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gpuoamuvq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gbxrjjxbl.sHtML

Counter(arr).most_common(3)
来源：http://3g.vehdjk.com/Article/details/gbovwwzep.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/guoaloltr.sHtML

deque(maxlen=10)
来源：http://m.share.fktsv.cn/Article/details/gbpajnftr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gslebzxwk.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/grjovxlad.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/gcsaxaodu.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gznvrzvqc.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gkhburpti.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gfnnamkvq.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gnworajpa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.sjlbkw.cn/Article/details/gyavrtajr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/geiwkzuap.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/ggnqwgllr.sHtML

[U19] Py：正则替换带回调
来源：http://3g.sjlbkw.cn/Article/details/gwoyypsrv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gyxldthrt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/gyvxfszwb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gbzvqjaep.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gluwliqao.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/glzhbzoef.sHtML

[U22] Py：矩阵转置
来源：http://read.share.epnwcf.com/Article/details/gkdjzobtw.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/gbobkrgxx.sHtML


<!-- 参考信息 -->