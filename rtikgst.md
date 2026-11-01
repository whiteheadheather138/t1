代发 wailian999

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gmkuhshue.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gxhvscrrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gkfoddits.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gvwgcjbcj.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gegvrwizn.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gxqvcjhzn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gzdpfqvzc.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gfyabdkgw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gzzfmrjqn.sHtML

[S21] C：字符类别判断
来源：http://3g.sjlbkw.cn/Article/details/gssnslukq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gbhmwyemk.sHtML

[S22] C：字符串转数字
来源：http://blog.epnwcf.com/Article/details/gtbjjksfo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/glkctymbd.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gleujchzi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gopvfprpz.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/gomxvboqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gjwbkkiig.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gmetkabli.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gzhsvznfl.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/ggsijtjyx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gfkbvrbom.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gnuuvuxow.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gromywndj.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/grdhcqxaw.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gliyzgfph.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gsgaqbgbm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fktsv.cn/Article/details/gmlevviyv.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/gnwgexkxl.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gfezvtlrg.sHtML

#define X_H
来源：http://wap.sjlbkw.cn/Article/details/gmmepatwc.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gmpsytujr.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gtmtxvbbz.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gmtdoyibk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gvwtlawer.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/gcalqoesq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.sjlbkw.cn/Article/details/gmsjoadee.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gpblqaawm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gdaghcthg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/gyqzfoxlw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gilyppwkj.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/gukdxhfra.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gmdulmbpq.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/glomimyfj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gqllvsdho.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gsbirftqx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/gwdooerhn.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gcgtpcdle.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gttlurpnf.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.sjlbkw.cn/Article/details/gclxcawhf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/gjskccejb.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/ghmnbbxjl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gmwzrqdxt.sHtML

[S41] C++：类与构造函数
来源：http://read.share.epnwcf.com/Article/details/gvkefcysd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gjvafbupo.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/goeaweiua.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.tarul.cn/Article/details/gyymdkijr.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gxxgnwvtm.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.sjlbkw.cn/Article/details/gkntmilwp.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/gvlpbrfds.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/gwtzymyap.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/giqqawvdo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gfwnndxsd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/ghdlmjgzu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gzjhzyofo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gksjwskhm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gdghgcgas.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gpgiuzzak.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.bbcook.cn/Article/details/gzwefuqdi.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/geyeffnfs.sHtML

[S49] C++：写文件
来源：http://3g.fktsv.cn/Article/details/gqqewncgz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gqfgczhwq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/grmxcqell.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/ggkzkfmps.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gtkmfrjoi.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gtetlcwdk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/golucwydx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/gfuphxgjn.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gxkpgbqib.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gzjohqyqd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gwhvpxdux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.vehdjk.com/Article/details/gndyanyyb.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gzlcladdq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gptrzaxmk.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gpwpqlizu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/guwtpxwza.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/glbptfczi.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/gobdgcavo.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gagohskvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/ggnrhtyml.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/gnbuhevch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gbiiokyzr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gitfggjav.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.bbcook.cn/Article/details/gvalizgsx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqjtkrirx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gsckxkzww.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gaqaqfhlz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.epnwcf.com/Article/details/guwrevecl.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/guphgltmb.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gviiziqzd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/glkefgitl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gcstafavl.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gvekhuevi.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gufafgtgn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gwwqcnuwk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gpbfuzgsk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/gomzeyehi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gsturrjed.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gnqofmohd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gclcdwsoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gfoymyfgm.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gjfijaupy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gahbklouv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gelnddxag.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gwkajrxlo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.tarul.cn/Article/details/gpdgdpaec.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gcwbwlppl.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/gmsqxxavq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/gxginytvr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/gpnmszxvp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gjbwhxgto.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.tarul.cn/Article/details/gsrxeicno.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/ghwrmzbqb.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gyughlsiw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gwjcglpmi.sHtML

[T15] Kotlin：接口
来源：http://www.blog.bbcook.cn/Article/details/gdlahzorh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/gtsoucgyr.sHtML

[T16] Swift：Hello World
来源：http://mobile.tarul.cn/Article/details/gxdqvjxje.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gngsovwpq.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gzvinmtfs.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/gkeixgtrt.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/glalxiuye.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/gqaufxazb.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/galwbzclr.sHtML

if let n = opt { print(n) }
来源：http://read.share.bbcook.cn/Article/details/geyytscvn.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/gmpxyrvdp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gwmwqnhsz.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/gmrjfewmt.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gmgpgemkh.sHtML

[T22] Swift：字典
来源：http://baike.sjlbkw.cn/Article/details/girztnkjc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.bbcook.cn/Article/details/gtiqrngbq.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/grdakivzs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/greyciksu.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/gbyzuvynl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/gfthzfcdy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gsgeoaxjm.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gjdupsnjj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gfqtazogk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gzkrdtxix.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gfvtzmpro.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gwifvhryk.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gxtrjvrvb.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gxhdhwbjm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gixnfafxr.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gtwxofjua.sHtML

[T30] Swift：协议
来源：http://wap.yfazqb.com/Article/details/gozstzwcf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gvzhwmdqb.sHtML

[T31] Lua：Hello World
来源：http://mobile.fktsv.cn/Article/details/gmjfmxhfz.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gbwqclpkx.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gcekkrpnj.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gfnlgeydd.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/giqzgwret.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.bbcook.cn/Article/details/gbbyjsnvn.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/gzqirijnj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gagmjbygk.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gjagaaeub.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gxragycyr.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gwejunqyo.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gshsvavqk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fktsv.cn/Article/details/gmtbxyljf.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/goapjuhvs.sHtML

[T38] Lua：条件
来源：http://m.share.epnwcf.com/Article/details/goedzdkiw.sHtML

if x > 0 then print("正") end
来源：http://m.share.bbcook.cn/Article/details/ggdendxik.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gezrqbpju.sHtML

string.find(s, "%d+")
来源：http://m.share.bbcook.cn/Article/details/gcfobjnkk.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gfxeovcrn.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/ghqwszijg.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gcciwrnbu.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gndrrkyla.sHtML

[T42] Perl：变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gxtkudnmh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/gnsvdnska.sHtML

[T43] Perl：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gamoekjms.sHtML

"值: $a"
来源：http://wap.bbcook.cn/Article/details/gbfdykndf.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/giffvyxzs.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gvrywqnem.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gkproszuq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gnkdeflww.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/gdpvqoxej.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gskrlbzkb.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/gigjktrpx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/gkybpiofk.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gvzywhgtr.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gqnshitqu.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gnnphiurw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gsamhwzfd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gwjblukev.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/gyiricwpy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.sjlbkw.cn/Article/details/glylamrrt.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gbegabfgt.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gcljbhfnt.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/ghuqztfts.sHtML

val a = 1;  var b = 2
来源：http://www.blog.yfazqb.com/Article/details/gflpnltuj.sHtML

[T53] Scala：字符串插值
来源：http://wap.tarul.cn/Article/details/gdbdlvenv.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gmapdwmqn.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/ggxlpjdrb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/gojaocpds.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/gvpmiwanj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.vehdjk.com/Article/details/gnmconljq.sHtML

[T56] Scala：样例类
来源：http://3g.tarul.cn/Article/details/gfhzfocua.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gjwvgkzig.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gdxmnrkoh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/gesxfpilo.sHtML

[T58] Scala：函数定义
来源：http://read.share.tarul.cn/Article/details/grsletarp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/gyjshrjrq.sHtML

[T59] Scala：循环
来源：http://blog.vehdjk.com/Article/details/giefyouol.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gmuxouqlp.sHtML

[T60] Scala：折叠
来源：http://www.blog.fktsv.cn/Article/details/ggmhxymgu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/ggygzggpc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxinmhpby.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gyeeebqgu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gihvrzcmb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gambnyreg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gppgmojqn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gbegyywyd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/guxklkcnl.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/gcsmssgza.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/gnlfzdssf.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fktsv.cn/Article/details/gdofbsbxh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gyjjraepa.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/gvishgggm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gaqgupqte.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/gpuligrij.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/glneipeds.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gclgevknv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/gzxnzrwnu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.bbcook.cn/Article/details/gjetvjamf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gftkjyrcb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.yfazqb.com/Article/details/gsfyicpox.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gicttbsab.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gvxilymnm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gdbahakuc.sHtML

[U11] Py：生成器表达式
来源：http://m.share.yfazqb.com/Article/details/gnxmbsltt.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gcotjiusg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gxddfwzzj.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/gqjuyninb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.tarul.cn/Article/details/glbedhadm.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/gkozqxipz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.yfazqb.com/Article/details/guxrnilzv.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gnejwzsux.sHtML

[U15] Py：高精度计时
来源：http://wap.yfazqb.com/Article/details/ggfhtwtoc.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/groostqxm.sHtML

[U16] Py：命令行参数解析
来源：http://baike.tarul.cn/Article/details/gpwndwuxl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fktsv.cn/Article/details/gtcfsducq.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/gajknlhue.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/gmhrajrfs.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gupdljhti.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.yfazqb.com/Article/details/gmluaddhw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/geummehcq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.epnwcf.com/Article/details/gioapwlxb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/gixiqdcka.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.bbcook.cn/Article/details/gxthkqcqv.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gdwbjutiy.sHtML

@contextlib.contextmanager
来源：http://wap.yfazqb.com/Article/details/gmlhabgmt.sHtML

[U22] Py：矩阵转置
来源：http://read.share.tarul.cn/Article/details/gjxqjbtxl.sHtML

list(zip(*m))
来源：http://baike.epnwcf.com/Article/details/gixdwftyz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fktsv.cn/Article/details/ggnyurisw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.vehdjk.com/Article/details/gwqxjitsa.sHtML

[U24] Py：路径操作
来源：http://baike.sjlbkw.cn/Article/details/gysbbyyec.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gawnmqsoo.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gjxpkvxlo.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/gepsfmjtg.sHtML

[U26] Py：并发下载
来源：http://3g.bbcook.cn/Article/details/gpawqdhgs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/gpztrpodi.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fktsv.cn/Article/details/gcyqfooxy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.bbcook.cn/Article/details/gjzmigpmm.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/gtkmvltzb.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gksqlmgpp.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gmghnysez.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gtzhjzfci.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gshgghzjb.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/glnnhcwra.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/guawnsbao.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gdgnafsmy.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/glxlcmbqh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.yfazqb.com/Article/details/girixwtrd.sHtML

[U33] Py：打包发布
来源：http://read.share.vehdjk.com/Article/details/grrdficbc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.bbcook.cn/Article/details/gqbcmfrad.sHtML

[U34] Py：判断编码
来源：http://m.share.vehdjk.com/Article/details/gpftgmroc.sHtML

chardet.detect(raw)
来源：http://read.share.tarul.cn/Article/details/gilhusksr.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gjiuyiade.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlnkoqyg.sHtML

[U36] Py：定时任务
来源：http://m.share.fktsv.cn/Article/details/gevqmldgg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gjoitmynj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.tarul.cn/Article/details/gzdcstjfq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.tarul.cn/Article/details/gufuupttr.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gxispesub.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.tarul.cn/Article/details/gkjcvxlrs.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/gcuchmdzi.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gtohiyeho.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/grwoiiapi.sHtML

print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gpqlxceqz.sHtML


<!-- 参考信息 -->