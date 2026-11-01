代发 wailian999

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gzqlpiyjl.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/ggpvfjtzc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gycurlhvq.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gmbtcalkc.sHtML

#ifndef X_H
来源：http://wap.bbcook.cn/Article/details/gtudbgool.sHtML

#define X_H
来源：http://3g.tarul.cn/Article/details/gwotvrxhv.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/ggdixiyeg.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gibiwafzh.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gupbhsuod.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/ghsvncxgz.sHtML

[S32] C++：字符串
来源：http://www.blog.tarul.cn/Article/details/gyppfhfcr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gdtboiunp.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gbcvgocmf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/gnklwziaf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gryejaflv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gwatgehte.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gbmcrcrub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gjrpwclal.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/glbeeafxh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gprflztsh.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/ghhbnwlxk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gtjelznxn.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gxuwnwfno.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/gijfrolwo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gmafurjwr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gqxlgmuja.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gjxvsbmho.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gxomyhlqi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/glhldoebp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gortpdduf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.sjlbkw.cn/Article/details/gwwpwsecg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gpzmgbhya.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gcpzdoxor.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/ghgmxewyu.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/glqapkrju.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gvmekkyqz.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gynaubnfi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gadjmhhnu.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gsksaxtop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/glrxuqsqn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gwaqhsvjx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gqmphxdur.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gbpibphqq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/giyqyzzsz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/ghjrtjjgk.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/gfdgcmphj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/griyiyldq.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/gfbiqizxo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gbiicuful.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/guohcfawj.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gbryhkjqg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/glmpzsmzf.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/geyiwyooy.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/gqczjbajc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.tarul.cn/Article/details/gxgdkuxzz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gvelmiehc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gsfkvefom.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gefpiaukx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/grnfrfzjk.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/gtxoaeydv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.sjlbkw.cn/Article/details/guhechqus.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gbgtvohpi.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gomnvalwp.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/grnhiniyd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/groablnsi.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gsvtrnscz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/geqsfoonz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.vehdjk.com/Article/details/ghkzshfug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gzluknrip.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtvejdiba.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/ghwjhowkl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcpwqbamm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gxsmrcegp.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gxunavrum.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gyujlqddr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gcsfwqxpv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gcycvlzse.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/goudnozmn.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gxbzwsjbt.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/gobzdeklk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gfuzsgqrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gdszciquf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.vehdjk.com/Article/details/gefokzhfo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gbxgylgde.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gzsdzjvak.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gkyqjtftr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/geaklylhg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gxjcpehei.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gadlhzqpg.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/ghzkfpodp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/giwulhtdy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gytssnuhl.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/ghxlzrupq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.sjlbkw.cn/Article/details/gchiacwno.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/gpaoluagz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfqbbebfi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/ghufpjwsh.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/gniswosbn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gkbmhifaw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gcxrmlvwh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkgkbtgf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gfaasoovy.sHtML

[T16] Swift：Hello World
来源：http://m.share.bbcook.cn/Article/details/gkyytgacm.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gikawpchr.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gcrltqebg.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/guhqlcsoq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gmsradfrg.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gdkqarwnt.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/grvudfppe.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gjhxyfpbf.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gcfnfzddw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/grfmvfiie.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gbjbjhdpm.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/gqaredxlf.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gkhxpftoq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gzhcmjilh.sHtML

[T23] Swift：函数
来源：http://www.m.share.bbcook.cn/Article/details/gkiyapnjh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gxraoseuz.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gqixfnlfi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gjazwzqhj.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gerjgbsne.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gyodztorb.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gnhtihgfd.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gqylhzduc.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/gxeqptyxc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gfipzttli.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gburdfdyd.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gisjzwbnk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gmblstpez.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/grvvbjfrw.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gtxzvpkko.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gexnfuphj.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gbdtwwcys.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gvlskpfkw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gprgtdhhz.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gwsvevayz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.epnwcf.com/Article/details/gvnotlgkf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/giuwhqpkg.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/grkqjsnmg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/glyapmkoh.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gmwpgtydj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/gdemoqlko.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gtucmwrvu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gjdkxoopr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/grxmkcdds.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/glvcfwgov.sHtML

[T38] Lua：条件
来源：http://wap.fktsv.cn/Article/details/gfymimxpy.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/grvgvmetl.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gntzzhwbd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gmdnxvcec.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/gxiieonnv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/gnpypacdq.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gcvfgpets.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/goiplicwg.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gwykqitxt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.bbcook.cn/Article/details/gbmqquyfs.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gblzyqzhh.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/gvcytpabs.sHtML

[T44] Perl：条件
来源：http://mobile.fktsv.cn/Article/details/gdsmigotk.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gsgiotwna.sHtML

[T45] Perl：数组遍历
来源：http://www.share.tarul.cn/Article/details/gmdymfxcg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/ghcpkwomh.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/ggpfqvnhy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/gestjscgg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.sjlbkw.cn/Article/details/gekiuiyjk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gxgzpvodk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gnwmsatru.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gulfyuney.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gbgjjlfyd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gvgqzpjti.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdpkhsuzc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.bbcook.cn/Article/details/govfuhreu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/ghpofiurz.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gzxkdfyua.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gvcngrwck.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gwjbmkhhf.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/gosamnksk.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/gphoanhvw.sHtML

s"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gewawedxn.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gucrmdzwq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gkkfvxyvz.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gyzfvcwtg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.epnwcf.com/Article/details/girkkzynp.sHtML

[T56] Scala：样例类
来源：http://mobile.sjlbkw.cn/Article/details/ghdnulirt.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.bbcook.cn/Article/details/ghvwqksao.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gydfbpumb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/gqfogwipy.sHtML

[T58] Scala：函数定义
来源：http://blog.tarul.cn/Article/details/gcdfubjhp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/gcjglftxa.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gzwskvohj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gzempbqpg.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gsxksrcsf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gtopjejtd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/goopjsyst.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggflzzsxo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggjmyckeh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.bbcook.cn/Article/details/gibljtfww.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/gxgexyljo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/guidbqbms.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/glfdezczi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.epnwcf.com/Article/details/giukrysrl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/gsxrivpvp.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/gexxbvtyc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/gzturmltm.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/gnrxawseq.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gvaplburb.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gotrkicun.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gvmorncrq.sHtML

[U07] Py：反转字典键值
来源：http://wap.yfazqb.com/Article/details/gsexkamws.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/grpdwztmm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/goezkwrxd.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gkjmoozyx.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.sjlbkw.cn/Article/details/ggdvxslxi.sHtML

max(d, key=d.get)
来源：http://www.share.yfazqb.com/Article/details/gvhfggkpz.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gnxsenban.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gpcokufdr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.vehdjk.com/Article/details/gnctbdmwb.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gdccywpel.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gmuqhqnyn.sHtML

Counter(arr).most_common(3)
来源：http://baike.fktsv.cn/Article/details/gtitjifpf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gglijprbh.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/gnnnnpgcc.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gkcojdpxe.sHtML

defaultdict(list)
来源：http://m.share.sjlbkw.cn/Article/details/gaqngsnoc.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/grigrypff.sHtML

t = time.perf_counter()
来源：http://read.share.vehdjk.com/Article/details/gyzymwlxx.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/glnhncopm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gtcfrwcme.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzhwjedr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.sjlbkw.cn/Article/details/gpfosplde.sHtML

[U18] Py：预编译正则
来源：http://mobile.fktsv.cn/Article/details/glebemtxi.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gniibwrtp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/gpfsdfnrp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/gddidsprv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fktsv.cn/Article/details/gfnpfrixh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.epnwcf.com/Article/details/gwxnzbhzu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.bbcook.cn/Article/details/gxuvgognq.sHtML

@contextlib.contextmanager
来源：http://www.blog.epnwcf.com/Article/details/ghaaevsnu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.sjlbkw.cn/Article/details/golwmpgyr.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/grruddsjd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/giuqcquwl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gorqbvcet.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/gwzjsrezf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gfykfnyjb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.tarul.cn/Article/details/ggbgwyysr.sHtML

csv.DictReader(f)
来源：http://blog.sjlbkw.cn/Article/details/gptdrweev.sHtML

[U26] Py：并发下载
来源：http://read.share.fktsv.cn/Article/details/glvrbexjb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/gvuhtzywa.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.sjlbkw.cn/Article/details/gadrdryac.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.yfazqb.com/Article/details/gzmpwzzoy.sHtML

[U28] Py：类型别名
来源：http://www.share.yfazqb.com/Article/details/gcvplrami.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gohjscqnq.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gdoeiagqy.sHtML

@property 与 @x.setter 配合
来源：http://mobile.sjlbkw.cn/Article/details/gjrwkjdyc.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/gurjsmwgb.sHtML

@dataclass(slots=True)
来源：http://www.m.share.yfazqb.com/Article/details/guxzsuidu.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gqmuugrpc.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/gmumpoddf.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/gpnqapnnn.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gxmoxuerv.sHtML

[U33] Py：打包发布
来源：http://blog.yfazqb.com/Article/details/gtkvrvjpp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.tarul.cn/Article/details/gwtpwvfya.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/gskfwmvqx.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gsjmazpfs.sHtML

[U35] Py：发送邮件
来源：http://wap.fktsv.cn/Article/details/gketuaesl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.tarul.cn/Article/details/gqjfozmjr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gzyfpitso.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.yfazqb.com/Article/details/gbhqofrqo.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/gsfymsuhe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fktsv.cn/Article/details/gjqyayiga.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gukvydinm.sHtML

Path(__file__).resolve().parent
来源：http://3g.sjlbkw.cn/Article/details/ggdpthgip.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.yfazqb.com/Article/details/gstoejxvp.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gbqtismcg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.tarul.cn/Article/details/gyhwwaeeb.sHtML

print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gylqhngoe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.yfazqb.com/Article/details/gjcpotguu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.yfazqb.com/Article/details/gvgcnxqqq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.tarul.cn/Article/details/gibmoqafz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gdledhgwu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fktsv.cn/Article/details/gcqhdaqoz.sHtML

namespace App\Http;
来源：http://www.share.bbcook.cn/Article/details/gmcokipzx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.yfazqb.com/Article/details/gkjlbnyie.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/gwpawtrjq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/gekyxdqts.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gpngsuqav.sHtML

[U46] PHP：可空类型
来源：http://wap.yfazqb.com/Article/details/gdlodxivs.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gdonixboo.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/gnakoqmay.sHtML

int|string $id
来源：http://mobile.epnwcf.com/Article/details/geerfacpf.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/gxfdrvsfz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fktsv.cn/Article/details/gwkixqkio.sHtML

[U49] PHP：只读属性
来源：http://read.share.fktsv.cn/Article/details/gvekzftmv.sHtML

public readonly string $name
来源：http://3g.bbcook.cn/Article/details/golxwjcmh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/gfzcukuzo.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.vehdjk.com/Article/details/gzqfgqjwq.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gsqmqnhom.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/gldohozrb.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gkvzvptyt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.vehdjk.com/Article/details/gdqusdpvh.sHtML


<!-- 参考信息 -->