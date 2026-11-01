代发 wailian999

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/glirmeghu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gdcawebgg.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/goamrnjkb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/geexbmbga.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gizivlhoy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gjicglpbd.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gfjhjztra.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gzprabuct.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/guunjrisc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gzxjgwsoy.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gcpenynhd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gchvjvyms.sHtML

[S37] C++：set
来源：http://www.share.fktsv.cn/Article/details/gocmgibfa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/ggroftglf.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gowtqmbbt.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gasuuokyl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gifyzuyrt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/gqezofnyc.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/ginfznqqo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gmcycumqr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/getzpqzqi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gklpenkgr.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gkpifauvv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gvutomcsf.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gpjohxdlc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/ggoazyvfw.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gujddmxlt.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/gixynemag.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gbzgmhmqt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gruecvjdw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gdjccxxdu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gwnxpusow.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gssmwuyad.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gpnslpadk.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gcycmiegk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gcbxnnmwu.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/gcwteotdw.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gsortrrko.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.tarul.cn/Article/details/gqpekbotj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gfjpnikfl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gotkkrtmb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gpgqchzjh.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gktzkmbsx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/groedxfxj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gismssrrz.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gkoveqlpk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gvqqrwtoe.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gbcsmfwgg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gweacmvsg.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gjxwlkjrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fktsv.cn/Article/details/gpcgyijzd.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gemjnvpdz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/ghvkndeop.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gkaputzrf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gzvdjavyd.sHtML

[S58] C++：命名空间
来源：http://blog.yfazqb.com/Article/details/gnxiquaoe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnnbenya.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gatiwglan.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gyfkwgazx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/glkcoitnb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gucolenjs.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvpahlgjo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gmeswhukf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghgzavebc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gmlcaphdl.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/giosllncs.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gkbymimgm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/gdzdlxlyj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gemfdavid.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gqbpnzrkn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gvrhkclgh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/glukpoafa.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gjavrypdl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gvtxheffk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gqcmmfnoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gleyopeum.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/grgihmhgd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gvtwfwrka.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gcmwjpjch.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/ghulrkjen.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gcvxmuort.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gpenuikmj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.vehdjk.com/Article/details/gzjrasqkn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gqfzfiaxs.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gwvmgfcgt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/glyhutnna.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gkhwnpyro.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gwxxwtsmt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gkbmaruby.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gawqrfkjz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/gcsbzsvbd.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gsxkznvvj.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/geylelsxs.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/gbhkqksve.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gcqkqtlzk.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gbiokkrbh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gxbhaddzv.sHtML

var a = 1;  let b = 2
来源：http://m.share.vehdjk.com/Article/details/gngvqyhcr.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gsavywffq.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gjtrvkznd.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gaoappbaw.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gkplvvqgb.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gdpaskvqa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gavfqvhqs.sHtML

[T21] Swift：遍历
来源：http://baike.vehdjk.com/Article/details/gzurlbfih.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/gyifdpmvc.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gmgcnjlej.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/giabcoplu.sHtML

[T23] Swift：函数
来源：http://blog.yfazqb.com/Article/details/grspbyawo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/gndzuyztm.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gzqocfeuk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gaxjzzhgg.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/geftoozdj.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gmriaapmx.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/gymmzghjc.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.epnwcf.com/Article/details/gymxnbopz.sHtML

[T27] Swift：错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gimjtypfs.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gzrgumoqg.sHtML

[T28] Swift：枚举
来源：http://www.blog.yfazqb.com/Article/details/ghvlvhqry.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gnmrdxeys.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.tarul.cn/Article/details/gkxwxytmp.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gwkogdszn.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/glfkrqqvq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gaiddyyfd.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/giqykfxiv.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gvzkzfarq.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gaoevskdx.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/ggkjdypdu.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gwxaavxcx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.bbcook.cn/Article/details/gyhuziihb.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/gnyentpfu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/ggxhbfezo.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/gxncgfgdr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/gtbfxwfse.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gjtjbpupz.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gxmiarzbs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gxexxefce.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gmskqyiom.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/glntxfhdm.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/gbdlrrfel.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/geccyjhhk.sHtML

string.find(s, "%d+")
来源：http://m.share.tarul.cn/Article/details/grdoxyrxo.sHtML

[T40] Lua：元表
来源：http://www.share.tarul.cn/Article/details/gdouchxqd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gacaosxzc.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/gatexvjpa.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gqasuncly.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/gsbllyvqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gngblxlpo.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gzeybkvmd.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gjmijcgzm.sHtML

[T44] Perl：条件
来源：http://www.blog.yfazqb.com/Article/details/gsvjqhvtu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.epnwcf.com/Article/details/gsehfafoc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gagieteyc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.bbcook.cn/Article/details/gfyzxhvhk.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/gnsideuan.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gwogxwsbo.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gombobvqf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/gvmxcwalr.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/ghdqxmnrn.sHtML

$s =~ s/old/new/g;
来源：http://3g.yfazqb.com/Article/details/gcpjaoxqv.sHtML

[T49] Perl：函数
来源：http://m.share.vehdjk.com/Article/details/gxumwioee.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gqwhmqdwb.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gzpmrbylz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gcynpyard.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.tarul.cn/Article/details/gkerarwyo.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/gjsvtvdph.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gtfocsbtl.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/geoiwhuow.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gocqcnqca.sHtML

[T53] Scala：字符串插值
来源：http://wap.tarul.cn/Article/details/gpmznoovf.sHtML

s"值: $b"
来源：http://blog.epnwcf.com/Article/details/gkyasbmzv.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gmmjbrzha.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.vehdjk.com/Article/details/ggquzduns.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gbdjwjlhd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gsnamcrti.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/gztyamaqd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gynpvrfhe.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gfyyaafsy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gjjbjbitx.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/ghhnuxcdb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gunydksxr.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gwgbpkrso.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/gsluayxbr.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gypzmkrdb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.sjlbkw.cn/Article/details/gebyzaizw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdvybkifa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/gmdvxspax.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdafcebkr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.epnwcf.com/Article/details/gbqfznqbh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.epnwcf.com/Article/details/ghfrbogph.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.sjlbkw.cn/Article/details/ggssphjky.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gkgxpuuxu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gtkzmboqz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.sjlbkw.cn/Article/details/gnhjkuatv.sHtML

[U04] Py：变量调试打印
来源：http://3g.tarul.cn/Article/details/gyswxetsc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gfhupefvy.sHtML

[U05] Py：列表去重且保序
来源：http://blog.yfazqb.com/Article/details/gpdinczlw.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/ggijsjqyw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gkggogtyb.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gqmcplnyh.sHtML

[U07] Py：反转字典键值
来源：http://mobile.sjlbkw.cn/Article/details/gtsbnnkbt.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.bbcook.cn/Article/details/gohhmvcqp.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/gnuneebxa.sHtML

[y for x in nested for y in x]
来源：http://read.share.fktsv.cn/Article/details/gpnszxxld.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/ghwjjgviu.sHtML

max(d, key=d.get)
来源：http://www.blog.vehdjk.com/Article/details/gowhejotd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gesbhpizf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fktsv.cn/Article/details/gslaszzjl.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/glbrovvba.sHtML

(x * 2 for x in arr)
来源：http://blog.bbcook.cn/Article/details/goltecaxy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.epnwcf.com/Article/details/glwtvdnlh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gbidugidv.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/gfvugwqxl.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/ggaisgkwz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gcfzehyik.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gheiigywk.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gbohjznwk.sHtML

t = time.perf_counter()
来源：http://baike.sjlbkw.cn/Article/details/giuphazkh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.vehdjk.com/Article/details/giugninpn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/gpqygwknz.sHtML

[U17] Py：初始化日志
来源：http://m.share.vehdjk.com/Article/details/gltacgdev.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.vehdjk.com/Article/details/gmqbpecxx.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/gnnwmqlks.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gmknfzfuc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/gogdiwifq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.epnwcf.com/Article/details/gdypyoodo.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gztytgwqh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gpodwybzo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/gaohorlfp.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gkfdktmyw.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gyttfviun.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/ghqwablaf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/giyfahxez.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.vehdjk.com/Article/details/grrklojjg.sHtML

[U24] Py：路径操作
来源：http://www.blog.epnwcf.com/Article/details/giyqaxofx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gkrsnhnhs.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.yfazqb.com/Article/details/gkxiierwg.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/gtdzaeltw.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gyqfcuukm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gdmvebvmh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/grluqnahy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.vehdjk.com/Article/details/gkevinoqb.sHtML

[U28] Py：类型别名
来源：http://m.share.tarul.cn/Article/details/glnkkfqtm.sHtML

UserId = int
来源：http://mobile.epnwcf.com/Article/details/glguohzgq.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gkmjeeavg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gkpxwerzx.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gukizpgml.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/guxlwalgk.sHtML

[U31] Py：单测
来源：http://mobile.vehdjk.com/Article/details/gbehqcqzh.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/gawjrnabb.sHtML

[U32] Py：代码格式化
来源：http://baike.epnwcf.com/Article/details/gudrqkvew.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gatafmzhz.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gzzillebp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fktsv.cn/Article/details/gtiumrfik.sHtML

[U34] Py：判断编码
来源：http://www.blog.bbcook.cn/Article/details/gpxdsodpx.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gppeozegi.sHtML

[U35] Py：发送邮件
来源：http://read.share.sjlbkw.cn/Article/details/gmjjqrmbk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/gtmumydhl.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/ghqoaqium.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fktsv.cn/Article/details/gxfbwfiwu.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/gizbheixa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/guqafkops.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.bbcook.cn/Article/details/gkbhzijwm.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gljpqdqmg.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.epnwcf.com/Article/details/gmnatqvkd.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/gxpeynqqt.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gbzpqmcpn.sHtML

print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gvruzgruu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/gdomnixaa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gfscppdnn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/gnmvugmkf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.tarul.cn/Article/details/gywwzvbbb.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gakqorfdo.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gygjajuaj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/ggkvhvcii.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/gmmydydcl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.yfazqb.com/Article/details/gxdyaopfn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gsysyqelf.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/gwfftfwnt.sHtML

?string $name = null
来源：http://baike.yfazqb.com/Article/details/gefxrnlbo.sHtML

[U47] PHP：联合类型
来源：http://www.share.fktsv.cn/Article/details/ghqbcxvku.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/gcmmbmpsn.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.epnwcf.com/Article/details/gvdnjestq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/gjyptvsrs.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gmqkwakwc.sHtML

public readonly string $name
来源：http://mobile.sjlbkw.cn/Article/details/gcayejkuo.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gxejhjmoz.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gshigafoq.sHtML

[U51] PHP：数组解构
来源：http://3g.fktsv.cn/Article/details/gjrmmxyiy.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/gljwnpazy.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gpxsaflyz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/gqwaiyujd.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/gtautiwue.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/gusrdbaba.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/godjkzrgf.sHtML

$obj?->method()
来源：http://read.share.tarul.cn/Article/details/gacchvcuu.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gpouttsws.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/grmljvaam.sHtML

[U56] PHP：命名参数
来源：http://mobile.vehdjk.com/Article/details/gnblidkeb.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gevgcysuk.sHtML


<!-- 参考信息 -->