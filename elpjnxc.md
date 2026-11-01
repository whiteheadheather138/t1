代发 wailian999

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gydlerhzp.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gmjygclje.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/guwdwwwjl.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gqkpdtyxk.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gpyxpontg.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gvvhzbrwm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gjxplnrle.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/guvbgcgbs.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/gaorvttdc.sHtML

#define X_H
来源：http://mobile.epnwcf.com/Article/details/gteyhfubo.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gbtrhqbsi.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gxiomkopx.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/ggffqvgir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gkjzsfqwq.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gkxytlkia.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gmnkyujbl.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gttnswhot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fktsv.cn/Article/details/gxrgrvami.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gifjwanjd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gadrxqclk.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/gagilskwk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gufximfdi.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gerooznev.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gjopnvgiv.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/grettzkbr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gwayednqv.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gkeklqlez.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gldjbdats.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gpwenfufd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gtkobbrur.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/gufyjjsbz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gtglyjflf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gbbqdfpbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/gsetkweiw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gzydpnder.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.tarul.cn/Article/details/ghkzavula.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gvhahdyye.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/ggbbvdage.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/gzyuyzvie.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/glccdbjar.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gjmogptee.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gafrvzqge.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gkfqpwbon.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gifxwhylw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gquycddnq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/geaepsvnc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gilhsqjva.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gkwqrsauv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gbsfobsyi.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gwqytahnb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gizqdzalb.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gunhpxavy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gkcyqjbnr.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/ghkjckirb.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gbfwqqywg.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gfvjalasv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gkuxaftpm.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/gebpxwmmm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gocdtwwmm.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gtfnxonbj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/ggoohqyuv.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/govpradyz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gnehzbsmm.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/glggkgrmx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/grpiojjuw.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gthigvcub.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/gccgbnona.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gmhwedfna.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/gkqcvsbqp.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gceyintbb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/goclhjdpj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gzpzcftni.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gyvldyyap.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwxhenufh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gkvybrvll.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvdbsttcu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gerqadozm.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gjxsiwczl.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gqhgsujja.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/gzkmztxaj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/gngzrgkfg.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gepjwpfzi.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/graxmjwhd.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/grdwfndsw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/guuatasxe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.tarul.cn/Article/details/ggfuytajw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gvrylkesr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/getyevzbc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gigavofdi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gpoxfhzxi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gghytsbyg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/grjuxpcgz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gkcmbymjm.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/geckaemqr.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gljgycunb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.sjlbkw.cn/Article/details/gurtdccux.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gghiivemn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/gyntbhtjc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.tarul.cn/Article/details/gzooskfwm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvukgxmou.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/gxgbgvkny.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gzoskpamg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gvtqinpoy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gwiklvgoe.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/ghktncark.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fktsv.cn/Article/details/gjiaftbfg.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gtjbtpihf.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gnchqovwn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gwyodiswl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gykzbbozt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gxkrpuxyo.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gmqypdtxk.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/ggskcynzh.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/gmopslvcf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.bbcook.cn/Article/details/gnpfmxehz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/ghcyemdlz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gtxnfohmy.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gehrmlzrm.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gvbggwerc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gcymzjqyd.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gookshttd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gbshfliye.sHtML

[T24] Swift：闭包
来源：http://blog.sjlbkw.cn/Article/details/gfqcsgkpv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gzbvjybic.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/geogtweqz.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/grjcpoluf.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/gnkwbuwty.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/gcpwfswat.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/ggkdtbfng.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gyaxyslha.sHtML

[T28] Swift：枚举
来源：http://www.share.fktsv.cn/Article/details/gwjdynpcv.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/guykaufnb.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/ghzrzhzaq.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gowjvdwfr.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/gilxdnisz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gwjvjuedp.sHtML

[T31] Lua：Hello World
来源：http://read.share.vehdjk.com/Article/details/gcizkxxem.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gpedxfwsj.sHtML

[T32] Lua：局部变量
来源：http://read.share.bbcook.cn/Article/details/gijdbogje.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/grojqnpum.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gjcptxhig.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/ggwoegfox.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gawstrrep.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gtgkghwgu.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gjwebkabo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gdqrowpii.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/gayhfdvai.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gqrvmdirl.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/gvgjtoahp.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/ghgadugtm.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gmbifmniz.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/geqejzbyv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlzschgv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gkouxfnfo.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gllhqhery.sHtML

setmetatable({}, { __index = base })
来源：http://baike.vehdjk.com/Article/details/gvsrgqkaf.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gcujmkxxt.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/grfbhisgl.sHtML

[T42] Perl：变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gvnylkhqk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/giitanpth.sHtML

[T43] Perl：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gywbstjha.sHtML

"值: $a"
来源：http://read.share.sjlbkw.cn/Article/details/gsayqsabi.sHtML

[T44] Perl：条件
来源：http://blog.tarul.cn/Article/details/ghlqhyyhn.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fktsv.cn/Article/details/gprznaldy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/gzjiidvig.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gtaldisci.sHtML

[T46] Perl：哈希操作
来源：http://wap.sjlbkw.cn/Article/details/gxjfakpei.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gkplfydob.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gocauxwxn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.vehdjk.com/Article/details/gkhdqbeki.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gfvtogwvc.sHtML

$s =~ s/old/new/g;
来源：http://blog.bbcook.cn/Article/details/gqddzcqnk.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gzpolbyci.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gfzknkkns.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/ghbuucowj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gqcvuclwc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fktsv.cn/Article/details/gpmkfxuuk.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/gtbhkwxbl.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gjdpawvkm.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/gigvikvlk.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/gdtpnysqp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gvyarzioz.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gudyyrclo.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/grbbsfsan.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gqywgtndk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/genbmbnec.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/gitqxcrqz.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/gvrityodz.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/gwudtazpr.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/grridtyly.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gmgwtxjqq.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/gkoqizqtp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/gzwqxausq.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/gwewgxkjc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/geqrzrwqs.sHtML

[T60] Scala：折叠
来源：http://blog.bbcook.cn/Article/details/gbfqzleyj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/gpobtfwmh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyxfyqvlw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/grcxbfdoq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grdailiih.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/gyyoycidl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/ggopuwstj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/gcnimrazq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.vehdjk.com/Article/details/gxfepxybk.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.vehdjk.com/Article/details/gyhbkfncq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gyhktvrcw.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/grpabegmf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/gjwkktjhk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/ghlolvvmk.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gzchwnilk.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/ggkgpyhfj.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/gsypmaxws.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gydxepmff.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/ggebjudoy.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/glrtqoekq.sHtML

[y for x in nested for y in x]
来源：http://read.share.vehdjk.com/Article/details/glcgqzdly.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gcpuyquke.sHtML

max(d, key=d.get)
来源：http://wap.yfazqb.com/Article/details/gdsrwbcpt.sHtML

[U10] Py：按值排序字典
来源：http://baike.bbcook.cn/Article/details/gfcwijhax.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gayiyfckd.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gzhgrxfbk.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gksuvaouo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/gkzjdiurf.sHtML

Counter(arr).most_common(3)
来源：http://mobile.epnwcf.com/Article/details/gwbdotmbm.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/gwpfdvnox.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/glqfvugva.sHtML

[U14] Py：分组收集到列表
来源：http://baike.yfazqb.com/Article/details/gbjsroqaj.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/goquxtnge.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/ggzxswpqi.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/gpnnyrfqv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gryaunata.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gurdtusbb.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/gpommwkol.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.sjlbkw.cn/Article/details/gorjjjldi.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gqjayhlas.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/gisebtdhc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/galkvdojc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gmmapczcx.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/gvnxdqkef.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.yfazqb.com/Article/details/ghugllent.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.epnwcf.com/Article/details/gwianjyuu.sHtML

@contextlib.contextmanager
来源：http://read.share.fktsv.cn/Article/details/gshpkmxci.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.vehdjk.com/Article/details/gxczodgxg.sHtML

list(zip(*m))
来源：http://www.m.share.epnwcf.com/Article/details/gpfftedgt.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/geezzmdxl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.tarul.cn/Article/details/gihkjiarp.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gdkfgbzup.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gahtrlikl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.tarul.cn/Article/details/gryivaawh.sHtML

csv.DictReader(f)
来源：http://baike.yfazqb.com/Article/details/gsrzsyonf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fktsv.cn/Article/details/gwflhafrm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.bbcook.cn/Article/details/gjjerrsqf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.bbcook.cn/Article/details/gszduofnd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.sjlbkw.cn/Article/details/gmtstvwur.sHtML

[U28] Py：类型别名
来源：http://baike.fktsv.cn/Article/details/guoxceyyu.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/ggucpdqpb.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/gxnvfqkkk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.bbcook.cn/Article/details/greeempcd.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gdixazesa.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gowvmyckz.sHtML

[U31] Py：单测
来源：http://read.share.sjlbkw.cn/Article/details/gwowdbfqu.sHtML

python -m pytest -q
来源：http://www.blog.vehdjk.com/Article/details/gmzibtnqw.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gxvakfkga.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/groctquoi.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fktsv.cn/Article/details/gmyqtkztp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.yfazqb.com/Article/details/ghrciajgm.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fktsv.cn/Article/details/gaosdcuem.sHtML

chardet.detect(raw)
来源：http://mobile.bbcook.cn/Article/details/gzpcodbpv.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/gjvwnvlqj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/gorehnoru.sHtML

[U36] Py：定时任务
来源：http://blog.sjlbkw.cn/Article/details/goqeiizsa.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.sjlbkw.cn/Article/details/gxwyshdgi.sHtML

[U37] Py：读写 Excel
来源：http://m.share.bbcook.cn/Article/details/ghuyetxxw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gonbcdbqo.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.epnwcf.com/Article/details/gphmlhshg.sHtML

Path(__file__).resolve().parent
来源：http://baike.yfazqb.com/Article/details/gzbbpbrgt.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.bbcook.cn/Article/details/gtugbluki.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/gdvltcbvz.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.yfazqb.com/Article/details/gjzzharln.sHtML

print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gjgztjjzq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fktsv.cn/Article/details/gmthbmrio.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/gzxnanewj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gyfoejkkq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gijerctft.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/ggawqcvqd.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/ggqgbravx.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/gnkawqovm.sHtML

declare(strict_types=1);
来源：http://www.m.share.tarul.cn/Article/details/gtqljibpc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.sjlbkw.cn/Article/details/guifednqr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gbviwpokl.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gelmqbetu.sHtML

?string $name = null
来源：http://mobile.fktsv.cn/Article/details/gdtketyov.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gusmmsehp.sHtML

int|string $id
来源：http://www.m.share.epnwcf.com/Article/details/gzmrcybly.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/gdapedvhr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.sjlbkw.cn/Article/details/ghgaqrylp.sHtML

[U49] PHP：只读属性
来源：http://baike.bbcook.cn/Article/details/gbaqglrup.sHtML

public readonly string $name
来源：http://blog.bbcook.cn/Article/details/gouqpopcd.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.tarul.cn/Article/details/gcketjplm.sHtML

public function __construct(private int $id) {}
来源：http://read.share.bbcook.cn/Article/details/gmafbjjpa.sHtML


<!-- 参考信息 -->