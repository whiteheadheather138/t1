代发 wailian999

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gyhysmoxc.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/golhsraqf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gsgmsznux.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gvbbeolex.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gasuukpby.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gqacxmexd.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/glazbwgbt.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/geyrxfmwq.sHtML

#include <iostream>
来源：http://baike.fktsv.cn/Article/details/gxabsvxeh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gkqisagsx.sHtML

[S32] C++：字符串
来源：http://3g.epnwcf.com/Article/details/gnhpnpsdr.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gsdwokwoe.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gmscaqbos.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/grexjptaz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.sjlbkw.cn/Article/details/gjlmvfmaf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gicolfgrb.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/gfnwslmoi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/giamixrhp.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gcmbqclwz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gxfeamqee.sHtML

[S37] C++：set
来源：http://baike.vehdjk.com/Article/details/gyceuupck.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/ghikqgevz.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/gfiqccazf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.tarul.cn/Article/details/gxwtcarux.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/ggwrroaqa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gzbkbwiek.sHtML

[S40] C++：查找元素
来源：http://mobile.bbcook.cn/Article/details/gwiipcwjk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gnncqoedt.sHtML

[S41] C++：类与构造函数
来源：http://3g.yfazqb.com/Article/details/gtmcctrjl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gswiexzim.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtldblmel.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gsldppswq.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gmxfazpai.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gbyygrfft.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/ghrhfssha.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/ghmnqgugv.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gphyafdga.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/gqyxobwto.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gpndxrgzz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gmzkggziq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gqnawznny.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/gnrddnebb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gfcpxketq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/gxsdwmeou.sHtML

while (std::getline(in, line)) { }
来源：http://wap.yfazqb.com/Article/details/gyjspncxl.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gflwwgobu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.vehdjk.com/Article/details/glgtkysrn.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gwwjaryex.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/gupwpaubh.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gpsnpsalw.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/gpgoxuhgq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gxxfvupwx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.epnwcf.com/Article/details/gqvjddefh.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gdribnhux.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/gmadoykat.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gqgwekjaa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gxiyehesx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gzphvswwp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gbqwognzp.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gdyiqxlai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/gkhyermrr.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/ggihppnhd.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/gsliipfnx.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/gxiiewmtm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbybkosa.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/grlzmossm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gssrkbvwf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/ggizdgigo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gynvzxjtu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdftcngnu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/grduaklcg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmnsuuqqq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gdilefugk.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gxbszgjky.sHtML

[T02] Kotlin：变量
来源：http://wap.epnwcf.com/Article/details/grqlfdemd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gbwpaonua.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/grcrgiyds.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gzsefkdam.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gjtezzmyp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/guxiniwef.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gugpuplsd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gwbaoskcm.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gfbcieunz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gapdgtbdu.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gabpkgyec.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gotgtseij.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gxsuhmgqm.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gvmlmxkuf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gwwgiwlzv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/ghibdshob.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/ghiepjekw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gumssgdec.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/gdwjdwrza.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gtyinlwxc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/gnbiclidz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gkydwzqki.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.tarul.cn/Article/details/gwpirqcvn.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/gruzpggei.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/geubpxhcv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gkohmaulx.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gbprorsck.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gngtomstk.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gvpsulwpj.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gpvckfyvt.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gszmcmouj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gipmcqwnw.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gfifayxpd.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gqdvfwzrv.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gnysdkwmv.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/gtxyzsqnv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.bbcook.cn/Article/details/ggsjmkcpb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gffwbqezn.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/giirlulpg.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gwgidfokb.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gvknokxmp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gobzxlogf.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/gdljanygq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/gvtstpyqg.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/glwpaimld.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.tarul.cn/Article/details/gfaktamqp.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gdvxxrxdc.sHtML

struct P { var x: Int }
来源：http://blog.epnwcf.com/Article/details/gpgjxbicd.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/gsojkrqov.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/gqzbysgdz.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gbcgpphgf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gflugilim.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gzzpexxst.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gdaqfhquz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.yfazqb.com/Article/details/gpyzopwdl.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/gmdabticn.sHtML

[T30] Swift：协议
来源：http://www.m.share.tarul.cn/Article/details/geuksektc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.epnwcf.com/Article/details/gvfrhcpws.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/granivttg.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gaoyqpcqc.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/grecqarvf.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/grndfyixq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fktsv.cn/Article/details/glfewtcqj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gpagauxhk.sHtML

[T34] Lua：遍历表
来源：http://m.share.tarul.cn/Article/details/gmdaccelq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/grtjufxte.sHtML

[T35] Lua：字典表
来源：http://www.blog.vehdjk.com/Article/details/gaqfewnqk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.tarul.cn/Article/details/gibdwtndq.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gwbygqebh.sHtML

function add(a, b) return a + b end
来源：http://mobile.sjlbkw.cn/Article/details/gpaxxbmyl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gcctrvtmo.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gqkrhymjv.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gzlimujaj.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gaaxnkjis.sHtML

[T39] Lua：模式匹配
来源：http://blog.epnwcf.com/Article/details/gvwiczjdj.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/gjfjfsgxk.sHtML

[T40] Lua：元表
来源：http://www.m.share.fktsv.cn/Article/details/gniotstog.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/godhayeqs.sHtML

[T41] Perl：Hello World
来源：http://3g.fktsv.cn/Article/details/gwmaexbcm.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gvshkecrg.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/grrclceia.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.yfazqb.com/Article/details/gglmmdled.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gotisgmit.sHtML

"值: $a"
来源：http://www.m.share.vehdjk.com/Article/details/gbmkgzzjs.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/gzetyzpib.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gczrmfupr.sHtML

[T45] Perl：数组遍历
来源：http://blog.sjlbkw.cn/Article/details/gjbwziedl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.vehdjk.com/Article/details/gvwbuxdaj.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gzqxtmnzz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gzdgyygwy.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fktsv.cn/Article/details/guvudeugq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gongjwgrv.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gnsckwjul.sHtML

$s =~ s/old/new/g;
来源：http://blog.yfazqb.com/Article/details/gxgfpztns.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/gkphxrymp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gozxmitps.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gswqengkb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/grpmimaxy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gnxquqprv.sHtML

[T51] Scala：Hello World
来源：http://www.share.epnwcf.com/Article/details/godwowwjk.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/greiajsfh.sHtML

[T52] Scala：变量
来源：http://read.share.tarul.cn/Article/details/gitgezvqd.sHtML

val a = 1;  var b = 2
来源：http://m.share.vehdjk.com/Article/details/gabqltgrm.sHtML

[T53] Scala：字符串插值
来源：http://www.share.vehdjk.com/Article/details/ghhmuxssp.sHtML

s"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/glwkcxins.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gbnhwtenx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gpibmwbou.sHtML

[T55] Scala：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gynxtizyb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.bbcook.cn/Article/details/gaitcggwp.sHtML

[T56] Scala：样例类
来源：http://wap.fktsv.cn/Article/details/ghdrkvydn.sHtML

case class User(name: String, age: Int)
来源：http://3g.bbcook.cn/Article/details/gilzhqqoe.sHtML

[T57] Scala：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gxgwfqnyt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.tarul.cn/Article/details/gmtfqcham.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gsytrcqjh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.bbcook.cn/Article/details/gueefqeje.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gldewioau.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gigfyyeee.sHtML

[T60] Scala：折叠
来源：http://m.share.fktsv.cn/Article/details/glynnsjqf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/gmkmqmxjz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfmaupjcw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gcxuzwhnl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpbgfxteq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/guvqdujtq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gbbnktvwe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gfuwfufkc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/geiojutbk.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.vehdjk.com/Article/details/gbslmvjos.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.vehdjk.com/Article/details/gnmtyzchg.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gcunwloix.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.tarul.cn/Article/details/gzrbzobjx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/grizovume.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gvnosfvmx.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gjdofinbe.sHtML

{**a, **b}
来源：http://read.share.tarul.cn/Article/details/gcgrpopwn.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/goxdtjjie.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/gysdhkuau.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gqkwesrlb.sHtML

[y for x in nested for y in x]
来源：http://3g.yfazqb.com/Article/details/gmkzofgjz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.tarul.cn/Article/details/ghchkyjbb.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/gscqbucak.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/grjawuscv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gzjojiyfl.sHtML

[U11] Py：生成器表达式
来源：http://blog.epnwcf.com/Article/details/gyglaammf.sHtML

(x * 2 for x in arr)
来源：http://www.share.bbcook.cn/Article/details/ghlrqmosr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/greqhirtv.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gzoqmmbbe.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gntqxqghl.sHtML

deque(maxlen=10)
来源：http://3g.vehdjk.com/Article/details/grepskysq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/gctgmfutv.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gecbdeere.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/glrbynlej.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gdapuixbs.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/gvqwhkotu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gzwgrsazw.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gylcalxlf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gdrzbmimt.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gaddoomrd.sHtML

pat = re.compile(r"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gezipteie.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.bbcook.cn/Article/details/gexotgvia.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gqeeyngrg.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/gejttuhab.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.bbcook.cn/Article/details/gettpyqik.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gjsnkmswe.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gaxdvpfsh.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gkqundnpd.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gcvrdwteg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.tarul.cn/Article/details/gfwpmfxgx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/gimoldcia.sHtML

[U24] Py：路径操作
来源：http://read.share.tarul.cn/Article/details/geubcwojy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/ggtquewpu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gwzhbqihp.sHtML

csv.DictReader(f)
来源：http://www.m.share.tarul.cn/Article/details/gsgmcptwk.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gynryxgyh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/guefyawme.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gcivmvwdf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gkampwvot.sHtML

[U28] Py：类型别名
来源：http://read.share.sjlbkw.cn/Article/details/gskmxhojv.sHtML

UserId = int
来源：http://wap.bbcook.cn/Article/details/gpjdhmpwt.sHtML

[U29] Py：属性校验
来源：http://www.m.share.tarul.cn/Article/details/gewewzfhk.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/gygtlmkid.sHtML

[U30] Py：数据类
来源：http://3g.bbcook.cn/Article/details/ggajasjjl.sHtML

@dataclass(slots=True)
来源：http://www.m.share.yfazqb.com/Article/details/gjmegtito.sHtML

[U31] Py：单测
来源：http://wap.bbcook.cn/Article/details/gnnqymadh.sHtML

python -m pytest -q
来源：http://www.share.tarul.cn/Article/details/ginapfmrm.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/gdazuykqy.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/ghrgcdqos.sHtML

[U33] Py：打包发布
来源：http://3g.yfazqb.com/Article/details/gtskijxvi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fktsv.cn/Article/details/gmegtlsgh.sHtML

[U34] Py：判断编码
来源：http://www.blog.fktsv.cn/Article/details/gtktttcvm.sHtML

chardet.detect(raw)
来源：http://www.share.epnwcf.com/Article/details/goijgsiaq.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/gxpokxodg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/gfkynuhpg.sHtML

[U36] Py：定时任务
来源：http://baike.yfazqb.com/Article/details/gzapwdjvu.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/guefnkmez.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.yfazqb.com/Article/details/gnyzzkpas.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fktsv.cn/Article/details/gzuycetld.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/guwqasxdo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.bbcook.cn/Article/details/gpbcwmwse.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gwvwvagry.sHtML

sys.stdout.isatty()
来源：http://blog.tarul.cn/Article/details/gqixwnlfl.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/gqcjqrisu.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gflfaogtz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/gwzlmgrrm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/gamaluenw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.sjlbkw.cn/Article/details/gsmwixpvq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gulghlous.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/gjuknkydu.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/garwnvrgc.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gqeyhmjns.sHtML

declare(strict_types=1);
来源：http://www.blog.epnwcf.com/Article/details/ghvztjvkj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.tarul.cn/Article/details/gnigfilor.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gkkleonfu.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gaclxiwlj.sHtML

?string $name = null
来源：http://baike.fktsv.cn/Article/details/gistyltce.sHtML

[U47] PHP：联合类型
来源：http://baike.epnwcf.com/Article/details/gxreheftn.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gjxoukeuy.sHtML

[U48] PHP：纯枚举
来源：http://baike.tarul.cn/Article/details/gqbddiylt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.bbcook.cn/Article/details/gpuqxtvzt.sHtML

[U49] PHP：只读属性
来源：http://read.share.yfazqb.com/Article/details/gwvzpngqd.sHtML

public readonly string $name
来源：http://blog.yfazqb.com/Article/details/ggrvkgrff.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gkequuslq.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/gfrefstrm.sHtML

[U51] PHP：数组解构
来源：http://wap.epnwcf.com/Article/details/gmkfnjdvs.sHtML

[$a, $b] = $arr;
来源：http://mobile.vehdjk.com/Article/details/gwyjzvyfb.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gdplktxkm.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/ghjqzxhmp.sHtML


<!-- 参考信息 -->