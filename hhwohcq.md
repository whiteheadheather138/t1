代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.tarul.cn/Article/details/glcmnlora.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/guknoirkc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/ghfrgyuml.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/ganfstvgd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gxwkcfjky.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gdhtkfvlu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gdbezgjto.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gpqvzggib.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlockxbx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gncmxfnvm.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gmqmjypix.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gifgfhqcj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fktsv.cn/Article/details/gkqilhymw.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/greyjhdxw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/gimgsvpzk.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gxmjdxljb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gaegntzhn.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gyjscnzjx.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gqswgymbx.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/ggswkjcti.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gqbfccrua.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gifqjnfcb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gtwfjjung.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gqxxjogkm.sHtML

int main(int argc, char **argv)
来源：http://blog.epnwcf.com/Article/details/giuofyfck.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gmvdotjza.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gehdbdlze.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gyxydxnrj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gtdexbvtj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fktsv.cn/Article/details/grzaqkczj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gdxvowczs.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbxhqxzk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gulyqizfi.sHtML

[S23] C：随机数
来源：http://m.share.sjlbkw.cn/Article/details/gspostden.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gwildwmhp.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/ghelgiecw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnslleuis.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gcwhuhopm.sHtML

memcpy(dst, src, n);
来源：http://www.share.bbcook.cn/Article/details/gdcaazjnf.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gzrlmfjbj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gpeqrxhrq.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gtvzxpscq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/grrujmjxw.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gjbiqrqvr.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gzeqvpfbv.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gsuprywew.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.bbcook.cn/Article/details/gfknxcxby.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gvsawmjdt.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gkquyoopl.sHtML

#define X_H
来源：http://baike.sjlbkw.cn/Article/details/glgxaufda.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gjpykwrko.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gkzoccvwj.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gzpbhlhxx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gimylckrv.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grhfedfrn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gjkgzilci.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fktsv.cn/Article/details/gantkzwuf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fktsv.cn/Article/details/gunskyxdo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/gtlvthslh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/gketvqxfl.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/ghblsqziw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gjmwnfpks.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gsvaggdbe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gbcsyzdou.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/gowotduip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gynupcojc.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/gfuanucbs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gmjykbxov.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/gsiwudorw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/grlnraige.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/gdzqfxzul.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/gilxtyret.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gumqknhgn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gvyckcyrl.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gjculbuxw.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gfdrikasd.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gzazgelup.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gisgojtvw.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/grimnabwq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gukldrajk.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gtjkzagxw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gdhvbcier.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/galbceyfe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gmprpckib.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gdqnwwsbq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gjwqhtjpp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gfkethjfn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gssdnjjrj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/ggpfcpbep.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/gjglzavbw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/ginsfmhdh.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gfnnvenwu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/grwwhpelv.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gxypqyfgc.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/grsjhypht.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gdyrpergb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gsmkxzcvp.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gbqkrstts.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gzvxiebfj.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gfuswtkwq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gpjkzrpyl.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gyfgypnwl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gzelyfsfw.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gpjmqnyuw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/ghjwgszhp.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/gwjmeydex.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gchutgrhy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gjebapuub.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gvhjntawh.sHtML

[S59] C++：静态断言
来源：http://mobile.epnwcf.com/Article/details/gxlkvotfe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gmivqvwse.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gzkvfczgr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/glycrsyup.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpvdzbuwp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gyflcvlti.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpanpjfiu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gjljfemiz.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/giugmewmp.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gidiuxccq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/gahuyrkij.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gbennlyqp.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/glowfwktt.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gqvfrvfpv.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gpfjrsexl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/glrpfrbqz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gcngurkuj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gdsmcqrqb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/gqudydzij.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gwvqgsdgv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gvqtavbra.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/geuiooxlw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/ghtkjsfcu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/ghfdkoulx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.epnwcf.com/Article/details/gluwxueuw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/glfmrsngp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gqoiiceuj.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gpmxbddcf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gwbcbwipn.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/gylagwrwe.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gkykrzgzu.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gfqdhqvra.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gsojcxeau.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gmyxswinm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gfumiweme.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gtovhhykq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/ghxfiamwu.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gfxzdskkx.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/giprtinyr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gelmcgjil.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/gentqqvfu.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gkwecljuu.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gtsozkvqz.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gcscmbxvm.sHtML

if let n = opt { print(n) }
来源：http://baike.tarul.cn/Article/details/ggsmdbbld.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/gpoxxrujq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gzkgkdpsl.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/ghwrfakuj.sHtML

for x in a { print(x) }
来源：http://read.share.fktsv.cn/Article/details/gtvarkqgw.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/grchfvvyh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.vehdjk.com/Article/details/gxneusvdx.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gnsmlpgpr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.sjlbkw.cn/Article/details/gwjxbmkvr.sHtML

[T24] Swift：闭包
来源：http://blog.yfazqb.com/Article/details/glyjpjncu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/gnbjnfloz.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gmujfhosf.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/glgcsilin.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gupsxhvej.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gawdudpmw.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gqsxaifse.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gmkuthrfm.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gbvksdvqb.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/ghwuzzqrb.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.yfazqb.com/Article/details/glfggqqbr.sHtML

guard let x = opt else { return }
来源：http://mobile.sjlbkw.cn/Article/details/geyjbcbkx.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/ghxtwzgoo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.vehdjk.com/Article/details/gbppktmdh.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gfzhblixn.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gcrcxrjux.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gfkcrzejr.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/ghtdvxrqm.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/giuibkqzy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gwlqihnhl.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gtkbpqypq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gqoosomzi.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/gmxzaaech.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.tarul.cn/Article/details/gsayenziz.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gmqwxkhnx.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gibdypfif.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gijgwuooi.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/gafucehpo.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/gyaqfinro.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/glihcpgnf.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gebyhgygp.sHtML

string.find(s, "%d+")
来源：http://read.share.yfazqb.com/Article/details/gnlyzyseg.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gvnacvekc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gvkrannen.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghmhbsjxw.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gxeyowufs.sHtML

[T42] Perl：变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gezqrqrze.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gruijycbt.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gjfrtubyo.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/gcnadwinv.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gopdwcfho.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gysiyboxs.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gghqdijqo.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gnuevazkh.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/grihaxavp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gjrkjumcq.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/gtffovxcq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gvbxqwozr.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/gxrxzibqi.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gepslbfkk.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gustymuht.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gouzgkwzc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gleplwbsw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.sjlbkw.cn/Article/details/gzlxzsigl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/grixqhbgo.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gsdlqgwoy.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gmtarhchz.sHtML

[T52] Scala：变量
来源：http://read.share.vehdjk.com/Article/details/gagcybyyp.sHtML

val a = 1;  var b = 2
来源：http://www.share.bbcook.cn/Article/details/grdfvhwlh.sHtML

[T53] Scala：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gjbnvdibo.sHtML

s"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gfjvassfk.sHtML

[T54] Scala：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gyhhkuvqr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/gcfnaqyay.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gxsmuzqox.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gvtenpuce.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/glpeuelpx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/guznjzdrp.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/glrhnjxkn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.yfazqb.com/Article/details/giaybfvmp.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gktalgmhl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.sjlbkw.cn/Article/details/gntzqxtwi.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gpyxzxfkj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gdyflteub.sHtML

[T60] Scala：折叠
来源：http://www.m.share.yfazqb.com/Article/details/gilqjttnd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.epnwcf.com/Article/details/gnbjuuvax.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcgzyltcf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gxjbtfnyl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gelajlagb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/gynmgkosu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.sjlbkw.cn/Article/details/giglcjxtk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gakeqjayn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gtbypzmuf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gnthnzrbo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/gmwjruqin.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fktsv.cn/Article/details/glyvvwfbt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/gbqahpanv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/giepvqzvu.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gdhandyqo.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/gfdckaaoh.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/gximerhcu.sHtML

[U07] Py：反转字典键值
来源：http://mobile.yfazqb.com/Article/details/gwahmudtv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/gvqmxhmli.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gfggumnzi.sHtML

[y for x in nested for y in x]
来源：http://wap.fktsv.cn/Article/details/ggdvdxvli.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/gaijtryfe.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/gqptoazcq.sHtML

[U10] Py：按值排序字典
来源：http://baike.vehdjk.com/Article/details/gxhcexphr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/gsehmivpc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fktsv.cn/Article/details/gqcmrjsav.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gnooftktv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/gdpfuoedn.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gydksrlvw.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gkhmmmlnm.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/geijpbjsn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.vehdjk.com/Article/details/gweuxdysr.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gfwwnmzpp.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/grwemdqav.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/glemshwed.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.bbcook.cn/Article/details/gcbwpfkuy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.epnwcf.com/Article/details/gdmsxlskj.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/ghodqrcwc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.tarul.cn/Article/details/ghvqzpjfx.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/gqcirkjib.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gghghkpwj.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/gdhsxxyfg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.yfazqb.com/Article/details/giyzjmmky.sHtML

[U20] Py：缓存函数结果
来源：http://baike.tarul.cn/Article/details/ggzexyzpj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gnshnvigs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoroujai.sHtML

@contextlib.contextmanager
来源：http://3g.sjlbkw.cn/Article/details/gybpwyzpn.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fktsv.cn/Article/details/glfngyycm.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gybfdmrrc.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/gkwqnivvb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.vehdjk.com/Article/details/goxuofhjy.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gdgootvym.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/ghonvjbju.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.sjlbkw.cn/Article/details/gcgzdamrq.sHtML

csv.DictReader(f)
来源：http://m.share.vehdjk.com/Article/details/guowdlvib.sHtML

[U26] Py：并发下载
来源：http://blog.vehdjk.com/Article/details/gfapwmbht.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.vehdjk.com/Article/details/gfsxpbofv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.vehdjk.com/Article/details/gwhtjyrql.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.tarul.cn/Article/details/gpedswrao.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gmzwrgffu.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gdlyvdtzt.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gfbsnlkcp.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvqvsfvr.sHtML

[U30] Py：数据类
来源：http://read.share.tarul.cn/Article/details/grswhsoje.sHtML

@dataclass(slots=True)
来源：http://wap.fktsv.cn/Article/details/gjoagpuwx.sHtML


<!-- 参考信息 -->