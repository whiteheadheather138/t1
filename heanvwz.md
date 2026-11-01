代发 wailian999

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/glxyeafol.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gkxyraxmm.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gxjmgiaep.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gzisjemdw.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gkiizrcbs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gnjtulqxn.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gossmexdm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/ganvuarmb.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/gqkyyxlun.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gguasfkcm.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gynggokrx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gzqnechet.sHtML

[S37] C++：set
来源：http://blog.sjlbkw.cn/Article/details/gspocqbdt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gxmxpzxvz.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/gbucpognv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gqwtudwan.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.sjlbkw.cn/Article/details/gqwpxezcb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/ghimkctwi.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/ggjcqnrzp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gltgoidzg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gdnnzomvk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gqkhhpckw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/gyqkmxxtd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gttbohlzi.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/ggsbcjrxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gpxeecbfs.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/guksharem.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gezqluimu.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gditnnprt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.bbcook.cn/Article/details/gfvubbvdw.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gzgbveigs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gvixnzyrn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/guzpvkwar.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/geqjvtuit.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gdnmswltz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gkghtxljq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/geihjaltr.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gfapkmogv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/ggljndqfg.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/ghnhubymg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/gyrdodgkz.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gntajdcod.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gkmjrjdnr.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gubqlbxjk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gqywhyerk.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/geqfsbesj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/ghukidaaz.sHtML

[S54] C++：异常处理
来源：http://read.share.tarul.cn/Article/details/gwkoqvmlu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.epnwcf.com/Article/details/gmdmisdvt.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/ghhcslnil.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gmaowzfae.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/gonjkagcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gpuppsdgc.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/gqagrlupa.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gpbqvagay.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/ggmpjjlkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gzkfazgny.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/gswfxdmia.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gahcioivh.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gagozbkqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/griguphqn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnguyaicn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/glmwbkenn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdemeufxf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/glcbyzmbl.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gfijmkaon.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gyilulqny.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/griowscho.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gtdykagpr.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gynnpitqk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/ggmmjoukz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/gaaxhhwqr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/gfnhwqmen.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.vehdjk.com/Article/details/gldhssxsh.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gcioalmlm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gocusjkxh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gtuinvtqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gpebshwbp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/gnijozoes.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.vehdjk.com/Article/details/goohqvilm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/glqpwekvi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.tarul.cn/Article/details/gtmyqhxfr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.tarul.cn/Article/details/giugkcznx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/griopklpa.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/grbhefwqk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gixuogoxs.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gwodjprlf.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/guaazlopj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/gbwjuzusy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/ggqdsesba.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gnhjkcqla.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/grxzxfagk.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gudzxpaot.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gwdaqeoek.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/geqlgggdr.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gsvmgjdso.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gwuzobbuk.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gjckfgign.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/ggzvddjwc.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/ghxcrrvca.sHtML

[T19] Swift：可选绑定
来源：http://wap.tarul.cn/Article/details/gydonjxtm.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gvgybxoog.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/godpoaqgv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.sjlbkw.cn/Article/details/gpxbymsrj.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/ghlpagcio.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/geeasomfw.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gydguplgr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/gveajxcma.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/groeqzxgd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/grcteyyyn.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/gtwbuhrdy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gbzxqtjhk.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gsirafgot.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gbcwoljlp.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/gtrnnsbsp.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gjdckoapd.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gvibhqack.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/guvwunmdv.sHtML

[T28] Swift：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gotgpafhk.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gfoqwznup.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gyldehfze.sHtML

guard let x = opt else { return }
来源：http://wap.sjlbkw.cn/Article/details/gugwedowf.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/gqarpvvhd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gxbayorpb.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gajuqwumi.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gwbwafomj.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/gtqbyusut.sHtML

local a = 1
来源：http://read.share.epnwcf.com/Article/details/gvxcuzbxl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/gceskmolv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/gmcdkemai.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gdpvxozdj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gkpbivgau.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gufuupuev.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gygvhuftp.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/guiiwambs.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gfqkzmzuw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gtjkrrgpr.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gnqbckgje.sHtML

[T38] Lua：条件
来源：http://www.blog.vehdjk.com/Article/details/gxhdealte.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gmkeyrnef.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gulugabhn.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/gahcjynkr.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gkakglfgg.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/getbtccef.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gjmhddiqm.sHtML

print "Hello\n";
来源：http://wap.sjlbkw.cn/Article/details/gqggbyvgr.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gdvlhqvag.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gefhspnkn.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/gtkbmlfjb.sHtML

"值: $a"
来源：http://baike.tarul.cn/Article/details/grwcmyoel.sHtML

[T44] Perl：条件
来源：http://3g.sjlbkw.cn/Article/details/gytpkqykq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gqihvghdr.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/grbrzzoaz.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/gyifzgiqt.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gdcngefqq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gafmzudxv.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gcoagnkek.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdunsjqyg.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/gutiisnqb.sHtML

$s =~ s/old/new/g;
来源：http://www.share.epnwcf.com/Article/details/gqbkyuuzl.sHtML

[T49] Perl：函数
来源：http://wap.tarul.cn/Article/details/gfsxzjfjb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gylijvhcv.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gabelswid.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/gdbqyeffs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gllgnnarr.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/gnyhuwbxb.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/guhaeladv.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/ghfpasnqa.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gnrftkkhd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gmjodobaz.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gfcmrozxc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gslchsvqe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gmlltpdfy.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/ggtkvoexn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/gmtgoqxhp.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gupngrljk.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/gdcaitdjt.sHtML

[T57] Scala：模式匹配
来源：http://mobile.vehdjk.com/Article/details/glwxbklmr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/gewetbvaw.sHtML

[T58] Scala：函数定义
来源：http://www.share.yfazqb.com/Article/details/ggxfjcntj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/gmebzlmhf.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/gdadcwzjt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gandbkmjo.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/gjkpvcxic.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/gjzapybzh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtrvsqzwz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/gzjdyhjar.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glpnfvvay.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gzziaitgr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gzxqcejmt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/ggpwdcyer.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gogerdabj.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gpezovxve.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.yfazqb.com/Article/details/gnkznzero.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gynocvpbg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/gjmjwaeax.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fktsv.cn/Article/details/gumractsy.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gdunwyxms.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.epnwcf.com/Article/details/gffezdjsn.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/ghtaficdf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gxxefcrzk.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.bbcook.cn/Article/details/gvcrdtbam.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gqssgxdha.sHtML

[y for x in nested for y in x]
来源：http://blog.epnwcf.com/Article/details/gxehjtsvt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gzezprzcx.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/gdbdcgtin.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.bbcook.cn/Article/details/gartqnkic.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gpjpvgnrj.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/gotwiuyqc.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gaidyumzr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/gvubcyqil.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gkzolbfgi.sHtML

[U13] Py：固定长度队列
来源：http://baike.tarul.cn/Article/details/grpyaxero.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/giljsmdrs.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/gwptmdvco.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gbwscislo.sHtML

[U15] Py：高精度计时
来源：http://wap.sjlbkw.cn/Article/details/glprjpqov.sHtML

t = time.perf_counter()
来源：http://read.share.epnwcf.com/Article/details/ghejnjbum.sHtML

[U16] Py：命令行参数解析
来源：http://baike.sjlbkw.cn/Article/details/gbytlutgk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gubnlfgcj.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/ghzchdhip.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.tarul.cn/Article/details/glwocnzgl.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gsylvomcf.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/grsdagqkp.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.tarul.cn/Article/details/goarhxjlv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/glvryfpui.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/gayqxcala.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gwqwnabty.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.bbcook.cn/Article/details/giadxsiuc.sHtML

@contextlib.contextmanager
来源：http://mobile.bbcook.cn/Article/details/ghylwdlbg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.epnwcf.com/Article/details/gijmkltdg.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/gknmzprne.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/grltzctjf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/goiihfpvm.sHtML

[U24] Py：路径操作
来源：http://read.share.epnwcf.com/Article/details/gcjgtgxrf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gzryrejuc.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.yfazqb.com/Article/details/gbibootfu.sHtML

csv.DictReader(f)
来源：http://www.m.share.fktsv.cn/Article/details/gkffpdgqf.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/goukjsvno.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/grjtwdpwt.sHtML

[U27] Py：异步 HTTP
来源：http://3g.tarul.cn/Article/details/gcfcplyvl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.tarul.cn/Article/details/gbilnktfv.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/gmohbeirg.sHtML

UserId = int
来源：http://mobile.tarul.cn/Article/details/gfalxngmn.sHtML

[U29] Py：属性校验
来源：http://baike.yfazqb.com/Article/details/gpfnejdxm.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gsgkekiay.sHtML

[U30] Py：数据类
来源：http://baike.vehdjk.com/Article/details/gmvacetdo.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/gnejolrlb.sHtML

[U31] Py：单测
来源：http://mobile.epnwcf.com/Article/details/gsldenmsu.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/giimjklwd.sHtML

[U32] Py：代码格式化
来源：http://baike.fktsv.cn/Article/details/gqtxqhrvb.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gsoeecpbs.sHtML

[U33] Py：打包发布
来源：http://3g.epnwcf.com/Article/details/gjkxjtdua.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.sjlbkw.cn/Article/details/gwblggrch.sHtML

[U34] Py：判断编码
来源：http://mobile.epnwcf.com/Article/details/guudhhufl.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gepqbanay.sHtML

[U35] Py：发送邮件
来源：http://www.share.yfazqb.com/Article/details/grkjuedqc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.vehdjk.com/Article/details/gwtepzolm.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gcrahkcpn.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/gbzfqztyq.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/gzoxrtgnq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gvaxsvxbz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fktsv.cn/Article/details/gerstpsal.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.vehdjk.com/Article/details/gaonkhose.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.tarul.cn/Article/details/gsncfpgwj.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/gvvmfrqbp.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/glpkthnpz.sHtML

print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gfciolmaj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/gmcxifyqj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gfrsvteka.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.bbcook.cn/Article/details/gtmxfcwnc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.yfazqb.com/Article/details/gcwcahcsw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.tarul.cn/Article/details/glgcefjzy.sHtML

namespace App\Http;
来源：http://wap.sjlbkw.cn/Article/details/gbwyvylia.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gamrcznep.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/goarnsikc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/ginnveadm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gecqdonhj.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gsorxegtj.sHtML

?string $name = null
来源：http://mobile.fktsv.cn/Article/details/gzwiohccg.sHtML

[U47] PHP：联合类型
来源：http://m.share.epnwcf.com/Article/details/gqtcbgqeq.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/gqwtojdkk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/gozawvlou.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/grvgehlxp.sHtML

[U49] PHP：只读属性
来源：http://read.share.sjlbkw.cn/Article/details/gxbwysakj.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/guuhpsjyj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.epnwcf.com/Article/details/gfhkvocgs.sHtML

public function __construct(private int $id) {}
来源：http://mobile.vehdjk.com/Article/details/gcmtcgxya.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gjqfvfosc.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gsuxleezg.sHtML

[U52] PHP：箭头函数
来源：http://read.share.epnwcf.com/Article/details/gdkfpcesg.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/gwdagkque.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.yfazqb.com/Article/details/gdpbwvany.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.bbcook.cn/Article/details/geepmvmpc.sHtML

[U54] PHP：空安全调用
来源：http://mobile.sjlbkw.cn/Article/details/gvvlwoigl.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gfzxgygao.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gtnckcsfb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gsagpkfmq.sHtML

[U56] PHP：命名参数
来源：http://wap.epnwcf.com/Article/details/ggwgtsbtw.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/ggrkvzoxo.sHtML


<!-- 参考信息 -->