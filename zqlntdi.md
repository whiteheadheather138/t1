代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/grdfdlzmb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/gkeuezjlt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/ggdcsapeo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gyzmulojh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gzpywblnc.sHtML

[S10] C：指针与解引用
来源：http://wap.yfazqb.com/Article/details/gotzmbtoa.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gnclxtljm.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gmzzvuzyf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/gxgfbugti.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gjguzuotl.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gldryioks.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gvszdhikz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gtnfaklil.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/gykhdgduq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/gfqhhbhfl.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/gqruaxlum.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/ghbasgyni.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/grtduoiyc.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gztwfjobq.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gpkmjpnbf.sHtML

x |= (1 << 3);
来源：http://www.share.tarul.cn/Article/details/gqynqjibb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gwomdadnl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/grxjpqfwa.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gvfnybysu.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/ggqpmzniy.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/gddlbmjhj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/givwvhzzb.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gzgoidzpk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/glddwlkod.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gtsukbpxv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gcexvrwjr.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gzusciltp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/goamrjuzt.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/grkjdomsv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gyfqpbaqo.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/grjuhdwik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/grwjxepon.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gujlfldiy.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/gfdwhlvfd.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gsaggvqen.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.epnwcf.com/Article/details/gvfqutiij.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gwycusyuw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gnngkqnkc.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gpgihbqzj.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gkbhdpmud.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gzkspymrm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gmkgllzkz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gysvgsrws.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gluxfgcgl.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gddiqcwnu.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/guyealtdz.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gxcumgeew.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gmmeypkag.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gglvioxjd.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gruiustky.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/ghmfcduzo.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gqjlmwuox.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fktsv.cn/Article/details/gcneadcka.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gusrvanmv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gyirjxhct.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gkczejbgf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gvpohfrbb.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/grewjaukd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gexccfgkp.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/gcjgpujve.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/glcaezlsv.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gpuzwzuvg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gefuzvmhs.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gsmevtsmx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/gsmqhnfkp.sHtML

[S40] C++：查找元素
来源：http://www.share.tarul.cn/Article/details/gnllzfufk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.epnwcf.com/Article/details/ggqdvgzlp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/grkekmfbt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gajhrcisg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gaqblsbxm.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fktsv.cn/Article/details/gotjgytvr.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gheiwuqfa.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/gcghtzmcx.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/geocowdjz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gbkyycdmy.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gnfksyuoy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/gwgisbumr.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gcxsyfibz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gltvnojmr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gezjzwcxm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gpsqbktbk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gzwkcqcxh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gmvypvdlq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gvyeymkon.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gbugddoph.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gomtfhogd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gyzziadbk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/grsmewxfx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gkuwqkkkt.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gdrcebvwn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/gdkmwxjua.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/grwopybxx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuluanrc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gkfglvzlk.sHtML

[S54] C++：异常处理
来源：http://baike.fktsv.cn/Article/details/gwgjvbcdw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gtbzumulk.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gnhhrafhh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gzjbnkvwd.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gaoqesbdz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gktiirfpt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gliqosaav.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gzralfxnf.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gvwvfyojj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/guerbmcws.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/ggkgvpalv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/giqnxhmui.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gybhnujzn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gxiweujaz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwaptvvmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/ghwwbxkoo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gymxqxjba.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gewnhtxxg.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/ghbxwjmtf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.epnwcf.com/Article/details/gtffpgaji.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/guobqzdpv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.sjlbkw.cn/Article/details/gykkznmmd.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gluavhyfm.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/gxwsgnmjk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/grnfwiykx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhnxfuna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.epnwcf.com/Article/details/gwdzzough.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gxtfppmzo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.yfazqb.com/Article/details/gkhntuzhu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gkozjmknw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gbyzlygqb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gkixppfsv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gtykisgjt.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/grehajdvc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gttnrzbwb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gulixaojm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/goqxshsbw.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gbdpfxyhf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/gsdiwsvtv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/ghtskyexz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gubnzspdc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/ghwujdpnp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gaujyszkq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gwkdephrt.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gfhrmxeop.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gonlfmgxe.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/gbuhjtpgh.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/glasysftn.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gangxuukt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gnzyogevy.sHtML

var a = 1;  let b = 2
来源：http://baike.yfazqb.com/Article/details/gkimlrbub.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gpahirgas.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gnwfkinde.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/goazdbuur.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/geqehjvek.sHtML

[T20] Swift：数组操作
来源：http://blog.vehdjk.com/Article/details/gcddrkgid.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/glolucozb.sHtML

[T21] Swift：遍历
来源：http://m.share.fktsv.cn/Article/details/glqlqyhfc.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gymgfhqxv.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/gbqtumdsi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gdubbblqp.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gywotspwr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gdahqlylg.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gejcchjwy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gnmxlztdy.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/gqajllvud.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gfjccwpmt.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gfhuprtsn.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/ghnooroty.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gfaroklaf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gygngupga.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gxgdrbzsv.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gwfbgpnna.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gifneyoyq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsiyznnl.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/gnhhrfbeo.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.sjlbkw.cn/Article/details/gnijpmodt.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/geujwsbmc.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gngbrwqis.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gaukdkheg.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/guhjwqsvy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.epnwcf.com/Article/details/gzikcevoy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.epnwcf.com/Article/details/gajeqffje.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gqgxfsnwq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gsljzmvzu.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/gcsbblhnm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.yfazqb.com/Article/details/galmxypbz.sHtML

[T36] Lua：函数
来源：http://www.share.fktsv.cn/Article/details/gdtcunhex.sHtML

function add(a, b) return a + b end
来源：http://m.share.bbcook.cn/Article/details/gumuogfve.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gklvjfvoe.sHtML

"a" .. "b"
来源：http://blog.tarul.cn/Article/details/ghghfyuss.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/ghxlvegxu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.bbcook.cn/Article/details/gsjftqtqn.sHtML

[T39] Lua：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gywcwyxuy.sHtML

string.find(s, "%d+")
来源：http://www.share.tarul.cn/Article/details/gsbtdopbh.sHtML

[T40] Lua：元表
来源：http://www.m.share.vehdjk.com/Article/details/glllydhij.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/geldbwgqg.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gkmpeufwp.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/gfhhaecfh.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gnvrjpbel.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.sjlbkw.cn/Article/details/gpuyrymwb.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gzxebfytv.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gunwgwfvf.sHtML

[T44] Perl：条件
来源：http://www.blog.fktsv.cn/Article/details/geepislvy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/gcnogwrvy.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gzjvnbioz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.vehdjk.com/Article/details/gcocsgqmn.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/gjluogyaa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfvodpfaw.sHtML

[T47] Perl：正则捕获
来源：http://m.share.epnwcf.com/Article/details/gcdqzjabg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/guypmyshf.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/glvvcskge.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gmchzcwpi.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/gyigqolip.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/godxawitc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/glpotpxkg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.epnwcf.com/Article/details/gmkkjwdfc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.bbcook.cn/Article/details/giibtbklc.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gprcrcxze.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gtkzlenbi.sHtML

[T52] Scala：变量
来源：http://blog.sjlbkw.cn/Article/details/gsdnuqeru.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gzgcsrvkz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.vehdjk.com/Article/details/geyjgeexq.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gkzksvfgz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gciwpqogq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.yfazqb.com/Article/details/gsbcqkjwq.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gtuknhdju.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/gsblfjbks.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/gnlcsgxgw.sHtML

case class User(name: String, age: Int)
来源：http://wap.bbcook.cn/Article/details/gekijqjcd.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gkjeztdpc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/gafknrlpx.sHtML

[T58] Scala：函数定义
来源：http://m.share.yfazqb.com/Article/details/gqslxvwcf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/glzhxrotn.sHtML

[T59] Scala：循环
来源：http://baike.sjlbkw.cn/Article/details/ghqlurccc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gcbfpyeie.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gecpxqqjt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/gytvqldco.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glnqfkhuz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/grumvgbvd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqkmshrde.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gvcccpglb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/gcldyjqdq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/guiucdfmx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/ghtagvouj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/ghywclztp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gvysthpjk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gxnbzapmy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.bbcook.cn/Article/details/gdiugkaxs.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gbfiqrdnc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gjvaujqsz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gligivtvs.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/gaibvcoot.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/ggkzxetun.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/glugzwcak.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gpyvjdkcb.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gybykyzmt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.vehdjk.com/Article/details/gcayvonak.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/guecsucsd.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gbfkzvrun.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/gqosueahr.sHtML

[U11] Py：生成器表达式
来源：http://read.share.vehdjk.com/Article/details/gngheotty.sHtML

(x * 2 for x in arr)
来源：http://blog.tarul.cn/Article/details/grqfthkhq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.vehdjk.com/Article/details/grddqxcdi.sHtML

Counter(arr).most_common(3)
来源：http://mobile.yfazqb.com/Article/details/gjnxkrkps.sHtML

[U13] Py：固定长度队列
来源：http://read.share.tarul.cn/Article/details/giblvqbin.sHtML

deque(maxlen=10)
来源：http://read.share.epnwcf.com/Article/details/gyfhpploa.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/guvusvhgs.sHtML

defaultdict(list)
来源：http://3g.epnwcf.com/Article/details/gdhouiafx.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gfxpbwmff.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gxrxjibxm.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gsklyltmd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.vehdjk.com/Article/details/gujgfnxcz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.bbcook.cn/Article/details/gdaxjmjqf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.epnwcf.com/Article/details/glkkgyzko.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/gtklafqph.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/gbiezofpw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gmcwzlkgj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.tarul.cn/Article/details/gimcqvdgn.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.yfazqb.com/Article/details/gbbgibjdf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.vehdjk.com/Article/details/gwlvcrujj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gbbdhcrds.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/gweqqeymd.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/gsafduwhw.sHtML

list(zip(*m))
来源：http://www.m.share.yfazqb.com/Article/details/gnogrwdbd.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/ghoihycfm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/gnnjiclfd.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gbdcduvdu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/gsaijjdud.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.tarul.cn/Article/details/gcuanwkqn.sHtML

csv.DictReader(f)
来源：http://mobile.bbcook.cn/Article/details/gvlewkmrz.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gtopbtsfb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.bbcook.cn/Article/details/gikrdmcin.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/geagszaqw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/godwrrylp.sHtML

[U28] Py：类型别名
来源：http://www.share.yfazqb.com/Article/details/gyeqliyzt.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gcosnsdzc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/gogmgfbbu.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.epnwcf.com/Article/details/gmafplpql.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/glxtrpzux.sHtML

@dataclass(slots=True)
来源：http://m.share.vehdjk.com/Article/details/guolcfdti.sHtML


<!-- 参考信息 -->