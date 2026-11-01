代发 wailian999

static int counter = 0;
来源：http://read.share.fktsv.cn/Article/details/ggwpqkslo.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/gkuxcpnkt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gcpyosvyv.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gsitpxnka.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gpgbagigz.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gqsxwjnql.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gqnituzsf.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gogjspqnz.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/gzrhkenre.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/grmcjiezi.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gkcwpfyse.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gsmrapene.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gomjyfgbr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gssgenpon.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gdafrueoc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gazylalij.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gwushtarl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gvtrfrjbu.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gvmwdgkxr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gmvfxingc.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/gqvqetchw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/ggbmeclqc.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/giqahktys.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gswxgxgdf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gvoprxvby.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gdwfjehnl.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/gdgptmrhw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/gqfqpewpz.sHtML

[S41] C++：类与构造函数
来源：http://wap.vehdjk.com/Article/details/gbtzxarqx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gisxvngyv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gwiymyudc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/glvaovhrt.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gajxeaeux.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkolhzwh.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/ghiwfvctu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/giakhniye.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gyuiuvfcq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.vehdjk.com/Article/details/gssnuwepz.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gmfxhfnms.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gjwtcfyyf.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/goauteozn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gatpwdbne.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gfsuucpis.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/grjjbxtpm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gwzqislsx.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/goqpzvgjy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.tarul.cn/Article/details/gfybjstjd.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gsatnahgu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gtbqcqasl.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/guatlmiop.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gmsxabeim.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gemsmlgsx.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gympgfcno.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/godsppdpy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gjzhonxwc.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gyoulnzbh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gjtzecinm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gevstfzvb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/grbipycqn.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/geavnzwor.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.epnwcf.com/Article/details/gftxfzgnd.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gqvmrzmtx.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gxjjidzns.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/gjifsdsto.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gqhwwdjnw.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gwzqwciyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gaalhkzde.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gyxctbklk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/gbbmcvuiw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxaeoqxje.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/ghraxehyy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtgzfjknr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.vehdjk.com/Article/details/grirvuyfi.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/guhepihru.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gbvrshwru.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gogfhuhbh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gofpfkfvv.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gorylelfu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gsxngyyfd.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/glhyhazyy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gqfmzsygo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/glrgzzsvc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gsgicobkh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/grflabupp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gdwzrkafm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gxpbdftfd.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gfruanhrq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gcghvcmwq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gzqnzllit.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gulqvbawd.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gxxhgvrho.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gusgnrgal.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gfndafcux.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.vehdjk.com/Article/details/gyuxqduvn.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/gycarbhkj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gzsnoftoq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gplkukegz.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fktsv.cn/Article/details/gugvkvarf.sHtML

[T14] Kotlin：循环
来源：http://3g.bbcook.cn/Article/details/goqnmuxlg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gdgzzwqla.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/garyzeusm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gorzibzzc.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/gnbtrrpvu.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gzahhbxgz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/geohcguct.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gfeupajfd.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gbrcbgdyc.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gzbngalek.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/gwtqoreti.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gtcjokpoz.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gkqchawil.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gizbucdre.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gbsyqejsz.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gsiijjrwd.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/ggrzyknrc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gxqlokqwq.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/goyboeqnu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gvehliycd.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/grllwrlqe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gbmsjlovt.sHtML

[T25] Swift：结构体
来源：http://mobile.yfazqb.com/Article/details/gfvccdwyz.sHtML

struct P { var x: Int }
来源：http://m.share.epnwcf.com/Article/details/gbdkcobrg.sHtML

[T26] Swift：类与重写
来源：http://wap.epnwcf.com/Article/details/gyitowrpr.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/gsgdjcwft.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/ggtzcnyvt.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/ggdcwhjfa.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gwgeljmmc.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gsfyquyew.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/gnnfugakv.sHtML

guard let x = opt else { return }
来源：http://3g.vehdjk.com/Article/details/gxnpqjosw.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/gimuctchm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/glpmxyeqt.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ghtiudnfv.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gggmqzxvp.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gceleyqif.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/gwlrpmiaa.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fktsv.cn/Article/details/gfoogcpzp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.bbcook.cn/Article/details/gjsjmjwyb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gtsrvoqpb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/gvknspauh.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gdfpuddgn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gajuqynth.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gntqpvszs.sHtML

function add(a, b) return a + b end
来源：http://www.share.fktsv.cn/Article/details/giuumwipz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/gauuxoewk.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gobmrzyvt.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/ghuefaewj.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gldeyosem.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gwjjxhgxs.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/gprvgynvm.sHtML

[T40] Lua：元表
来源：http://read.share.epnwcf.com/Article/details/gqrzrzckf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/gybiglbxg.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/garhxpfwa.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gbjdysmjs.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gojzvwjhi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fktsv.cn/Article/details/gbtzcvdac.sHtML

[T43] Perl：字符串插值
来源：http://blog.tarul.cn/Article/details/glxckdgri.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gahxcyuvj.sHtML

[T44] Perl：条件
来源：http://www.blog.fktsv.cn/Article/details/gnthhwxns.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gkmsfyyzt.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/grnhdoyep.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gcnfxbuso.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/giczotyrd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gekwxvkqj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/gpnkadbkc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gfogbcpll.sHtML

[T48] Perl：正则替换
来源：http://blog.tarul.cn/Article/details/goemmlpse.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fktsv.cn/Article/details/gmkycqjxc.sHtML

[T49] Perl：函数
来源：http://read.share.tarul.cn/Article/details/ggzdgacpv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gsurkbftu.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/goxibupuy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/ggkgumwyf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.epnwcf.com/Article/details/gmpizqcig.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gyjgompba.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gatragavo.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gnrjoqkto.sHtML

val a = 1;  var b = 2
来源：http://blog.yfazqb.com/Article/details/gxbjysfqb.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gccjueczg.sHtML

s"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gnihccqjz.sHtML

[T54] Scala：集合映射
来源：http://mobile.epnwcf.com/Article/details/gholraywh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/ggjfkerrq.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gmlxststk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gtxixuqbx.sHtML

[T56] Scala：样例类
来源：http://read.share.sjlbkw.cn/Article/details/gkpbbylgi.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gbmsgicpv.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/gwjmidwxk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.epnwcf.com/Article/details/ggtkikvzu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.sjlbkw.cn/Article/details/gafqqwkax.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/gqqsdsedf.sHtML

[T59] Scala：循环
来源：http://www.m.share.fktsv.cn/Article/details/gtjougytp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/grumynehx.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/gfjwrjpbp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.bbcook.cn/Article/details/gonxepesg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwlxbiwht.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/girzkpsio.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/goxibuhua.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fktsv.cn/Article/details/grjxdkhyl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gzfpqhyut.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gagqlsqxf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/gdkjnfgio.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.vehdjk.com/Article/details/gludvmgmk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/gsmdorrlh.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gfmauushn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/garvexkga.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/grjpoacqo.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gbasibmuo.sHtML

[U06] Py：合并两个字典
来源：http://blog.bbcook.cn/Article/details/givqkprrc.sHtML

{**a, **b}
来源：http://wap.fktsv.cn/Article/details/geilxorxv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/ggkfyregh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.bbcook.cn/Article/details/gcwsjxnzx.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gsfehbucr.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gvzxeumqb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.sjlbkw.cn/Article/details/gylyencky.sHtML

max(d, key=d.get)
来源：http://baike.tarul.cn/Article/details/gwzobftql.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gmaoprfhk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gcinxuczi.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/gmkkxiibm.sHtML

(x * 2 for x in arr)
来源：http://www.share.bbcook.cn/Article/details/gegiscpzf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/grdbuwanz.sHtML

Counter(arr).most_common(3)
来源：http://3g.vehdjk.com/Article/details/gboxrnlna.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.epnwcf.com/Article/details/grotfylqt.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/gkpfnjohc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gdehavzof.sHtML

defaultdict(list)
来源：http://blog.bbcook.cn/Article/details/gatekapje.sHtML

[U15] Py：高精度计时
来源：http://blog.bbcook.cn/Article/details/gonqvywvv.sHtML

t = time.perf_counter()
来源：http://3g.fktsv.cn/Article/details/gzaiekakp.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gvkbrsxsc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fktsv.cn/Article/details/girpfguhm.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gwgjxepmm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gvgwgqoea.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/gavfstpyh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gtftaafws.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/grzjyofur.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.tarul.cn/Article/details/gidfnckmd.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.vehdjk.com/Article/details/gwuixtvus.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/gpdmpvula.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.vehdjk.com/Article/details/gzkfmksnm.sHtML

@contextlib.contextmanager
来源：http://www.m.share.bbcook.cn/Article/details/gikrdqdeq.sHtML

[U22] Py：矩阵转置
来源：http://blog.epnwcf.com/Article/details/gaodnevia.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/ggrliytnx.sHtML

[U23] Py：分块读取大文件
来源：http://blog.bbcook.cn/Article/details/gazxeyhlj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/gpfvlcgod.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/guwohvsnz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gmcdtpmuj.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.epnwcf.com/Article/details/gnkoqzgdl.sHtML

csv.DictReader(f)
来源：http://3g.bbcook.cn/Article/details/gngeavaiq.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/gveudzjst.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gfgtbtfyi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/godhbvnps.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/gcgiueybb.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/gnwknhtje.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gkmhvpwmf.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gfqwjzlcp.sHtML

@property 与 @x.setter 配合
来源：http://www.share.yfazqb.com/Article/details/ggjahothy.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gpdaujgbk.sHtML

@dataclass(slots=True)
来源：http://baike.bbcook.cn/Article/details/gfjajejbj.sHtML

[U31] Py：单测
来源：http://blog.sjlbkw.cn/Article/details/geljzohdk.sHtML

python -m pytest -q
来源：http://www.share.vehdjk.com/Article/details/gdtyohrtf.sHtML

[U32] Py：代码格式化
来源：http://3g.fktsv.cn/Article/details/gbqtkrvec.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fktsv.cn/Article/details/gkfdgvexn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gcnzfiuqj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gibjopkmw.sHtML

[U34] Py：判断编码
来源：http://3g.fktsv.cn/Article/details/guogdehqm.sHtML

chardet.detect(raw)
来源：http://baike.epnwcf.com/Article/details/gzgrnsqfg.sHtML

[U35] Py：发送邮件
来源：http://blog.sjlbkw.cn/Article/details/gyqvtekba.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.yfazqb.com/Article/details/gxsuuxhnr.sHtML

[U36] Py：定时任务
来源：http://baike.fktsv.cn/Article/details/gxzlxcxdx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gntmeqwck.sHtML

[U37] Py：读写 Excel
来源：http://blog.epnwcf.com/Article/details/gmrlwvkuo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.tarul.cn/Article/details/gltgslssm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fktsv.cn/Article/details/geubuowbw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.sjlbkw.cn/Article/details/gxxoytmte.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fktsv.cn/Article/details/glihfsdik.sHtML

sys.stdout.isatty()
来源：http://www.share.tarul.cn/Article/details/gbpmsvtsy.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gkynfdchf.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gpdkisgkw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.vehdjk.com/Article/details/geiqatetu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.epnwcf.com/Article/details/gqnwxlhvk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.epnwcf.com/Article/details/gedbqztbi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gygrbxjmq.sHtML

[U43] PHP：声明命名空间
来源：http://wap.yfazqb.com/Article/details/gtqrfgjol.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gekspgrdb.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.bbcook.cn/Article/details/gvnkroovd.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/gblmankqt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.yfazqb.com/Article/details/guwodcupi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/guofzgeaj.sHtML

[U46] PHP：可空类型
来源：http://wap.vehdjk.com/Article/details/gftxibotc.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/gfwtiazay.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gmcbmhtok.sHtML

int|string $id
来源：http://blog.bbcook.cn/Article/details/gshaakaue.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gptvlajju.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gecwmccrp.sHtML

[U49] PHP：只读属性
来源：http://www.share.fktsv.cn/Article/details/gcgrzldvr.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gizyzjhav.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fktsv.cn/Article/details/gjfhnqpiw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gswsehxfw.sHtML

[U51] PHP：数组解构
来源：http://mobile.sjlbkw.cn/Article/details/gojsmbfdq.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fktsv.cn/Article/details/gjvimwcdk.sHtML

[U52] PHP：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gxoomvosc.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fktsv.cn/Article/details/gysivywdh.sHtML


<!-- 参考信息 -->