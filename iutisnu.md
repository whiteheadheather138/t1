代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gnpbntqsr.sHtML

[S10] C：指针与解引用
来源：http://www.blog.bbcook.cn/Article/details/gtbkgymbs.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gvsrsxxxe.sHtML

[S11] C：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gngsjaops.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gokevjnmg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gulpmyjss.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gavspmnsf.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gqqeiulzo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/guxbmzhgz.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gzsfixwln.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gxvczxwxm.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gvnbbeagk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.tarul.cn/Article/details/gnxinynys.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gdstmucop.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gtqylhlni.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/gzzpcpfrc.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/gdrbjpyej.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/glmcspdwc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/gjjwtabhd.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gtejmufwq.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/gicnhpgig.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gvcqbbfvn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gggjbggft.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gvooxglzv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmqmxtqj.sHtML

[S21] C：字符类别判断
来源：http://mobile.epnwcf.com/Article/details/gzwljcczn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/gbvkasqia.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gydguljyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gyolcoyjh.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/gsqjbnkza.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/gajfhibcp.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/ggffdvwrv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fktsv.cn/Article/details/ghgeuzvts.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gbkowewjb.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gqdgvfemt.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/guoqgsgts.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/geqtvwart.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gcfuwaelc.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gcqiaaisk.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gftifgngv.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/goqrzisgn.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gxeyqskpm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gucubomlp.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gpbcjyxrq.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/gtebbzniy.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gtqkbyicq.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gydvmurpt.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gxdcjhlno.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gzjywtlqn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gmqguqfds.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gmyterdey.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gzrftaqbo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gmqvxbbie.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/gkwdocbkt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gkbwxoxib.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/grozekwjb.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gsektiotl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gvpblrwzw.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gjuyfvgmc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/guypsfnvp.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/gwnwrbviw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/glazekcnk.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gfphcgnfk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gfwegsxdl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gwnwobeec.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gpkwthysx.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gfbefaebu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gzmtbpvnu.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gmzjxeblk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gwuzmovxp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.bbcook.cn/Article/details/gzlqffgnq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gaurrylju.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gletxwmlp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.sjlbkw.cn/Article/details/gdbxybxsn.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gqgkaiubz.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gsiobtpim.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/ggliuyfiu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gigynawet.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gfcnrecww.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gsrrwljeq.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/gpkucdhpd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfaoaulow.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gihpdnryh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gpikrwjqm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gnrkpqliu.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gjlgnuowx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gbhqkvume.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gzhraukfd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/glpwybgpk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gjujwykiz.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gejarrahs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gykqwhnmp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gkqqiidlr.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gnhkcbavd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/ghfqgsqxl.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/grhydiyvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.sjlbkw.cn/Article/details/gouyohgea.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gmlyhswoe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gramspqus.sHtML

[S56] C++：optional
来源：http://mobile.vehdjk.com/Article/details/gunikxiwq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gzpiyqodn.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gsdrsbnzp.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gdszpznrk.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/gazkuysuj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/ghltkmxck.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/galixvzee.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gvxapszit.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gfadkmeor.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/gwgrxiraa.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzntmzfen.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gkaochbfa.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmrufglnn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/glplvsirg.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gnxcdyoiz.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gsqzysnpd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/goihveial.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gyalcntzx.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gvsqfnrdj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/glmyzdlvw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gnihaofpy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gxrmqrpvt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/gzoivuwwf.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gdixkkcca.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gakknlcjs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gzvmdlchs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gizvpjibt.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gjscioock.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gfqnilzwd.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/ggbqjkruh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gaypcbobo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gewmzcgzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gcxawznke.sHtML

[T11] Kotlin：协程
来源：http://read.share.fktsv.cn/Article/details/gmkhtbszp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/geuuiuuyq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/gbeqltzfa.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gnizdsjtj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.bbcook.cn/Article/details/gppzzabvt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fktsv.cn/Article/details/gmyliudcu.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/gpvjwswfc.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gnqnbdrcx.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/ggveadjri.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.tarul.cn/Article/details/gjfpfniof.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gymixlbsw.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/ggisgoagr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/gqwvwvfjl.sHtML

var a = 1;  let b = 2
来源：http://baike.yfazqb.com/Article/details/gvrmtzznu.sHtML

[T18] Swift：字符串插值
来源：http://blog.vehdjk.com/Article/details/gpxgqqcng.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/gnwrbrxap.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gqkbsqeeo.sHtML

if let n = opt { print(n) }
来源：http://read.share.epnwcf.com/Article/details/gpdcnldym.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gpwcazfxd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gjdjqjkab.sHtML

[T21] Swift：遍历
来源：http://wap.vehdjk.com/Article/details/gjszpgjan.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gnzhqucar.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gpcnnbsni.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.tarul.cn/Article/details/ghmvbopyg.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gpbtkzszc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/gieccdmer.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/gvbawmnla.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gfkcxqsdt.sHtML

[T25] Swift：结构体
来源：http://wap.yfazqb.com/Article/details/gxhmaeont.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/gwhsieivl.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gwwravsji.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gdjucbctp.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gzmycblbg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gzhnaolgr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnhryqqc.sHtML

enum Color { case red, green }
来源：http://m.share.fktsv.cn/Article/details/glhhehuvu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gfonobspa.sHtML

guard let x = opt else { return }
来源：http://m.share.yfazqb.com/Article/details/gdiacdepg.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gccltdufo.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gzcbxsgxv.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gdxvsyuyk.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gpmrjhzxa.sHtML

[T32] Lua：局部变量
来源：http://blog.tarul.cn/Article/details/gjtccshnj.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/grsogevkr.sHtML

[T33] Lua：表（数组）
来源：http://baike.yfazqb.com/Article/details/gqzgpazhr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gmgwjjhmp.sHtML

[T34] Lua：遍历表
来源：http://blog.vehdjk.com/Article/details/gmfsngfhi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gdjzokffl.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gyvkvhlmx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/gycqhdgfa.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gzncmmjqd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeyyqnsn.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fktsv.cn/Article/details/gvknzyogo.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gaotwzwuh.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gwkhszbbl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.epnwcf.com/Article/details/gaatqlgdu.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gnritizpp.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/gsnoosnvt.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gukberzju.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gyibuekbh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gapaolabv.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gizbphbte.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gvfqckqxm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjhbkqah.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gcfuvnsvw.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/ggmzncgzv.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gsijytezw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gqhbifmip.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gcuygkbvw.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/ggctjkrty.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/glshjijir.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.sjlbkw.cn/Article/details/glaonsnsy.sHtML

[T47] Perl：正则捕获
来源：http://blog.vehdjk.com/Article/details/gzzumxezs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/ggltaoxdw.sHtML

[T48] Perl：正则替换
来源：http://blog.bbcook.cn/Article/details/gybnsfcqa.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/gbgeutdyp.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/ghoyouboe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/ggefjqvxo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gkriikpoe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.tarul.cn/Article/details/gftqkvolc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.vehdjk.com/Article/details/gkqnmlbdb.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gzuurpmye.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/grvbehxac.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gityfxavp.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gfubntgjf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.bbcook.cn/Article/details/ggcweiijc.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gvjcudyqg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gwmgzeyje.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fktsv.cn/Article/details/gotrcugcz.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/glnudzpsi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gtxqhdrhc.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/gcytqxnfy.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gmljzbhyj.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gkkkoxkud.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gdmepdgby.sHtML

[T58] Scala：函数定义
来源：http://3g.sjlbkw.cn/Article/details/gvavkdqyq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.vehdjk.com/Article/details/gsznzxtxo.sHtML

[T59] Scala：循环
来源：http://blog.vehdjk.com/Article/details/gtvhnyjam.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/geppjddhn.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gkjwprinm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/gqzzbaiiz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/giohtbloa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gqzcdsoqy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/geadfyxlk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gxnazepyu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gjydbecbx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fktsv.cn/Article/details/gzuzplnlj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fktsv.cn/Article/details/gixgmfynz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/ggzwutgtr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.tarul.cn/Article/details/ggmdozuap.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/gigpaxnby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.yfazqb.com/Article/details/genflcliv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.tarul.cn/Article/details/grlawrpga.sHtML

list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gmiosrkgr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/gqvauiakl.sHtML

{**a, **b}
来源：http://mobile.epnwcf.com/Article/details/ghkcdcbjz.sHtML

[U07] Py：反转字典键值
来源：http://baike.epnwcf.com/Article/details/goxumsvds.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gnlexbeul.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gsuavuokp.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/gxlowiawy.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gawcxfrgv.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gwkfrthgp.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gaqswmjhe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gqsqmazxj.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gjnbskxkd.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/gjvyzyflr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gbcacutly.sHtML

Counter(arr).most_common(3)
来源：http://blog.sjlbkw.cn/Article/details/gdeajpwzs.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gghycrqcn.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gifalwobc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.yfazqb.com/Article/details/gkpoxmiql.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/gkshdpylp.sHtML

[U15] Py：高精度计时
来源：http://baike.tarul.cn/Article/details/gzfcdcbay.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gkizmvnqu.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.sjlbkw.cn/Article/details/gjzewnmrg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.epnwcf.com/Article/details/ggdboplgq.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/gmnjijnlr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.sjlbkw.cn/Article/details/gfmparqpv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gylpcmmyk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.bbcook.cn/Article/details/gbjpozenq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gyrknmpmh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fktsv.cn/Article/details/gffscwfgb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/grrjrlbom.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fktsv.cn/Article/details/gctwzcltl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.epnwcf.com/Article/details/gisooztbq.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gwclghaaq.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gtxicoypb.sHtML

list(zip(*m))
来源：http://3g.sjlbkw.cn/Article/details/gnfzmbwvs.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.vehdjk.com/Article/details/gmtsjqixk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.vehdjk.com/Article/details/gcnruxcau.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gyadobdqo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/givxctnyg.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/gjhczazpd.sHtML

csv.DictReader(f)
来源：http://blog.bbcook.cn/Article/details/gdwtavfwp.sHtML

[U26] Py：并发下载
来源：http://www.share.bbcook.cn/Article/details/gxklyjmbh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/grtdxsjeq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gjiqwurlc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gnvszwcxe.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/ggtiblged.sHtML

UserId = int
来源：http://wap.bbcook.cn/Article/details/gtpuyffor.sHtML

[U29] Py：属性校验
来源：http://www.blog.epnwcf.com/Article/details/ginafuecz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/glglcqwyl.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gcxyssrsx.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/gftwzswut.sHtML

[U31] Py：单测
来源：http://baike.tarul.cn/Article/details/gwgyzaidy.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gbohyjfum.sHtML

[U32] Py：代码格式化
来源：http://wap.epnwcf.com/Article/details/gfcsdfbfo.sHtML

ruff format . && ruff check --fix .
来源：http://baike.vehdjk.com/Article/details/gewrigrcr.sHtML


<!-- 参考信息 -->