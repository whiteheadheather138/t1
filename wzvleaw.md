代发 wailian999

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gnyvwyuaz.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/ggomnzkjo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gkoxhtogr.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/gdvlkgtkj.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gmqrzussn.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gbmerrwwy.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gvzxpzzvc.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gqsumogmj.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gukaqqfsm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gakegzzfi.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gqwbkbjqk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/gwfoadhob.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gevcjcrou.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/genyzkity.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gvvbpeuct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gicjexkbf.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gmntrggst.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gtomkwujl.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gttjxeknw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/glkglahsq.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gzbyyelsu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gryolkagg.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gqmvrbmte.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gfprivgzq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/goanvkiey.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gknomknuy.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/grklhmoha.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gbtyrrhpn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/grujnqwko.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gfwarlpiz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gtdgbnhat.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/ghixujotl.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/geszcfhft.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gnapljopy.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gmxvdbyqn.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmegtlrlm.sHtML

[S45] C++：lambda
来源：http://wap.bbcook.cn/Article/details/gwltyayyl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/grgastxhu.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/glpgvfayp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gyleymudz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/gefbmpkpf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyodbynrg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gxkmcxjui.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/goyesntlo.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/gutxocpdd.sHtML

[S49] C++：写文件
来源：http://wap.bbcook.cn/Article/details/gibrvkotb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gsdvdbcpj.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gzfpqosxd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/gddfjyeir.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gatnlgmle.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fktsv.cn/Article/details/gbcabzcbh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.epnwcf.com/Article/details/gtwlrnukx.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvkxcteox.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gzkcsllcf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.bbcook.cn/Article/details/gmblyscgc.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/grtabqixh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/grlrxaewt.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/geovqbolx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gaysvrpbc.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gedekptyh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gtrtgqswd.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gqlyzlzdj.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/gmsovkknx.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gdjrfqnqu.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.bbcook.cn/Article/details/gfwsvypcg.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/grnvxkscz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gkqjrrlro.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/guhyegokh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/gwrbdibwq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gxskwknma.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gtwzijynr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvwozeife.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fktsv.cn/Article/details/glrtinhlb.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/godbwikym.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gzcerwtwt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/gkcrvvogx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.vehdjk.com/Article/details/gakvihifu.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/geqnmfxgv.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gtcpdiyrc.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/gojcibvgu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gfhonrara.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.yfazqb.com/Article/details/gzvibolns.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gqnfpeife.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gdocmhvng.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuogbylw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuoyxbbb.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/ghmcscacv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/glovcbtak.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gnyjfvswx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/giydomtqv.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gtegbguhu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/ggzqdifwl.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/gtpzjnluf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gxzgtnsns.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gizihgfdp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/glzvwiomv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.bbcook.cn/Article/details/gbaeyrflz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gejozjakp.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gemuaoohs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gweqxqcbw.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gxoxaaygh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gcyjxtxlr.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gauvfzdzp.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/ghzbaacgu.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/ghwuvzsyk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/girplvigj.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/ghjqvsqrf.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/gzttrsuim.sHtML

[T19] Swift：可选绑定
来源：http://mobile.sjlbkw.cn/Article/details/gamjskzsb.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/ghblvaloh.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gmjzlockb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gvbotpyis.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gjvqhylrd.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/grxyhztdn.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/gtexerirl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/gedrapocm.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gusvjbsgh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fktsv.cn/Article/details/gavytohmr.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/goqrppola.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/ghfoirkwj.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gkmatttyx.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/guegutzwx.sHtML

[T26] Swift：类与重写
来源：http://baike.epnwcf.com/Article/details/gulbxojpr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gpaxxjxwu.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gorhjvsby.sHtML

do { try f() } catch { print(error) }
来源：http://blog.bbcook.cn/Article/details/gcejdcuuq.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gfvyuozcv.sHtML

enum Color { case red, green }
来源：http://read.share.epnwcf.com/Article/details/gnmgdhbxt.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/gjhqtctny.sHtML

guard let x = opt else { return }
来源：http://m.share.vehdjk.com/Article/details/gkmlzfcna.sHtML

[T30] Swift：协议
来源：http://baike.bbcook.cn/Article/details/gjmrwuepf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gasxccdxy.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gntwnesta.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/giwkbjrrk.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/ghyokymok.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gwhysjipw.sHtML

[T33] Lua：表（数组）
来源：http://www.share.epnwcf.com/Article/details/ghmkrjakz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gpfnyvwkf.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gttsbxxdz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.tarul.cn/Article/details/gtjdmzocc.sHtML

[T35] Lua：字典表
来源：http://www.share.bbcook.cn/Article/details/guqmdzawi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.tarul.cn/Article/details/gfcskhjuc.sHtML

[T36] Lua：函数
来源：http://baike.sjlbkw.cn/Article/details/gnvbcmadf.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/glhivdpya.sHtML

[T37] Lua：字符串拼接
来源：http://3g.vehdjk.com/Article/details/gsupqnebh.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/gbybynufo.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gxpmlqrpy.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.bbcook.cn/Article/details/gorptjvev.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/gddaglxut.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gdnmedfbs.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gkvembawo.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gngbaqxoh.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/goxwosged.sHtML

print "Hello\n";
来源：http://wap.sjlbkw.cn/Article/details/gegklzlas.sHtML

[T42] Perl：变量类型
来源：http://www.blog.yfazqb.com/Article/details/grijyngww.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.vehdjk.com/Article/details/gbuiqmfta.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gjshslleu.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/ghtwxepfr.sHtML

[T44] Perl：条件
来源：http://www.m.share.tarul.cn/Article/details/gnqxcbhwp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gczfaigmx.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.epnwcf.com/Article/details/gofffzexb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gnflgycxv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.vehdjk.com/Article/details/gtocbzqeo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/ghpuzxdok.sHtML

[T47] Perl：正则捕获
来源：http://baike.sjlbkw.cn/Article/details/ggumvvjsm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gfyxkokne.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gswtmnnpu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/gcwtpxqst.sHtML

[T49] Perl：函数
来源：http://read.share.epnwcf.com/Article/details/gjtjpdhfs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gjxggywew.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gakysrnqz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/gdqqulmdh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/grhgmfotc.sHtML

[T51] Scala：Hello World
来源：http://www.share.tarul.cn/Article/details/ggcsbdrqr.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/glnohgbwl.sHtML

[T52] Scala：变量
来源：http://read.share.bbcook.cn/Article/details/gfsughmjs.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/glsghubay.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gumbrqcog.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gatfbndow.sHtML

[T54] Scala：集合映射
来源：http://mobile.epnwcf.com/Article/details/gosmpwblc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.yfazqb.com/Article/details/gfvgmkpom.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gagxztezo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gsgthbjzy.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gqnmiecqf.sHtML

case class User(name: String, age: Int)
来源：http://3g.bbcook.cn/Article/details/gqwxctgug.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gfwhymynv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/gucadgvpg.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/gtxcjseio.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gfazkgheu.sHtML

[T59] Scala：循环
来源：http://m.share.sjlbkw.cn/Article/details/glphaqdjz.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gdkbheojx.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/gqptihfqd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.sjlbkw.cn/Article/details/grnvdsvvn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtantbkaa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gixlynjau.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gevuqgvss.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/gqwzxmeif.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/gkystubor.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.tarul.cn/Article/details/gexledrik.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/gkwmtcwoy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gwtdmhkfs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/goqlwqcbi.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fktsv.cn/Article/details/grgjyhvhg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fktsv.cn/Article/details/guzpkivlx.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/giemrfmnp.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gezsonmfc.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gqppnosbj.sHtML

{**a, **b}
来源：http://wap.vehdjk.com/Article/details/gruupiuvt.sHtML

[U07] Py：反转字典键值
来源：http://3g.yfazqb.com/Article/details/gehjihrmh.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.bbcook.cn/Article/details/gmnobvlfx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.yfazqb.com/Article/details/gbqwuhfbg.sHtML

[y for x in nested for y in x]
来源：http://baike.yfazqb.com/Article/details/gkteddsye.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gkrcdyntt.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gsshdmbqb.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/goxmywqhf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fktsv.cn/Article/details/gnpefhmzx.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/gbnqgulaz.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gorhbudqr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gmparrola.sHtML

Counter(arr).most_common(3)
来源：http://read.share.tarul.cn/Article/details/ghdahqdor.sHtML

[U13] Py：固定长度队列
来源：http://3g.epnwcf.com/Article/details/gmokdjyex.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/geogkkety.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.bbcook.cn/Article/details/gbcjuvnls.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gunwbmptw.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/gqxcfjthq.sHtML

t = time.perf_counter()
来源：http://read.share.fktsv.cn/Article/details/gvcpautvo.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gqjxjfkfc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gnxsfqqaq.sHtML

[U17] Py：初始化日志
来源：http://m.share.tarul.cn/Article/details/ggnjqhvny.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gnklqezrz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/geyhaxuyg.sHtML

pat = re.compile(r"\d+")
来源：http://baike.yfazqb.com/Article/details/goywfgngr.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.vehdjk.com/Article/details/gpkpomgsm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gfuaqhijk.sHtML

[U20] Py：缓存函数结果
来源：http://baike.tarul.cn/Article/details/gztfsvkle.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.sjlbkw.cn/Article/details/gvvcymblj.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gnakbfqfm.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gtpugklud.sHtML

[U22] Py：矩阵转置
来源：http://3g.fktsv.cn/Article/details/gjwvwyexu.sHtML

list(zip(*m))
来源：http://3g.sjlbkw.cn/Article/details/gnaakbyxp.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gevjxuchy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gfblasqxf.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gwigslbjo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gpdblsfsy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.sjlbkw.cn/Article/details/godfblefz.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gfgxmyufy.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/gbaxoyumn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.epnwcf.com/Article/details/gkhakgqwg.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.epnwcf.com/Article/details/gfzarqbnr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/gjcjshisp.sHtML

[U28] Py：类型别名
来源：http://baike.vehdjk.com/Article/details/ghegcnoqp.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/ghytzdisj.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gnfgtlvig.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fktsv.cn/Article/details/ghltbsnjz.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gcvulsfyv.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gizurqywy.sHtML

[U31] Py：单测
来源：http://mobile.bbcook.cn/Article/details/gkxvwlegf.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gunzjmoec.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/girlayvjg.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.tarul.cn/Article/details/ghgukpqgo.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/glnexzrfd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.yfazqb.com/Article/details/gzurhvdyh.sHtML

[U34] Py：判断编码
来源：http://3g.epnwcf.com/Article/details/giejgnnxf.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gcuwggcwr.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/getjyoafs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/gbjxiktao.sHtML

[U36] Py：定时任务
来源：http://m.share.vehdjk.com/Article/details/gxbyqmysf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gkfggygpu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.sjlbkw.cn/Article/details/gycgpjmdw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/ggeqfgxpr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.sjlbkw.cn/Article/details/gnqmlnkmp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.vehdjk.com/Article/details/ghrektldz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/gnfovjwkc.sHtML

sys.stdout.isatty()
来源：http://blog.fktsv.cn/Article/details/gjkmfyycl.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gdzjnnbck.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gvoaetegx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.tarul.cn/Article/details/gyrperluv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gkihaunge.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gksnpkqun.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.vehdjk.com/Article/details/gcfxqbcjs.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.vehdjk.com/Article/details/ggvmmclre.sHtML

namespace App\Http;
来源：http://www.share.bbcook.cn/Article/details/gpfixjkkg.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.sjlbkw.cn/Article/details/gfbtcgfql.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/grbmwyurr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gkhildagr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gcrmflnyr.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gkjhxswav.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gorzwidni.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gvusevkig.sHtML

int|string $id
来源：http://blog.yfazqb.com/Article/details/gmogiqegb.sHtML

[U48] PHP：纯枚举
来源：http://blog.yfazqb.com/Article/details/gcqpqadjm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/gximyyagm.sHtML

[U49] PHP：只读属性
来源：http://3g.epnwcf.com/Article/details/gnlhvrecm.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/gygoyfjjd.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gtrobtook.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gqjdyaise.sHtML

[U51] PHP：数组解构
来源：http://m.share.epnwcf.com/Article/details/gbbukmvfa.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gaadpqvru.sHtML

[U52] PHP：箭头函数
来源：http://baike.vehdjk.com/Article/details/gtqjirssv.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.yfazqb.com/Article/details/gndvobecn.sHtML


<!-- 参考信息 -->