代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gczxinxoa.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gvupxpxfj.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gsmroegtu.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gizgwfjvt.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/gxshdfaat.sHtML

[S29] C：变参函数
来源：http://mobile.vehdjk.com/Article/details/garnrizaz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gxardxoks.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gpnhajbfm.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/guufobzly.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gghqhigoz.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gkaujaqpx.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/ghbzkflim.sHtML

#include <iostream>
来源：http://www.share.sjlbkw.cn/Article/details/gbyzfferl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/giyfsucaz.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gvobamglc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/glsrotjjp.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/genrwgcui.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/gzgbqtqqb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/goyqpdvcn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gpplhrbxy.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gegirfwds.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/geyvuvkkt.sHtML

[S36] C++：unordered_map
来源：http://baike.sjlbkw.cn/Article/details/gwkkrnlqb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gfymwamds.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gfznjcwmj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gqxwhtagc.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gmqdfxisu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/grcrldpzp.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gxkiwomqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gfjhfptha.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/gonemczmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gtmfrggpg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gfolvwicw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gjkhohwnj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/gpvpnagtu.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gotsevjgg.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/galnmxzil.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/gbkncaoej.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gamvbqxpv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gfzysawxt.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/gkmmoywxb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/grizfhuqf.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gqwsjtplo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gpccmyyfe.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.vehdjk.com/Article/details/gjmntdqcs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gueitjioy.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gmditlulz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/ggrjaksgq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gkmxqbmgo.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/ghcqiwgrq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gciglgvga.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gkfwengfp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gastsklmk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gumcxojyn.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gqoyqvvnk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.epnwcf.com/Article/details/gsmkeuazm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gacelkxti.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gnvzlpwmw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/ggvmtxiap.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gedgcbzsz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/gnqnaguux.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gckqkuvzh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gpjjwylmw.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/gioeayirg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnltjtlqy.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gpdkonmfa.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gjosdhvqh.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gdsyitppi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/grnzxdxff.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/gigfkikzv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/gcqtuwvri.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gebpwqdaj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/giplckmie.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqutvtavh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gpdqmyife.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkeajwzsj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/gswquctpg.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gerslvcwh.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gzahmjskx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/gqiaqufjs.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.vehdjk.com/Article/details/gmguybhcv.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/gziwhvuil.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/gpbugftzs.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gquwiiwss.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/glfcckebu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/gmipvpdkj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gfbukofuf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gmedjycnn.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gbyrfrvoa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gcvdyjdes.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gbdybafdq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gtbfqnhwh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/girvqeanr.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.yfazqb.com/Article/details/gsfigcccc.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gzwyxvjvf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gavxsoiss.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/gwycrlvyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gfhltkfhf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/gfwdmcvll.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gyhnimphp.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/gznubesgw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/goejtdbky.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gfusyfkwx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/guwycjula.sHtML

[T15] Kotlin：接口
来源：http://read.share.bbcook.cn/Article/details/gguoyuucz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gztxtfhiz.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gxmjiuubs.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gjgqftpgf.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/giihzxjbo.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/gydelfknu.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gjelrujxc.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gwaymiizo.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gizbkhhau.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gjpdqwwmz.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/guvqdmrcb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gzcwrxsgv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.yfazqb.com/Article/details/gawreuswq.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gqmypajhi.sHtML

[T22] Swift：字典
来源：http://www.share.tarul.cn/Article/details/gvfnrzlsf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gxkjofgqr.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/ghyjhhlsc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gmdvdnzol.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/gkltjkmnm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/glbdameso.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/grhhausrw.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gzsknwyga.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/ghnrnebft.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gfljxuhja.sHtML

[T27] Swift：错误处理
来源：http://www.share.vehdjk.com/Article/details/gtyaufjfr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gfoayjdez.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gywhngnln.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gscgxhzxt.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gdydmzdmx.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/gymxmeeeb.sHtML

[T30] Swift：协议
来源：http://blog.sjlbkw.cn/Article/details/gfutobhox.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/guzefpckv.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gmmldnolr.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gexhwpwfa.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/gjsxtortl.sHtML

local a = 1
来源：http://www.share.sjlbkw.cn/Article/details/gqltebzvp.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/gkluuxlgu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.sjlbkw.cn/Article/details/ggwnrfnlh.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gzlutjwij.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gmwqrhqzm.sHtML

[T35] Lua：字典表
来源：http://3g.epnwcf.com/Article/details/ghkndvltv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/glchorfng.sHtML

[T36] Lua：函数
来源：http://www.blog.fktsv.cn/Article/details/gacjkupku.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/gawggarxn.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gjvqswsww.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/guvbbpjif.sHtML

[T38] Lua：条件
来源：http://wap.epnwcf.com/Article/details/gmnujiigb.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gemrvksea.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gnncxmalm.sHtML

string.find(s, "%d+")
来源：http://www.blog.bbcook.cn/Article/details/gihawkavr.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gccnxxgme.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gonaeniey.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/grvnkbbhy.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gwzkvcyvg.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/grdbcpmlc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gcbqvynpo.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gwhewlwst.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gheljerzp.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gmulaaook.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gfmixzfuu.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gbvpcmign.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gbqpqhbhx.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/grmninpyv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/gcxzcoeqt.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gzzmwpqsg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gxnldoebo.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/gvgaapvkb.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gmhtpjwpq.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/ggsuhtuid.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gafhrwqbr.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/grqjdyolb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gawwrfquq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.vehdjk.com/Article/details/gsymglvow.sHtML

[T51] Scala：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gusmikdfw.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gcylgdvhq.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/gzwlonnbs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/ghccprtts.sHtML

[T53] Scala：字符串插值
来源：http://baike.epnwcf.com/Article/details/gmubqatjb.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gpkplbnky.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlcipmxf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gbpexulym.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/grxwhdawi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.yfazqb.com/Article/details/gxoekqtct.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/gxigebeke.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/grgjoblzb.sHtML

[T57] Scala：模式匹配
来源：http://3g.tarul.cn/Article/details/gaaukdzrf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gngnpqhde.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gyvwegpnq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fktsv.cn/Article/details/gqrdxqoov.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/grnpjdujt.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/guplvzkbp.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gbkpnxuem.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.epnwcf.com/Article/details/gwofrigjv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghyrodqaa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gulmlwpkm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/garybvvuh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/gjryzonpi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gcnbsyphm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/gjkazpiik.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gnzldshkx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/grlzheqtb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/gfoquzcik.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gqwoexkqr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/ghmjeerss.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gtkyjpctb.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gitpvdvtg.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gwnkonvcr.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gzmehxrzp.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/gjdqwgasb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gulytppic.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/gdvlaphmh.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gltobyljz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gmikxrfrf.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gulvwiogr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gzxqqjjdv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.vehdjk.com/Article/details/ggoodhkms.sHtML

[U11] Py：生成器表达式
来源：http://m.share.yfazqb.com/Article/details/gnkrfzmhd.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gmdtptoyw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/gsjuftscg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/gdvuaiiwo.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.vehdjk.com/Article/details/guspezvev.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gziulkvxx.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/ghgkxtxtc.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gqxhzofjs.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/guouhyfvi.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/ggyujwjhn.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/gylwugors.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gdaukpskn.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gzpdzuvfh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.tarul.cn/Article/details/gcghmmrpw.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gstklpjhh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/gjwuoyzpk.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/gnffjoabg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fktsv.cn/Article/details/giehzandj.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/gcfnaelae.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/gurvkwtsc.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gbauedgwp.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gkmabgfxa.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gfktadoiu.sHtML

list(zip(*m))
来源：http://3g.sjlbkw.cn/Article/details/gloahrhde.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/gphkeafzp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.bbcook.cn/Article/details/grzwvtvkb.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/ggmeakqzf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gthjywwki.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.bbcook.cn/Article/details/gexswvnle.sHtML

csv.DictReader(f)
来源：http://baike.fktsv.cn/Article/details/grzbazulh.sHtML

[U26] Py：并发下载
来源：http://www.share.bbcook.cn/Article/details/ggzfysdpu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.bbcook.cn/Article/details/gmxghcfvy.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.sjlbkw.cn/Article/details/gwgkgyvrt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/gldjbdogb.sHtML

[U28] Py：类型别名
来源：http://m.share.vehdjk.com/Article/details/gdmvwdhgr.sHtML

UserId = int
来源：http://www.m.share.vehdjk.com/Article/details/gyzmsnwah.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/gkvsutvhx.sHtML

@property 与 @x.setter 配合
来源：http://wap.epnwcf.com/Article/details/ggnsivanv.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/gtuyfxzaw.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gbtjnokhg.sHtML

[U31] Py：单测
来源：http://blog.tarul.cn/Article/details/gwakvhurl.sHtML

python -m pytest -q
来源：http://3g.yfazqb.com/Article/details/gxtxhmrya.sHtML

[U32] Py：代码格式化
来源：http://3g.sjlbkw.cn/Article/details/galkpakvu.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/ggqfhdrql.sHtML

[U33] Py：打包发布
来源：http://baike.bbcook.cn/Article/details/gkvbktpdf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.bbcook.cn/Article/details/godhlhrka.sHtML

[U34] Py：判断编码
来源：http://mobile.sjlbkw.cn/Article/details/gfaicybko.sHtML

chardet.detect(raw)
来源：http://www.share.epnwcf.com/Article/details/gvpxmmflw.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/gfihgtytk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.epnwcf.com/Article/details/gzceujqqt.sHtML

[U36] Py：定时任务
来源：http://blog.epnwcf.com/Article/details/ggljtkfvq.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.yfazqb.com/Article/details/gonntxdlb.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/gnoerqrnc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.sjlbkw.cn/Article/details/goagmahpv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.bbcook.cn/Article/details/griaflsbx.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gouiphruk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.yfazqb.com/Article/details/givczbrxq.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fktsv.cn/Article/details/gstoexymm.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fktsv.cn/Article/details/gthkmyehj.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gyhdxlfmq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.yfazqb.com/Article/details/gghmuimrb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.epnwcf.com/Article/details/gotercqdl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/gfnsmjlip.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.vehdjk.com/Article/details/gglxusxnc.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gzglwzhjf.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gprdkakbr.sHtML

[U44] PHP：开启严格类型
来源：http://wap.epnwcf.com/Article/details/guigctiyd.sHtML

declare(strict_types=1);
来源：http://read.share.sjlbkw.cn/Article/details/grlgdfoqk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.tarul.cn/Article/details/ggwxuxbyu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gtmwneiew.sHtML

[U46] PHP：可空类型
来源：http://wap.bbcook.cn/Article/details/gsoxaapga.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gxcbqaesc.sHtML

[U47] PHP：联合类型
来源：http://www.blog.tarul.cn/Article/details/gxyzibagp.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gizwdipfn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.yfazqb.com/Article/details/gknkdiisk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fktsv.cn/Article/details/gxedrnidr.sHtML

[U49] PHP：只读属性
来源：http://www.share.fktsv.cn/Article/details/gtnocxokm.sHtML

public readonly string $name
来源：http://blog.sjlbkw.cn/Article/details/gdvsunxla.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gqnreyyvy.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gzfzxaaxb.sHtML


<!-- 参考信息 -->