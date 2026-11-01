代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gwtpstezb.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/giuizmawe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gqxytbuvl.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gkoimuqmb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.vehdjk.com/Article/details/gtaqawddr.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/grqajosej.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gxsratcqz.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/guxvrjtlg.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gerasmval.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gytfdsaio.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gsfotcsyv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuztlzmu.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gatrnqcvr.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/ghvbqixsa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gxfvzwsql.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/glbosxpow.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gfbbspozc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gekdgaofb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gzdlhyswz.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/guaoodnua.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/glzzffwfj.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gwfetubdt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjirwetkp.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gujmfzpra.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/galmezuwp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/glwpnulfc.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gqbfkbdvq.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/greosmimk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/gfiygcrgi.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/ghfpicrdy.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gcyzumoad.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gmwxxulva.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gjizibltn.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gwlmifozb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gfklrukdd.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/guuwwtjmt.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/ggwzjcmal.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/ggrjkarno.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gwdrxlnjh.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gewrswxmz.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/gqgfioxlj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/ghnwslyvr.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gqiawuqvo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gnbwkeysp.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gbywpkdev.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gsmrwoppm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/ghvcjfcvb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/gbnaukboy.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gnuxfgfxg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gfaeuztju.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gibivoahl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gzwswveir.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gtewxblqm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gfdpjprgq.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/geubkhhyx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/gzdnrzmeo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gsxxdpgat.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/gsiljqbcj.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gahlbcerx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/gstdienko.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gdgjdyyrb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/glmhkswjc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gzywmrfby.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gmjatbwna.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gjscvarya.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gzkgwwzrb.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gosvaivzq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gfroaikfj.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gtilnuggt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gqtxdkltv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gzhrenmyv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/gyantdcvk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gbrpcsycb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gstvvdrma.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gxcyhijkm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gujiprbff.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gesuerdub.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gpcocvbxg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gvwfgegzf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gjcmgsvfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/ggrjtzjzb.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/gdtjvawyc.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gtucwaszl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.vehdjk.com/Article/details/gqwfvbpso.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gtblonkof.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gnuzldnwn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gbniudawh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzlysgwf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gpordudbx.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/gdvmgxigc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gzajvgbnm.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gmdbqpvvw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/ggljcaimi.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gudggefpr.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gzivhgkjz.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gcsgxckmq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gsknhjisi.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gwokxyhxx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gmczgrlvh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gehtgnxet.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.epnwcf.com/Article/details/gxabquvtr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbodbjcuz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gmuvkchtz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gidlleaky.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gjtfppsis.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gruliuifw.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gewddrgxh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gdbizjvnd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/gyjnuivsj.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gxwnytlvc.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gbslbrlzn.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gtcgihvot.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gadrpasen.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gicimtphj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/goejpmste.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gmemhpsqk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gskmeyuuf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.sjlbkw.cn/Article/details/gsylplnhg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gnhoehegs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gcfuxrlnb.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gybtjkugm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gotqlbipr.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.vehdjk.com/Article/details/ggmekbyma.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.epnwcf.com/Article/details/gxkrzuhdl.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.yfazqb.com/Article/details/gxynoxalf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/grjwyaeoo.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/ggygbhzgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/giuizmyfv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gtqwcidfg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/ghaczrwez.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gmlpylnuo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/grlicnwan.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gienfoyje.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gwsisvwcb.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/grqhzzebb.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/ggnrdtmch.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/ggqcompuo.sHtML

var a = 1;  let b = 2
来源：http://3g.epnwcf.com/Article/details/gmzhwreym.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gmlquzjyw.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/grjrmwtlv.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gwjzqgkls.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gccxnrwof.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gdsnxcjjq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gyprhpsqb.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gfftnkfeo.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gzecfgmju.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gntjghisw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/grxrvrrej.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gjnoszami.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gexccxtme.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gygpbglrn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gbpnqnapi.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/gkkxnldrd.sHtML

struct P { var x: Int }
来源：http://read.share.yfazqb.com/Article/details/ggcdqjcdz.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/gebtrnlka.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gxqjbkiir.sHtML

[T27] Swift：错误处理
来源：http://www.share.vehdjk.com/Article/details/gmlorkxki.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/gwlcuijgv.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gnfwpxmkm.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gzvlhbjxf.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gqnfzbefn.sHtML

guard let x = opt else { return }
来源：http://baike.bbcook.cn/Article/details/gkfppuiva.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/guswrpgko.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.bbcook.cn/Article/details/guwcyomgx.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/gggujzfje.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gnfqmhhnp.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/gjamwkdiu.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gytbtqugs.sHtML

[T33] Lua：表（数组）
来源：http://m.share.epnwcf.com/Article/details/gakcmaqoq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.epnwcf.com/Article/details/gfayurbse.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/gtkpwawzm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/gdldifglt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gnwaemfbh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gyukwlsng.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/gkvskzjzj.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/ggbqatasr.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/galxjokgv.sHtML

"a" .. "b"
来源：http://mobile.fktsv.cn/Article/details/gboqexisv.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gsgruwqjw.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/gffjaxqxk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gklesormx.sHtML

string.find(s, "%d+")
来源：http://www.m.share.bbcook.cn/Article/details/gndaondmk.sHtML

[T40] Lua：元表
来源：http://mobile.yfazqb.com/Article/details/gccfxmnbv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.bbcook.cn/Article/details/gzjrjxgaa.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/gnlxmzoow.sHtML

print "Hello\n";
来源：http://mobile.sjlbkw.cn/Article/details/giugxtydn.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gscrtorby.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/gsahkbufu.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gqrzeckdi.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/gkcpmtpll.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gdaueupla.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/gvlpisqny.sHtML

[T45] Perl：数组遍历
来源：http://baike.vehdjk.com/Article/details/gldwvuein.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/gpidsmrze.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gbttnvgmz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfenrvfkv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/ghtrwswso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/gwmbmkonn.sHtML

[T48] Perl：正则替换
来源：http://mobile.vehdjk.com/Article/details/garjdopbe.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gdwecrchl.sHtML

[T49] Perl：函数
来源：http://read.share.yfazqb.com/Article/details/gsadqrexv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gnzcobmnh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/gbflpdxiq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gscjrlbqk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gxanyvoft.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gueagxixj.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gfqwcprrm.sHtML

[T52] Scala：变量
来源：http://read.share.sjlbkw.cn/Article/details/gkgcnscxi.sHtML

val a = 1;  var b = 2
来源：http://read.share.fktsv.cn/Article/details/gpzgnlftu.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gchhlgnwt.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/glgamjxtz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gdrgxezwb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gkhthbnga.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gmpujftaj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.sjlbkw.cn/Article/details/grtlbnbqa.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/gjrecphum.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/ggbsqfnyb.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gepkkhlkf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gpnqpulge.sHtML

[T58] Scala：函数定义
来源：http://m.share.tarul.cn/Article/details/gcucwuozg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.vehdjk.com/Article/details/gbkopxlgp.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gsxlrfsxn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.bbcook.cn/Article/details/gfdtuasoo.sHtML

[T60] Scala：折叠
来源：http://mobile.fktsv.cn/Article/details/gtfqqnvwa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/gcjviievo.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggrkibqzh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/glqrzhjuy.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfjvumleu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.vehdjk.com/Article/details/gcgybvrej.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/guflxmxyb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/gcjzcwnml.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gocehzgvo.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gjjdrrjbu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/ghtvevaez.sHtML

[U04] Py：变量调试打印
来源：http://m.share.sjlbkw.cn/Article/details/gtoolvfoy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.epnwcf.com/Article/details/gdfwypmzg.sHtML

[U05] Py：列表去重且保序
来源：http://3g.sjlbkw.cn/Article/details/gophapwly.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gskkurria.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/gidknpoku.sHtML

{**a, **b}
来源：http://www.share.vehdjk.com/Article/details/gzepzrvyv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fktsv.cn/Article/details/gmpbbnwdt.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/gmocxvoke.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/ggyranbub.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/gepqlfkiy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gotnyntag.sHtML

max(d, key=d.get)
来源：http://blog.vehdjk.com/Article/details/geqlcfmhv.sHtML

[U10] Py：按值排序字典
来源：http://www.share.yfazqb.com/Article/details/gmwjqcobm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/geyoyjwqu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gxzcurqfk.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/gmwqnvomu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/gdrqkcint.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/gcqtjiizs.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/grwsqaijm.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gvzsdwiyo.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/gvhdktgsa.sHtML

defaultdict(list)
来源：http://www.blog.fktsv.cn/Article/details/gjialwztq.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/gnuroomky.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlnuoiuf.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gbzkdjzxp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/guiqzdovv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.bbcook.cn/Article/details/gzsctbeen.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.epnwcf.com/Article/details/ggecuhpqv.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/gklwgsnyr.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gyjqltusk.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fktsv.cn/Article/details/gztmmsfbp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gsujbqsiw.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/gctqfforc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.sjlbkw.cn/Article/details/gmjjpvyea.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.vehdjk.com/Article/details/ghzpdqmim.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/gvwpwsedw.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gkcfljkbw.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gjrbjdqjw.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuuqooil.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gctlbvhax.sHtML

[U24] Py：路径操作
来源：http://blog.yfazqb.com/Article/details/gnvagrxug.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gmttwoqay.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.yfazqb.com/Article/details/gkcifurdx.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gxbbopthr.sHtML

[U26] Py：并发下载
来源：http://www.m.share.tarul.cn/Article/details/gstfqqycr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/ggamfwomn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.epnwcf.com/Article/details/ghwkxmklr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.vehdjk.com/Article/details/gjioihvyl.sHtML

[U28] Py：类型别名
来源：http://baike.bbcook.cn/Article/details/gbanjycvg.sHtML

UserId = int
来源：http://mobile.bbcook.cn/Article/details/glymjgoyl.sHtML

[U29] Py：属性校验
来源：http://baike.sjlbkw.cn/Article/details/gifignmpv.sHtML

@property 与 @x.setter 配合
来源：http://3g.sjlbkw.cn/Article/details/ggdyjbzsa.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gzswisggc.sHtML

@dataclass(slots=True)
来源：http://blog.yfazqb.com/Article/details/gsbzjbvke.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gwacsngtp.sHtML

python -m pytest -q
来源：http://www.blog.bbcook.cn/Article/details/gitfinlmg.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/gapdgezkj.sHtML

ruff format . && ruff check --fix .
来源：http://wap.yfazqb.com/Article/details/gfrupjjkc.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/gvhlxggks.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gucwmkpmt.sHtML

[U34] Py：判断编码
来源：http://m.share.tarul.cn/Article/details/gsrnfrjpg.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/gavnvqiou.sHtML

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/gvgkdntet.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/gskpzjvgx.sHtML

[U36] Py：定时任务
来源：http://m.share.fktsv.cn/Article/details/gpdwxwpgm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.tarul.cn/Article/details/gvhryldmu.sHtML


<!-- 参考信息 -->