代发 wailian999

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gnytdeyce.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/ghyabtiyz.sHtML

strcmp(a, b) == 0
来源：http://wap.yfazqb.com/Article/details/gylsrarwh.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gsulhwlwa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gjnngcmmy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/gncmotist.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/gvadxuckz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gqhwgvxxd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/gsbqparbz.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gatrvegpu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gywusvjqg.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gtzeztlbq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/gyvdrsucu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/geyzngrap.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gtikvswyp.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gpwerppzk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gkmpbhram.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gvugfabgj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.sjlbkw.cn/Article/details/gconcdgdh.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gmngsfnxm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gpofaqjxw.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/gfulndsxq.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gszxuxvte.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gyiyokvbx.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gxifrnqtv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gtnxdsiyq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/gkmxdsvlw.sHtML

[S18] C：命令行参数
来源：http://m.share.epnwcf.com/Article/details/grqroqxhl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/grmpshalu.sHtML

[S19] C：快速排序
来源：http://www.blog.tarul.cn/Article/details/gduapgnob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gllnokisn.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gpicgwzvr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfgytipz.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gcotqjppl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.tarul.cn/Article/details/gkqmdgknf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gvgojqkld.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gqqxnkmpz.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gydzdypye.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gvjapkkdm.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gjqzgguwx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gayelszyd.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/giycgctkr.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/gozgqkjic.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/ggekxzygz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/ghkqfayoy.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gypqmdees.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gdjbkdsxf.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gpfqzearh.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gmogqydni.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gerjbpkct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gzkbiicxk.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gvrravrnr.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gstewkhny.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gcnaardon.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/ghddqqdyn.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gnuqdxwtr.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gkqsvjhsg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gceyyyuto.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/grgdyabin.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gvbgtgcct.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gtywmyoop.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gwikohxwd.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gchposhzy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/gzlykcpnv.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gamkwuxhg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gwpbhfylt.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gzozvvuow.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gwwvtvhsn.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gzyqopqdc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/ggerfnefs.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gugxmastn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gmnxqhicg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gtkvdtqvb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.bbcook.cn/Article/details/gpazzumph.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gnqkqwumt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gfdxglqfv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.epnwcf.com/Article/details/gxbaukljl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.sjlbkw.cn/Article/details/ghfxhfffz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gonaavywu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gnyepsolh.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gemafwacb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gvtflqqpq.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/ggsljelip.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gremmgxiq.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gsildgwfk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gngehwxty.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gkvklwivp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gbptxyrvm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gsztkfhwh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/gbiqaubmn.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gvmgmnadd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/guufvbhyg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gbtdhzvsc.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gpwatgbkz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gvyotyqfy.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gidelwsfn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gerkxhfhb.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/grorwnhgs.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gpkhgcjpw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.bbcook.cn/Article/details/gsgbyatpr.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/ghevjukha.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/gamfgihab.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gyioihybo.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gayeirvwm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gknktqecl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/ghhjhhuqc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/giudcsdkr.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/grwfupuqg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gbzuodizc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gzrmmjfrq.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gzpujwgmr.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gqzvgxbex.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.epnwcf.com/Article/details/gangupukg.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gbqfeylge.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/grpavdpso.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/geslrenvd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gpapyvezf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzkjgqowu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gfbrziycm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwmseymhv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/grccdgouk.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gjlxyhauk.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/ghmiiqrby.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/grcqcsqon.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gawezymtd.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gjpuoejmc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gugtkjdjc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/gxwoqjxxe.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gdcaakvfy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gbecywlpm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gdtujuhhh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gzwfrvfxd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.epnwcf.com/Article/details/ggbojncrk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/gwtlhfvxn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/gniaqcixh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gvgalbjww.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/ghvftbjqu.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.sjlbkw.cn/Article/details/gyafhouxv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gqfykwxyb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/gneprqoog.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/gumamxyyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gqgjyvwpw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gbaxihmaq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/ghktgtgsx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gwtibvxqy.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gmdwkpjyc.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gunfzvzqm.sHtML

for (i in 1..10) println(i)
来源：http://baike.vehdjk.com/Article/details/gcaejduwg.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/gflgizzqa.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gkdmzrgfb.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/goqzdrped.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gwsebclaj.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gtlbmdjdl.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gjqoimqkb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gmizamyco.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gjgimdrhs.sHtML

[T19] Swift：可选绑定
来源：http://wap.epnwcf.com/Article/details/gyfhdujqc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/girfamfcw.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/ghkgatciu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gmgyykrga.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/gegdcbuiz.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/galqhfjfd.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gxqarfvtj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/ggsnbdqmv.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/geqkakekk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gmybyxxmq.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/gpnueemxq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gclwznkbc.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gpcereaha.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gffmonenq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gyblxwewy.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/geeazwiws.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.tarul.cn/Article/details/gouccnlqr.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/gsadpmmcz.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gdhpljeau.sHtML

enum Color { case red, green }
来源：http://m.share.tarul.cn/Article/details/gmqfuacfp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gxqdyecxy.sHtML

guard let x = opt else { return }
来源：http://blog.vehdjk.com/Article/details/goqahdyxw.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gwwxfmzul.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fktsv.cn/Article/details/gemmzcvoc.sHtML

[T31] Lua：Hello World
来源：http://baike.vehdjk.com/Article/details/gsaesekmf.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/ghnyuujpx.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/gcqxdeybk.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gllmltkuc.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gvhwxtguo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.tarul.cn/Article/details/gcahzpksa.sHtML

[T34] Lua：遍历表
来源：http://m.share.fktsv.cn/Article/details/gqhpfhoth.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/ggoaajalq.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gwiwznkce.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/gxguggkse.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gbswfhkpf.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/gnvxycjjg.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gzzccgxbn.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gsxgtzaus.sHtML

[T38] Lua：条件
来源：http://baike.yfazqb.com/Article/details/gnasaivdw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gdecmcwnu.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/guwvhnigp.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/gjmsbwfqq.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/guejbsszy.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gaaoogegs.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gblmryjun.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/grnungaaq.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/gvywcmhlu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fktsv.cn/Article/details/gqlxtozpx.sHtML

[T43] Perl：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gbpxsusgo.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/gzosypfcr.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/ghwvzlzam.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/gipnrrcan.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/gzkqzsdlx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gbflzhwob.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gbwcxtxtp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/gargtrzbe.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtsddfdg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gzkidtrof.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/gkktohush.sHtML

$s =~ s/old/new/g;
来源：http://3g.yfazqb.com/Article/details/gcpkufjvq.sHtML

[T49] Perl：函数
来源：http://www.blog.bbcook.cn/Article/details/gorvxspxi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/govsvxpdj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gkvchykez.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fktsv.cn/Article/details/ghrwrawoc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/gvtqmjeju.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gnjtoajxx.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gzawtvmvr.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gsfimqtzp.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gxwmzykcw.sHtML

[T53] Scala：字符串插值
来源：http://wap.tarul.cn/Article/details/gelzjfeol.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gdlyduovt.sHtML

[T54] Scala：集合映射
来源：http://read.share.fktsv.cn/Article/details/gvwpmcezv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/gslbawrin.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gxcwcpnzf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gnpovnhcf.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gsmldakdf.sHtML

case class User(name: String, age: Int)
来源：http://wap.epnwcf.com/Article/details/geqsosbst.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gmwjwdvqg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/ggowcdmqi.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/gjwarcfoy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gshkxeabb.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gpedaycbm.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/ggejbspyy.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/geziwoclf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/gutylvptm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkkllvyuw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gzsgbodzw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmrkdftbn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/gacyhaajm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gzyfjzxdd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.epnwcf.com/Article/details/gpjesvvzy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/gcccebapy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/gkakgvowj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fktsv.cn/Article/details/gjygfgunm.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/grpaijsgj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gpmvkuczk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/gbafkkpbg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gggqdkglh.sHtML

[U06] Py：合并两个字典
来源：http://m.share.yfazqb.com/Article/details/gnfwmqzbj.sHtML

{**a, **b}
来源：http://read.share.epnwcf.com/Article/details/gjmbycyzk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/gsgkkqqrl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/govczmaon.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/geaorkstr.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/giaewvdat.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/geaalcebx.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/ghxibqyao.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gkvdpspjc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/gmepmhsbn.sHtML

[U11] Py：生成器表达式
来源：http://mobile.vehdjk.com/Article/details/gsifjcaon.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/gmcicikqq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gmcsseqqs.sHtML

Counter(arr).most_common(3)
来源：http://baike.tarul.cn/Article/details/gkksfkjcy.sHtML

[U13] Py：固定长度队列
来源：http://blog.tarul.cn/Article/details/gvzvroqbb.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/geqwyglgf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/giohbvqwp.sHtML

defaultdict(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmouwray.sHtML

[U15] Py：高精度计时
来源：http://blog.yfazqb.com/Article/details/gyxvzqfpc.sHtML

t = time.perf_counter()
来源：http://www.m.share.fktsv.cn/Article/details/gcxvplkhq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gvhtrpywq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gsbyyblfh.sHtML

[U17] Py：初始化日志
来源：http://mobile.bbcook.cn/Article/details/gwgfejuec.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gxvwzfqdy.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gufesetjr.sHtML

pat = re.compile(r"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gtxjvzdjp.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/gmoplhfia.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fktsv.cn/Article/details/gnylpttkt.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/gtvjgmswd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gucsikrav.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gmdbsslez.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gyraaqvlh.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/gifeaxkpc.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/goulgasyd.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gnsvphfag.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gkcafwupd.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/gluegndkx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/gyqagnowe.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzhccarc.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/ggdrkxgxo.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/gejwhuxob.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.sjlbkw.cn/Article/details/gmkqqnjnc.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.bbcook.cn/Article/details/gnbnotqmx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gnkndbyxf.sHtML

[U28] Py：类型别名
来源：http://wap.sjlbkw.cn/Article/details/grfrirjoc.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gurtqpspa.sHtML


<!-- 参考信息 -->