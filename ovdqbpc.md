代发 wailian999

memset(a, 0, sizeof a);
来源：http://m.share.fktsv.cn/Article/details/gytzmrbct.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gkqpabwtc.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gkvgzlimi.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gfzfkzwyh.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/geixikzlf.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gsgxhfxdm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gafewtryn.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gxdpeppxf.sHtML

#ifndef X_H
来源：http://3g.tarul.cn/Article/details/grfuczidv.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/genyynnns.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/gwhwloiqr.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gpojrjpve.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/glfwpayhl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gprbjynuy.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/gxyuzrarg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtsfwhab.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gmwqixced.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gzqvxeewz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/gdprojqxl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gnhdbasdh.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gmxwngudn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gwifcfiqa.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gfutfggza.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gwhetyodf.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gsmzvszue.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gzdrlufuf.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gzxoppurq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gzniofoxz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gprkzqxog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/glftxrzds.sHtML

[S40] C++：查找元素
来源：http://3g.bbcook.cn/Article/details/gdqpqerlo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gywqymdal.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gvxvloopt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/getfuvzdk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gsbmwnify.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gvbwxbfsd.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gmhfhyjha.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gyvdzsmhg.sHtML

[S44] C++：引用传参
来源：http://blog.fktsv.cn/Article/details/gtcbhewdf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gcqmixali.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gpqgcegar.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gdchuivdd.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/grbkgacjn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fktsv.cn/Article/details/gspgymmjo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/glwigxjzn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gsdajcpfk.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gcekldvzo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gbzjjpkao.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gsdyrsjin.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/guhcdymkl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/glgbwmncp.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/gwcskoeeq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gxvoarcni.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gvocrdrzs.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gonjzqgqb.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gjomorfrs.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gtapoikgs.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/gvaygxsdr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gxgnempgc.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gydfehthk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gwqencych.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gnnwafzwh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.bbcook.cn/Article/details/gtdpbrdde.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gfsczppfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/guxjgmopk.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gjxsdxgpr.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gvnjwuixq.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gzeaftcxk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gcbolltln.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gutsewjad.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/guppvmbbq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gdcdkjynf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/golqhlybq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grraubpwc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gfgqdcdwj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxhlndcrt.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/glwwmdnke.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/glahvjxqx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/gqbcripai.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/gbugcjyks.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gdjloropx.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gwxcnnolj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gnhoetibx.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/guicixkod.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gnyecaewe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gqxtpsfli.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gsbmdnmev.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gwroqpdjh.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gspgzfuws.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gtmckkeoe.sHtML

[T08] Kotlin：数据类
来源：http://wap.fktsv.cn/Article/details/gnorkxdni.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gfotttfeq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gsesyxfht.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.bbcook.cn/Article/details/gchietfhr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gckpqjhhv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gqfjvedaj.sHtML

[T11] Kotlin：协程
来源：http://www.share.sjlbkw.cn/Article/details/gfuqanztp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/glupruszd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.bbcook.cn/Article/details/gtdgkoddy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/gbajednda.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/guxdmwbzt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gmfseerep.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gkjgowatn.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gaqqvllgm.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gwjircicm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gwqnwhxih.sHtML

[T16] Swift：Hello World
来源：http://wap.vehdjk.com/Article/details/gnddgftmt.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gtaozxwpq.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gdnpexzic.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gmazhnthy.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/gogpqbmkz.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gwlujlpnq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gdppkuhwu.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gdwptofcd.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gjihhjenz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gpochajrp.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gxqhrsfod.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gfrjmtzbd.sHtML

[T22] Swift：字典
来源：http://read.share.bbcook.cn/Article/details/gufhvuxqc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/ghscoevjv.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/gpgmrewco.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gqcwjiugv.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gsoyevpih.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/grywvjtup.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/gdgtgbuqj.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gqwqjtjbh.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/ghbdahkkm.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gzysxeode.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gxnqddzqn.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gvccwivfm.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gpsofthis.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/gkxxikxpi.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/gjjawkjjv.sHtML

guard let x = opt else { return }
来源：http://www.blog.epnwcf.com/Article/details/gccubljxh.sHtML

[T30] Swift：协议
来源：http://baike.bbcook.cn/Article/details/gqmyptoll.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gcsiizxhd.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gtqwjpegp.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/ghfdqanye.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/gblwkblow.sHtML

local a = 1
来源：http://blog.sjlbkw.cn/Article/details/ggmslffcg.sHtML

[T33] Lua：表（数组）
来源：http://m.share.epnwcf.com/Article/details/gtiyyhwdi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/gwcgcsqhu.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gthricerw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.tarul.cn/Article/details/gzpqrocka.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gljsqrolf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gxwexpwyy.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/gqnosniub.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/gdiuhgsfs.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gkuvslcuc.sHtML

"a" .. "b"
来源：http://blog.tarul.cn/Article/details/gjuurezrp.sHtML

[T38] Lua：条件
来源：http://www.share.vehdjk.com/Article/details/gizunjjkr.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/gatplgyyl.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/guopwmsxg.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gpqpceaww.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gnfglgkdb.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/gnxcowyxp.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gqkxflaxx.sHtML

print "Hello\n";
来源：http://m.share.bbcook.cn/Article/details/glgqtpmap.sHtML

[T42] Perl：变量类型
来源：http://read.share.fktsv.cn/Article/details/goqlvgqne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/gfkactwdi.sHtML

[T43] Perl：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gdioqvoax.sHtML

"值: $a"
来源：http://www.m.share.vehdjk.com/Article/details/gjnoagxcj.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/gcfrtqsfc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gvyxxjjyu.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/ghvldgeym.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/ghrvelrnj.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gfkkggsuv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/grdazlzjf.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/ghhspfjim.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/gavbknfkq.sHtML

[T48] Perl：正则替换
来源：http://m.share.bbcook.cn/Article/details/ghzlvwjmf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fktsv.cn/Article/details/glxrksjaq.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gvqbzjthi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gxyqvixll.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gwwhutnyz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.epnwcf.com/Article/details/gwchsyunz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gzyojfaep.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/gcjyimsfb.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/ghsenwjrb.sHtML

[T52] Scala：变量
来源：http://blog.sjlbkw.cn/Article/details/gigkplahv.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/gxvxoudeh.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/gzminmvej.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gzhoiexuo.sHtML

[T54] Scala：集合映射
来源：http://3g.tarul.cn/Article/details/ghuciemxp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gwjdutmww.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gciwvtkbd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.epnwcf.com/Article/details/gajmletzn.sHtML

[T56] Scala：样例类
来源：http://mobile.epnwcf.com/Article/details/gonudeerm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fktsv.cn/Article/details/gltlkjbxq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gcoiktrdu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.tarul.cn/Article/details/gizmftxoa.sHtML

[T58] Scala：函数定义
来源：http://blog.tarul.cn/Article/details/gouqokhxc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.epnwcf.com/Article/details/gieztfkft.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gdkwdbvcy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fktsv.cn/Article/details/ghaviwkqh.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gntufplpt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/glckelxwb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gglusjiah.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gddgiyxlm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghiwhryse.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/grjjsrrhl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gtaevhxwt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gikczurfg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/grbfpgdqo.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/golkofvpv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.vehdjk.com/Article/details/gtthumugl.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/glnjvgado.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/ggdjxblvx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gneqgvwkm.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gknnloicy.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gyzshdpok.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/gxrtexeem.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/gqctxrsux.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/gfbjrvsik.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gacvyomir.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/gnhmdwzxc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.yfazqb.com/Article/details/gljkskiif.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/gybxghrgq.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/ghpvqjwkr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gijeocygr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/gdqunzust.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/ggmcksiky.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/gvmkqelhv.sHtML

Counter(arr).most_common(3)
来源：http://read.share.vehdjk.com/Article/details/gobycrwuw.sHtML

[U13] Py：固定长度队列
来源：http://wap.sjlbkw.cn/Article/details/gmxdghumv.sHtML

deque(maxlen=10)
来源：http://mobile.epnwcf.com/Article/details/gxihfstfx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/gsxknjrvg.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/gggfcaaey.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/gyigaulyb.sHtML

t = time.perf_counter()
来源：http://mobile.fktsv.cn/Article/details/gcmfknnqw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/gqeyzvcqh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/ghvviwvhq.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gorbpfcch.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.sjlbkw.cn/Article/details/gbzxjvrgm.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/geqdbspjb.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/gdiziksro.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.epnwcf.com/Article/details/gtmczgrlh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/gklskhdwl.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/gizsehtsk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gyvdleyxy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.vehdjk.com/Article/details/gdnusdffa.sHtML

@contextlib.contextmanager
来源：http://mobile.epnwcf.com/Article/details/gjrpobcoj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.yfazqb.com/Article/details/gqgwdrdwx.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gxoxmrpys.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gxvdxfhiy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/gzubsligi.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/guucnogbt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gxntdcflo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gzheskzxp.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/gqvrqacdw.sHtML

[U26] Py：并发下载
来源：http://baike.vehdjk.com/Article/details/gyaqbdzpk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.epnwcf.com/Article/details/gejspoqvp.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.epnwcf.com/Article/details/gvdoyjjez.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gsehngrmr.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gbrwmqxze.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/greaislrb.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gxcpobmgm.sHtML

@property 与 @x.setter 配合
来源：http://wap.yfazqb.com/Article/details/gicuwmbky.sHtML

[U30] Py：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gqobfcyvc.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/goqdkgxxz.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gwzhhzghl.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/gkxytgdgo.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gsmfhzmoe.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gmyuwrxly.sHtML

[U33] Py：打包发布
来源：http://read.share.bbcook.cn/Article/details/glmuhpyle.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.bbcook.cn/Article/details/grfvvubhj.sHtML

[U34] Py：判断编码
来源：http://m.share.yfazqb.com/Article/details/geprvllfa.sHtML

chardet.detect(raw)
来源：http://mobile.tarul.cn/Article/details/gxgkqqlrj.sHtML

[U35] Py：发送邮件
来源：http://m.share.sjlbkw.cn/Article/details/gvwnuukqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/getozyjuc.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/grpiqcqmc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gqlywphfp.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/grzszeweu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fktsv.cn/Article/details/grednwggx.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/gfwlrqkdh.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/gkdythkyu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/gppdgpxac.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/gcafnjqtm.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gidwktnkz.sHtML

print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gaakdcgcz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fktsv.cn/Article/details/gcddrcoxk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gyshnxkxa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/grqlxvcyh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gjlrteahy.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/goaeubrlq.sHtML

namespace App\Http;
来源：http://baike.vehdjk.com/Article/details/ghylngtiy.sHtML

[U44] PHP：开启严格类型
来源：http://wap.epnwcf.com/Article/details/gbqwzcmhq.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/glzgvlyas.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/gkqunzmhg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gvkwccqxl.sHtML

[U46] PHP：可空类型
来源：http://mobile.bbcook.cn/Article/details/gibwbnxfy.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gnxxbowcg.sHtML

[U47] PHP：联合类型
来源：http://www.share.tarul.cn/Article/details/gewxxccpr.sHtML

int|string $id
来源：http://read.share.sjlbkw.cn/Article/details/gjzjpfrgr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.bbcook.cn/Article/details/gtqreokut.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gievrboah.sHtML

[U49] PHP：只读属性
来源：http://read.share.epnwcf.com/Article/details/gzngcqewp.sHtML

public readonly string $name
来源：http://read.share.epnwcf.com/Article/details/gyafxujqe.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.yfazqb.com/Article/details/gvhnknlly.sHtML

public function __construct(private int $id) {}
来源：http://m.share.bbcook.cn/Article/details/gsyrtqqfy.sHtML


<!-- 参考信息 -->