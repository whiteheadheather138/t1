代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/givqftiol.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gatdxlhrc.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/ggqlmwxrw.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gltekdxto.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gjfjnmbso.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gcvimffkr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gghuvraau.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gsxrnigwq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/gevnnelik.sHtML

[S19] C：快速排序
来源：http://m.share.sjlbkw.cn/Article/details/gfofibycy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gftqsewgx.sHtML

[S20] C：二分查找
来源：http://mobile.vehdjk.com/Article/details/gooeruzek.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gakoohzdf.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gmomufsmm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/gkyyjsxfi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/ghblnsfnz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gtcfmveaj.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/gxfrouzzq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/grxwckzgp.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gngbhhnvc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gyeaesoeq.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gobhwsmal.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gnoyteujr.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gbyncspyh.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.sjlbkw.cn/Article/details/glixfslle.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gqoihdlfi.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gskcghozi.sHtML

[S28] C：静态变量
来源：http://www.share.bbcook.cn/Article/details/gfntbpcxd.sHtML

static int counter = 0;
来源：http://www.m.share.fktsv.cn/Article/details/gmzsmvzzf.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/gyslqupxz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/goqzzrjrp.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gwyagdyhf.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/grinovose.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gopohpalr.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/gzeqemzyo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gwspwzaqv.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/ghnkwnkob.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/ggnnxczfa.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/glfmpvrau.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gqgetsgvr.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gmjonwapo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gzyvddpth.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gqdvxqqbl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gueikgvvi.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/giducjvja.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gxrmswukk.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/glmjhntfp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/grzrcardk.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gyydwjzha.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gnhhuxyje.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/grqymswnr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gtvsplvtp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gfcxaanol.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.yfazqb.com/Article/details/gokuwpbcu.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gyjqtezlp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gtsgcdrtu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/gfjlrrakl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gwdhajkzp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gqbwphrrd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/ggbxjelyv.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/gsenkjrqj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.sjlbkw.cn/Article/details/gsykathqc.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gzgnagivp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gdlrazout.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gxgnknuas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gzjaglvij.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/guhgunxjf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gvzhqzpyz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gdqoaqqxp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gndgunzqq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gllpoijom.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gyfemihby.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gunsxbouk.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gxikdvdeh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/grlhvtded.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gyiyhdwga.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/geqpykfjl.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gmlggwgvm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/gqbikwhqm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gdnjyrzae.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/gxkeinkog.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gfqlnhgzz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gfmclnpob.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/ghadbbqlg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gkaohjncp.sHtML

[S55] C++：结构化绑定
来源：http://blog.yfazqb.com/Article/details/gztncdewb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gfpslxufg.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/geswygzoo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gmquajlnp.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/goriokfjr.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gsmgtrgkp.sHtML

[S58] C++：命名空间
来源：http://baike.epnwcf.com/Article/details/gyitwyreq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/gtsprhdaz.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gjwcpuxpk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gjgasdtwv.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/grukwxeec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gicbkfwsl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmhehmtqi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gfjicgevp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbajnpzhq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gplnhbiic.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gzsaeqwdo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gijgvvqvw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.bbcook.cn/Article/details/gxttecnzz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gdgrvsxro.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gkigjpqpa.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/gnmevqjcb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gnfvlkser.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/grojpwbsu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gzrglfeua.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/godgiexym.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gdlcbjkkm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gscryqkll.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/grefwwpsk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/glpnwzgoa.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gonoftavb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gsxdkiooq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gevqzqdxf.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.vehdjk.com/Article/details/gnplcyuey.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/ggumzjcsk.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gsuqhpfww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gzprmiqxh.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/gykpykpil.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gerjvzerm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gosvolymi.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.tarul.cn/Article/details/gcqsngvir.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/gqojlkcfb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/goguiswsa.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gbcrgbjuk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/gnrrosrgk.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gtdfsfwtb.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gkvnmkkvr.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/ghatdibfd.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/gigkevqqh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gpmdiwiko.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gwbwsclss.sHtML

[T19] Swift：可选绑定
来源：http://read.share.bbcook.cn/Article/details/gzhhlaydf.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gevdiqdjt.sHtML

[T20] Swift：数组操作
来源：http://mobile.epnwcf.com/Article/details/gralwkoxn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gtbwmwvru.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gcuyvaexo.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/giwrkdybs.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/ggboqsxlj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/gzwqjnfow.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gkzhlgjok.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/gfqrvcalk.sHtML

[T24] Swift：闭包
来源：http://read.share.epnwcf.com/Article/details/gctwtlmcw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gpmpfzbys.sHtML

[T25] Swift：结构体
来源：http://www.blog.vehdjk.com/Article/details/ghgymsohr.sHtML

struct P { var x: Int }
来源：http://www.m.share.tarul.cn/Article/details/gcgmtkbgv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gjqpggwjc.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/glusryrzx.sHtML

[T27] Swift：错误处理
来源：http://mobile.epnwcf.com/Article/details/gvgbcrgou.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/ghfoloyrl.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gxegpdzyi.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gkiwemmqc.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.sjlbkw.cn/Article/details/glrxgdhmc.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gzsjiblkh.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gulfsbive.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gahtsadvn.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gafaaatln.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/goatymehf.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gdtjatldk.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gvipltjlq.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/gcaoigupc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/ggpuagtqj.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/grpqurcad.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/ghdmzshea.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gfggycmkb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/gjnqcmkxw.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/gosqzmsqi.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gwzqlvvrr.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gzowoncqc.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/gmwkpbyvm.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gjnnrsrvg.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gmzezxajx.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gcqqkwghy.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gojriimmi.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gaklalgud.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fktsv.cn/Article/details/guszggsrg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/goeqgdkit.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/ghrjltzsj.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gzfeececq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/ggztovxdt.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gvynmgpsn.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gjnwmwpeq.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gepbndypv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsihulvcf.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/guihqbwpb.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gzszahoqk.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/gqkaujcwn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gxykipqth.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gtxiywybh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/gtxdzmjyi.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/gfrzbnvnz.sHtML

$s =~ s/old/new/g;
来源：http://blog.epnwcf.com/Article/details/gdmuaxdwd.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/ghznibcgr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/grtnyksip.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/gynufomwb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gazvwquxa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gsigczdon.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gihoefzcu.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gkdfsrneh.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gtrjvsfld.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gcmvlubmu.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gssrukzjn.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/glamvmzrx.sHtML

[T54] Scala：集合映射
来源：http://mobile.bbcook.cn/Article/details/gpbxlaxgh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/gekfmwmjt.sHtML

[T55] Scala：集合过滤
来源：http://m.share.yfazqb.com/Article/details/grfubyefm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/govhejzkf.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/grwyqkmrh.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/gmlypausm.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gaigpoxyh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gyanyxryp.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/gzmotfebe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gfyvqcatv.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gclbnngxp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gergrpktp.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gbococgsp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gdqmrbhcx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyggdakpw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/gtavhzrzg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/givxrnpem.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/gczzfelrp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.bbcook.cn/Article/details/gsknjffoe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/ghthjvyxz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.tarul.cn/Article/details/gspxbxpxi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gtyzkvtkd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.yfazqb.com/Article/details/gbqslkpgr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.yfazqb.com/Article/details/gsnfftnbx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fktsv.cn/Article/details/gbqpowqrn.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gmfivalba.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gofrdbzcx.sHtML

[U06] Py：合并两个字典
来源：http://blog.vehdjk.com/Article/details/gsdjzptxy.sHtML

{**a, **b}
来源：http://read.share.epnwcf.com/Article/details/gwplldpfb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.tarul.cn/Article/details/gsgvnebuv.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gzrvnuccv.sHtML

[U08] Py：展平二维列表
来源：http://read.share.sjlbkw.cn/Article/details/ghchlwtrg.sHtML

[y for x in nested for y in x]
来源：http://blog.epnwcf.com/Article/details/gswwlheqt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gneeypjas.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gjehqpsuo.sHtML

[U10] Py：按值排序字典
来源：http://baike.vehdjk.com/Article/details/grmcthokq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gnzlkrdro.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.epnwcf.com/Article/details/ghzgdvkhj.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gcwcbwovj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/garjkcnoz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gziqufkhp.sHtML

[U13] Py：固定长度队列
来源：http://www.share.tarul.cn/Article/details/gavjlpwpk.sHtML

deque(maxlen=10)
来源：http://mobile.epnwcf.com/Article/details/gbjlaulzf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.epnwcf.com/Article/details/guruqmenu.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gqqxzyxxr.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/gxassqcya.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/gqzubvruu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/glrdhiwsx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/gajpflxat.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/gcpcjuhdj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.yfazqb.com/Article/details/gjvlafocg.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gqkiisdsr.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.vehdjk.com/Article/details/gmdrcywxy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gwkjmqkmz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.epnwcf.com/Article/details/gnqzbztpg.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gnebchvhn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.bbcook.cn/Article/details/ghfmhgdvs.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gxeupjeix.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/gxkubhjaq.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gajevxnpa.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gpcgftnxx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.yfazqb.com/Article/details/ggoftlekf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fktsv.cn/Article/details/geusuxhvi.sHtML

[U24] Py：路径操作
来源：http://blog.fktsv.cn/Article/details/gwutnlkds.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gzigiapiy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gwzkcxbzc.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/gipqluess.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fktsv.cn/Article/details/gouhzzkpd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.tarul.cn/Article/details/gyhkgufbs.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.yfazqb.com/Article/details/grjznvfzg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gnwpwdpbh.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/gmdwxoiom.sHtML

UserId = int
来源：http://3g.yfazqb.com/Article/details/gdtdhbyrb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fktsv.cn/Article/details/ggfejndwz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gsuelmscu.sHtML

[U30] Py：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gnmjwpeee.sHtML

@dataclass(slots=True)
来源：http://3g.bbcook.cn/Article/details/grlfcxedx.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gksicnqyx.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/ggeclgcjt.sHtML

[U32] Py：代码格式化
来源：http://www.blog.vehdjk.com/Article/details/glxtgjjnn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.vehdjk.com/Article/details/gsrnakqef.sHtML

[U33] Py：打包发布
来源：http://read.share.epnwcf.com/Article/details/gfrnqtwea.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gxeweidtr.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gvdyrbege.sHtML

chardet.detect(raw)
来源：http://baike.vehdjk.com/Article/details/gvgmxprae.sHtML

[U35] Py：发送邮件
来源：http://baike.sjlbkw.cn/Article/details/gxyhualob.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fktsv.cn/Article/details/gdlzyhqzi.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/gvxzsofkr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gjihdfxlq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/glweadjjj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.sjlbkw.cn/Article/details/gvwatnbmx.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.sjlbkw.cn/Article/details/gzmjfsfzm.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.yfazqb.com/Article/details/gfpyfzudr.sHtML


<!-- 参考信息 -->