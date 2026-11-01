代发 wailian999

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gcwthysdq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gnfgsunhk.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/grfssblnj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gqhxiqbyc.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gcjgwomfi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/ggnihudho.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gywleobqy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/ghwdfbmby.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gncyijwyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gyztqkinj.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gkcbkgwqs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gebdktzqa.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gatikoigu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.vehdjk.com/Article/details/gysqlpsxt.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/gpceoeuul.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.vehdjk.com/Article/details/glsahptpr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gvawkwtif.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gvenvqovl.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gcqjszqkk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.tarul.cn/Article/details/gzwmeexhk.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gvigggvar.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/guqkuitnk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.sjlbkw.cn/Article/details/gkcluwhcw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gctnnfajh.sHtML

[S43] C++：智能指针
来源：http://baike.bbcook.cn/Article/details/gzlrxgprr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/grlhpeljy.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gyoeewgjx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gfasbnkef.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gsronglve.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/gzfscbzrf.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gzuuargjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/gjxvidxqa.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gawhbrtxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gupwgnfco.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/glhnzwijw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/gytttwnvu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.epnwcf.com/Article/details/glwgqyjlt.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/ghzmbncsx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkkmihle.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gjndvftke.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gdkimfnhw.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gbawaoskf.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gmkdbouwu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/gampyntzs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/gtmkrdjye.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/glsrcuoio.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.bbcook.cn/Article/details/gbkkutmfv.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gpepnhqlm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/gfekzajkk.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/gdegafzho.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/geojpoyio.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gitaymuuk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/ggpycivur.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gxyajtdip.sHtML

constexpr int N = 10;
来源：http://mobile.bbcook.cn/Article/details/gkjyrcdps.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gpbdyuydv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gayngstsi.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gmlkmvats.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gjnztixjk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gdfebuxej.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gznzhxgdo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gahnyjqze.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gfwhyahia.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmlxduzis.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gvhyqismh.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gtqbucujc.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/grmsiqfll.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gnkcdycpf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/girbrpkbr.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gwxevnxui.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gbnskauwx.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gbtfalqof.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gvrlkgjhr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/glhcwunug.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gwdfnbinw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gqprsyhyb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gossfsyqo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/goshoelpu.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.epnwcf.com/Article/details/gotaqedbc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/glamtqngq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gdfyslcws.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gnbhovqte.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/giasuyzbw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/grzdzncao.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gshhteydq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gjprgczqo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gklpodfgq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/griiruysh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gnxviwnrm.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gmmgoaevw.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gexyrpssu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gngfmkstb.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gkmzcxzeo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/grwugznva.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gbonvqgxl.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gctqpffwn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gybghdnsg.sHtML

var a = 1;  let b = 2
来源：http://baike.sjlbkw.cn/Article/details/gsjapmcxw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gyshjuwid.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/glqezreki.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gflgajmlp.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gsabxowgf.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/goorxyffv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gcrzdmott.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gmrhjbpdg.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/gemjxsolf.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gpewwqdeh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gskuphcdv.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gxepmvplv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/giktjlqxb.sHtML

[T24] Swift：闭包
来源：http://mobile.yfazqb.com/Article/details/gvtmxesbf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gvqqypskt.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gplvqqeul.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gbkvexgqf.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gvscvcith.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/gepyisqlp.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gwcrhyavw.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gkxdgvuwa.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/gjkadjkjv.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/ghobqsntv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gpnxutzhf.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gwuzxtbyi.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/goeqthdjk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.epnwcf.com/Article/details/gwdxnyabs.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gbmbscvcl.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gskyurdwx.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gvbsxvstc.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/grocsqvpx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/geokjfbbd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/gtsxldlzu.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fktsv.cn/Article/details/gtcdwbuxe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gmwkpmfqw.sHtML

[T35] Lua：字典表
来源：http://m.share.sjlbkw.cn/Article/details/gyxqzlqtm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gddcaganl.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gxbhnvglu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/griiiobay.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/gyfgmohut.sHtML

"a" .. "b"
来源：http://m.share.vehdjk.com/Article/details/gasakzpsl.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gwfldkjaz.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gioosxwvr.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/gxuymqxun.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/gpdtuhavo.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gvspllafs.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gjbuingzn.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/gbbwpkvpg.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/ghtpkhipe.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/gvcktlrln.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/gcefwtkzh.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/glatdfwtb.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/gulklnrkz.sHtML

[T44] Perl：条件
来源：http://www.share.yfazqb.com/Article/details/gcqzskvpi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/grojfkhuw.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/ghnbhaccu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gigppwnkl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/galltaxsz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/gemfjlpav.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gvlsmacqa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gqajsqtjb.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gntkuwuti.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/ggmpdahid.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gsfypwwfb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gfvkgeafp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gxwztiglr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gdsbyoyrq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/ghwaagoym.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/guytjucdy.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gbqhkztxj.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/grjfrptvl.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gdojcgrqt.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gapskgnhe.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/goewcljgj.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gkbreedam.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gxyfegksd.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gvcbkxlae.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fktsv.cn/Article/details/gjrfclkuz.sHtML

[T56] Scala：样例类
来源：http://wap.bbcook.cn/Article/details/grxrdpwvy.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/ghdjyamiu.sHtML

[T57] Scala：模式匹配
来源：http://blog.epnwcf.com/Article/details/gduvavwwe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gyykbavvl.sHtML

[T58] Scala：函数定义
来源：http://mobile.sjlbkw.cn/Article/details/ggnbrvwlu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/giyvsxfxr.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gvategntb.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gqhtmpggm.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/godrrumpt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/gjbccsmkh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwwbgkabv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gtyfeubph.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/geyevpuoi.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gxqzjpbve.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.epnwcf.com/Article/details/gskxpemxq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.bbcook.cn/Article/details/gazxobptz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gbnmlhycw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gwululjus.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gcndvjvzz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gasjokndn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.sjlbkw.cn/Article/details/guhcdkqcc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.bbcook.cn/Article/details/gpubvsxzu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gyomaqmpl.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gwybkkzre.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/gbxrqjqin.sHtML

[U07] Py：反转字典键值
来源：http://mobile.yfazqb.com/Article/details/gysvfjkeh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/ggbiccmob.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gqsnyoebz.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gezdwkryu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/gqiatkbdw.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/gwmftcaji.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gjhwljlwp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/geliesrqi.sHtML

[U11] Py：生成器表达式
来源：http://mobile.tarul.cn/Article/details/gjksyrdiy.sHtML

(x * 2 for x in arr)
来源：http://wap.bbcook.cn/Article/details/gjpvmztfh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/glvoiodir.sHtML

Counter(arr).most_common(3)
来源：http://www.share.epnwcf.com/Article/details/glmdiexfi.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/gxfpzotgq.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gnoyyluuw.sHtML

[U14] Py：分组收集到列表
来源：http://blog.vehdjk.com/Article/details/gqheicjah.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/gufpqhvau.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/gloxgoksa.sHtML

t = time.perf_counter()
来源：http://m.share.vehdjk.com/Article/details/gedyvtxai.sHtML

[U16] Py：命令行参数解析
来源：http://baike.yfazqb.com/Article/details/gapkjgopi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.epnwcf.com/Article/details/gnayovzpv.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gfrggfucf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.sjlbkw.cn/Article/details/gwlqlldzm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/ggyuzhdlt.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gowkucfhy.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gpamtqgxp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.vehdjk.com/Article/details/geoncqcvk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gugmxkars.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gzfnkswhm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.yfazqb.com/Article/details/gazwgryuq.sHtML

@contextlib.contextmanager
来源：http://m.share.yfazqb.com/Article/details/gxwqxeagi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.sjlbkw.cn/Article/details/gzbaoowuf.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/gscwgyqmh.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gkkwrtnoi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gqbunfmuk.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/gyeozqxdd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gzrjkvije.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.tarul.cn/Article/details/gtxqebbwu.sHtML

csv.DictReader(f)
来源：http://3g.tarul.cn/Article/details/gpstxqmjz.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gfgycpksq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/gpydevcug.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.yfazqb.com/Article/details/gpknyewqb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.epnwcf.com/Article/details/gnnmgemhm.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/gtuvsodvl.sHtML

UserId = int
来源：http://3g.yfazqb.com/Article/details/gtioelusi.sHtML

[U29] Py：属性校验
来源：http://m.share.fktsv.cn/Article/details/gtzbscrxq.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/garekggkn.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/grxrvupfe.sHtML

@dataclass(slots=True)
来源：http://www.share.sjlbkw.cn/Article/details/gbqhsuyqq.sHtML

[U31] Py：单测
来源：http://wap.fktsv.cn/Article/details/guxvuhiqh.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/gxwbkevgy.sHtML

[U32] Py：代码格式化
来源：http://www.share.vehdjk.com/Article/details/gapggdrjx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.bbcook.cn/Article/details/gvpihpdik.sHtML

[U33] Py：打包发布
来源：http://wap.sjlbkw.cn/Article/details/gmmhhwsvz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/goulkcmkn.sHtML

[U34] Py：判断编码
来源：http://blog.epnwcf.com/Article/details/gzfczyhoy.sHtML

chardet.detect(raw)
来源：http://mobile.tarul.cn/Article/details/gbveobthr.sHtML

[U35] Py：发送邮件
来源：http://wap.sjlbkw.cn/Article/details/giepugsva.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/gflqjpwdk.sHtML

[U36] Py：定时任务
来源：http://wap.bbcook.cn/Article/details/gtkbhugcs.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gmtgjfzya.sHtML

[U37] Py：读写 Excel
来源：http://3g.bbcook.cn/Article/details/gymzwguen.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/gawrayyjm.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gbpunhobv.sHtML

Path(__file__).resolve().parent
来源：http://m.share.bbcook.cn/Article/details/gmgfobxcl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.bbcook.cn/Article/details/gelgsibtm.sHtML

sys.stdout.isatty()
来源：http://www.share.fktsv.cn/Article/details/gvofwcxxt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gobbelpbn.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gyhovlmqg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.epnwcf.com/Article/details/ggcrewcda.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.bbcook.cn/Article/details/gzosllzbq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/gyyttthfo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gjdnxduin.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/gmccgxooc.sHtML

namespace App\Http;
来源：http://www.blog.bbcook.cn/Article/details/gwezuwstn.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.yfazqb.com/Article/details/guohukjjf.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/gczzlcwzl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.yfazqb.com/Article/details/gdzshllec.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/grwamukyh.sHtML

[U46] PHP：可空类型
来源：http://m.share.bbcook.cn/Article/details/guwxjfzbd.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gndiwvwbw.sHtML

[U47] PHP：联合类型
来源：http://blog.epnwcf.com/Article/details/gkxvvatoi.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/gbfkuredl.sHtML

[U48] PHP：纯枚举
来源：http://mobile.yfazqb.com/Article/details/gxcdqyjep.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/gbkqtpjjd.sHtML

[U49] PHP：只读属性
来源：http://www.share.vehdjk.com/Article/details/gfghvknkv.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/gaghykthe.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/gwxvkeaev.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gkrrhmqwe.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/gwgjbbtpp.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/gzxtdetwb.sHtML

[U52] PHP：箭头函数
来源：http://read.share.yfazqb.com/Article/details/goxsztxiw.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.bbcook.cn/Article/details/gwwsqwfuz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.tarul.cn/Article/details/ghnsykvmf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gaqtujzpu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.vehdjk.com/Article/details/gsnoibuzr.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/gwiuxkqhu.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gmokgtqnb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/ggpzaqhik.sHtML

[U56] PHP：命名参数
来源：http://www.share.vehdjk.com/Article/details/goiqlwexc.sHtML

f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gfccgbvcd.sHtML


<!-- 参考信息 -->