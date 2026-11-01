代发 wailian999

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gabmicbci.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/gjemsfuxl.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/ggkprjpko.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gnqfhfpgg.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gpnypnwxg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gvelopvmb.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gsxhvqpin.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gjjpllytk.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gretianwb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gxgucwkek.sHtML

[S34] C++：遍历 vector
来源：http://3g.fktsv.cn/Article/details/gmetbmauh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gurvlwanr.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gqtvujtzl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gqfbqsvmm.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gpuytcwje.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gecndmjzs.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gprufboyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gqrohddoj.sHtML

[S38] C++：排序
来源：http://www.blog.bbcook.cn/Article/details/gagjiylxg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gwuzcowcr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/ggygmkyor.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gqpxfookw.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/ghwyhnymp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gkqrnnzzj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gwmiollmq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/goqvdlsjf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/goidjepml.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gpdeobcgq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/gltbbbche.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/giupfvhku.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gzehjdnnc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gzlchqtpu.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/gdwoatvwr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gnkiabhzt.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gnsizasld.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/gotedxhsu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gzzrswgzm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.bbcook.cn/Article/details/grojhlblo.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/goqtvcpap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gnloobxhw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/giuucspka.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/gsctpqqlj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gpcmtbhmy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/gknklsyqg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gytutkjlt.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/gmmmnqvcw.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/gjkmkhopg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gfmnearsj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gytlhmgpq.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gechdoixh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gqiqblnzi.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/ggtsbdoyi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/gyndsfjwu.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gvtbbeixt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gjdzfpzdm.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gejnazkhq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gizwdeoeb.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/ggeylzcrg.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gsvkcdpyx.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gzncgzjtj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gvyiwfain.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gjmqyvfoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/gjyqlyuyk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gglcddioa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/ggzvacein.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbquncrid.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gjhhxutnm.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqfqvglak.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/grqndtoor.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/guqqmdlbz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gywzwcgli.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gcbtezyfm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/gjgpnebvb.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gjgmqqsoa.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gbytqqkem.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gdszoecmo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gtdnciydc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/giqhobbzu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/ghaysneoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gzhxfqyct.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gjyebdxfr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gicpdoqwi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/goxzoxifb.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/gkkfhhrik.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/giecszstq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/glsfdqtxt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gkumfkfbt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/gltxtocij.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/guxgnbagu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gesklhmqh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/geavdlutl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/ghznckiiu.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gdckenwnx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/gyjlacjsp.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gbyqycove.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gtyvdigej.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gvcdyoizc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/gnkonazci.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/ggywafpcr.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gainhcxfd.sHtML

[T17] Swift：变量与常量
来源：http://3g.yfazqb.com/Article/details/gbkyufxhe.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gtpfpspgy.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/gjrhxlodp.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gfdbjzzaq.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/gpadjxodo.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gohwgopoz.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gutrnjooi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gevhkfvxg.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gobtjcboj.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gwczurhpq.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gpdoljlkm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gbraburvq.sHtML

[T23] Swift：函数
来源：http://blog.sjlbkw.cn/Article/details/gayxlcaaw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gkmjspmqi.sHtML

[T24] Swift：闭包
来源：http://m.share.bbcook.cn/Article/details/gyewrotzo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/glldshohk.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gjvehilfr.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gqpzggnvj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gjkvawkde.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/gtcqjtzps.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gfgknoans.sHtML

do { try f() } catch { print(error) }
来源：http://3g.epnwcf.com/Article/details/gkntllmcl.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/gmkhewede.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/guaptbfvi.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gauwqmrzl.sHtML

guard let x = opt else { return }
来源：http://m.share.tarul.cn/Article/details/glfdrtfzr.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/gslfsyqqs.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gpnixqdkd.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gjlnlwywo.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gshtevfbl.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/ghkqlpfaw.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/ggykwbvgk.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gpsxybseu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/gpjdxzqlz.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gusiivsvi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.epnwcf.com/Article/details/gwgsottnb.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gfnqkhsae.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/ghiesrodi.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/glwvrnmay.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gmmcamdxm.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gxupdpmde.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gcnowetxa.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/gxriuolcu.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/gdjcfmbwe.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/ginlkaxmv.sHtML

string.find(s, "%d+")
来源：http://m.share.yfazqb.com/Article/details/gcraavmzb.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gdxysvpml.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/gclnvmosu.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/gcufuuqla.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/gxfcjyjbi.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/gotebwltw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/ghnnxpifv.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gnqtvlind.sHtML

"值: $a"
来源：http://wap.vehdjk.com/Article/details/gnawpjzba.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gsscjelvg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfwlvpbfc.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.yfazqb.com/Article/details/gkekysccq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gapikallg.sHtML

[T46] Perl：哈希操作
来源：http://3g.sjlbkw.cn/Article/details/gzabiegah.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fktsv.cn/Article/details/gpavfwtku.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gomofcids.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.bbcook.cn/Article/details/glozrqfkt.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gkrlikeav.sHtML

$s =~ s/old/new/g;
来源：http://baike.vehdjk.com/Article/details/ghlkqzdle.sHtML

[T49] Perl：函数
来源：http://read.share.yfazqb.com/Article/details/gnftnmcjg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gsmfntgec.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gntnlzrpv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/gedelyqfl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gmbzbkmix.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/gcwuxetgv.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gvzgrqtya.sHtML

[T52] Scala：变量
来源：http://read.share.yfazqb.com/Article/details/gxknakmre.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeunokbi.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gjagipifr.sHtML

s"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gjwjtlqpl.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gxehfymhh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gmmgfgfzq.sHtML

[T55] Scala：集合过滤
来源：http://3g.epnwcf.com/Article/details/gbyrhbykn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.bbcook.cn/Article/details/girvwkmjx.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gaiygbidv.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gtylvrgmf.sHtML

[T57] Scala：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gkzqujcml.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gksddphit.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gjwtenxqd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.bbcook.cn/Article/details/gbneubvdh.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gexrzmerb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/grvkwzoyq.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/gtpqexylh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/giyxgnucg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqcjsseoy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/gdetsyomj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtnqdyfwf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gzurbdtjw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/ghatgiqma.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.bbcook.cn/Article/details/gjwrjyzct.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/giuzxyonl.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gomiydrli.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gcxsthcxj.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gdpcvzqxj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fktsv.cn/Article/details/ggqdwloms.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gzqjhkcui.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gwoepieyu.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gkxjmmcpy.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gwcflpwcc.sHtML

[U07] Py：反转字典键值
来源：http://blog.tarul.cn/Article/details/gcmucspcv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gkwuyrkuf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gjtypcjcz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwrwtmqt.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/glfzebuxn.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/glupxagjh.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/galbdguet.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.vehdjk.com/Article/details/gikjbzndy.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/gzogjbckc.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/gyoilqamw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gpudizobp.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gdasdyqct.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gazejlqyp.sHtML

deque(maxlen=10)
来源：http://www.m.share.epnwcf.com/Article/details/gczrlcpjn.sHtML

[U14] Py：分组收集到列表
来源：http://3g.vehdjk.com/Article/details/gjuwkmfcb.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gynoyylja.sHtML

[U15] Py：高精度计时
来源：http://www.blog.sjlbkw.cn/Article/details/gqlershaq.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gvwmqjlzs.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/glkzainzz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/ghfhtcbej.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/gtexazlss.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/govblnzuf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/gyfktulfj.sHtML

pat = re.compile(r"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gnqymxjeo.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/gbqwdudey.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gmxcifpvs.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.bbcook.cn/Article/details/ghjbsznhq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/grzperaqt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.sjlbkw.cn/Article/details/ghdydcncn.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gzgrlorip.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/glihulswn.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gwyszewrh.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gsawnkzhj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.tarul.cn/Article/details/gwozymyqt.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fktsv.cn/Article/details/gqvakbgfr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gwwtgezog.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/ghywqzmov.sHtML

csv.DictReader(f)
来源：http://wap.vehdjk.com/Article/details/gjkesnxvv.sHtML

[U26] Py：并发下载
来源：http://blog.tarul.cn/Article/details/gholizvmw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.bbcook.cn/Article/details/gqdwueexa.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.bbcook.cn/Article/details/gseweoqsa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.tarul.cn/Article/details/glkhivphv.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/gbmzvbxrs.sHtML

UserId = int
来源：http://3g.yfazqb.com/Article/details/gkavexzfz.sHtML

[U29] Py：属性校验
来源：http://www.blog.vehdjk.com/Article/details/gbrzahzvv.sHtML

@property 与 @x.setter 配合
来源：http://3g.epnwcf.com/Article/details/gpnxxiote.sHtML

[U30] Py：数据类
来源：http://www.share.epnwcf.com/Article/details/gbrmvjupy.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/gdsepamsa.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/govoprngk.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/grxydxbzy.sHtML

[U32] Py：代码格式化
来源：http://3g.fktsv.cn/Article/details/gvthyaqor.sHtML

ruff format . && ruff check --fix .
来源：http://baike.bbcook.cn/Article/details/gmqfclrii.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gdvcezzlo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gdnbscbbl.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gavztkexj.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/gvanoacwr.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gibamnzic.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fktsv.cn/Article/details/gleyyzafh.sHtML

[U36] Py：定时任务
来源：http://3g.bbcook.cn/Article/details/gceejxgrz.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fktsv.cn/Article/details/gnmusonct.sHtML

[U37] Py：读写 Excel
来源：http://blog.vehdjk.com/Article/details/gmzxwkmtx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/gzkirvuwt.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/gnwxgbvqm.sHtML

Path(__file__).resolve().parent
来源：http://baike.bbcook.cn/Article/details/grmvkmjiq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fktsv.cn/Article/details/gggqxdclb.sHtML

sys.stdout.isatty()
来源：http://www.blog.tarul.cn/Article/details/gsjjhgwdz.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/gxtcjmspu.sHtML

print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gqngpyyfh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/gqweumldc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gpegqjluh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gbppwhlxw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gkvrcxewk.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gavvhrjok.sHtML

namespace App\Http;
来源：http://www.m.share.tarul.cn/Article/details/gucmvgzai.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.sjlbkw.cn/Article/details/gnevipdzz.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/gbmioaddk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.bbcook.cn/Article/details/gpqtulozu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gknjitwmj.sHtML

[U46] PHP：可空类型
来源：http://m.share.fktsv.cn/Article/details/gssrfoseb.sHtML

?string $name = null
来源：http://blog.fktsv.cn/Article/details/gmtqvakyc.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/gkpeuatjb.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gcqoneddq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.yfazqb.com/Article/details/gslkvxyhw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gyrovxkvk.sHtML

[U49] PHP：只读属性
来源：http://wap.fktsv.cn/Article/details/gtgdnyanh.sHtML

public readonly string $name
来源：http://baike.fktsv.cn/Article/details/gkowauumv.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.vehdjk.com/Article/details/gygzgydtu.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gtcgsbevf.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/gjaepkbxv.sHtML

[$a, $b] = $arr;
来源：http://www.share.yfazqb.com/Article/details/gwqolhnvs.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gpfvsinaq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fktsv.cn/Article/details/gbnouzaww.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/glterkyid.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/gyucjafqu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.vehdjk.com/Article/details/gvjrjveuu.sHtML

$obj?->method()
来源：http://wap.sjlbkw.cn/Article/details/gbtcoirau.sHtML


<!-- 参考信息 -->