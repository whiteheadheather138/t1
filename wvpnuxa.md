代发 wailian999

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gbwzttzin.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gsjkkohrf.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gnirerhjw.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/goiaffyru.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/guvxyqfek.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/gyzruryzl.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gdeinbipb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/ggmghgalx.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gpzbwnvel.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gqmuqacbp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gocdtcpay.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gmtiodxge.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzqzuezl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gunnhemai.sHtML

[S36] C++：unordered_map
来源：http://read.share.vehdjk.com/Article/details/gvddnqryy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gnkeprzbl.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gazmjywrt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gxcieoklf.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gyzgtgxmp.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gfebeolnw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gglnfwgvk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/giuoewlox.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gjkhknbzk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/grpeyzudb.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gqmathqvi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gdzhtfnca.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gdzakrlzh.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gnmenalau.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/gnqemoatz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/ghkvxfolf.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gmjmvbvph.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/gppajcgag.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gfqqgaqst.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlqjjorb.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gzpezwjrq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/glsazydcn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/gcqxyvzou.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gglpztkjr.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gkuupvoxe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.vehdjk.com/Article/details/giaqjcvam.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gczsemdeq.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/ghittshtr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gfrpulhuy.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gnoswxjto.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/gguiwjnhe.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/guoiskofj.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/glwvvjgsr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/gxchfgpyd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gioltnfym.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gizykwsqu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gpxnqncwt.sHtML

[S54] C++：异常处理
来源：http://read.share.tarul.cn/Article/details/gpfxrdojg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gwnfucewj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/guydwzwed.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gsliuzadj.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/guzpxhvfk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/galzugidt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gbmgkpyeu.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/ghpczichk.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/grgodqdph.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gtoopljsw.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gximpomyq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/glljuenyp.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/grlbhmwfr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/gneemwbhs.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpppsonfl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gmnqzdvyw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gncgowyvm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.tarul.cn/Article/details/gkxmmvvkz.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gzrrrvlur.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/girnngzlm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/guicrhmfe.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gpkvxsczo.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gfgfbqfcp.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gfzecwgzt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gkmgmkksl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.yfazqb.com/Article/details/gnbiebniz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/ghmnrdnre.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gkgsuiksr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gczpuwqtr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/gxhucjxya.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gzboorpqn.sHtML

[T08] Kotlin：数据类
来源：http://baike.vehdjk.com/Article/details/ggobayrzl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/ggfilprsj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gygqpehos.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.bbcook.cn/Article/details/gmalogqkk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gzanzaaxr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/goxuueazd.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/gncqambtk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzokhyzim.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/gbbyzboos.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gftudspeo.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/gqlbxsdoq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/ggadzibnw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gjjsaymij.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gxplhqrlc.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gbmaywtsi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gugwcxfqk.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/ghobiiidt.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gvplqmacx.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/giqgogamf.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/ggtbrpuca.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/ghhjchvli.sHtML

"值: \(b)"
来源：http://read.share.fktsv.cn/Article/details/ghreawjtx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.sjlbkw.cn/Article/details/grctqaccc.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/glfjyinpx.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gxwnbuokl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gkqlowqki.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/glqgurkgg.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gfdjlwijp.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gznkwvkum.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/gmupyjfmy.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gogffwxod.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gjguaetzw.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gwcrgtlzq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnzqjwgj.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/guvunhfyv.sHtML

struct P { var x: Int }
来源：http://mobile.fktsv.cn/Article/details/gvgglqsuw.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/ghpsjdkwo.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/gejpyxwkd.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gupwbyavm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.vehdjk.com/Article/details/gwwbffxll.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gxeipdrpd.sHtML

enum Color { case red, green }
来源：http://www.share.tarul.cn/Article/details/grscjaorz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gpanbkxzb.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/gxyaisqfv.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/gkhdqcatr.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fktsv.cn/Article/details/gsonnartc.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/guqwcnmnt.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gbyvtobit.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gohctdbmh.sHtML

local a = 1
来源：http://wap.epnwcf.com/Article/details/gyzzsxpps.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/goaptmxmn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/ghiwewcgu.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gkoavutas.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/glmxcyhuk.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/gaqkuqmqr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gkqudgnxa.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/gcvuxbyae.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gjgbggrtr.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fktsv.cn/Article/details/gukvlnpcf.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gcbuwphtt.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/guvnynfns.sHtML

if x > 0 then print("正") end
来源：http://www.blog.tarul.cn/Article/details/gevhuxrnx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.tarul.cn/Article/details/gjfganrqm.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/ghhdsfvng.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/gwjuzcqph.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/ggwkmiunn.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/ghcjubhzy.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/gfvauiuvl.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/glvpmjefk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.epnwcf.com/Article/details/gaakiqprv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gjzyvysog.sHtML

"值: $a"
来源：http://wap.fktsv.cn/Article/details/geblhrdrd.sHtML

[T44] Perl：条件
来源：http://read.share.vehdjk.com/Article/details/guskenpdi.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.bbcook.cn/Article/details/gzkinilza.sHtML

[T45] Perl：数组遍历
来源：http://mobile.vehdjk.com/Article/details/gnpdkgosb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gsuwmvito.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gacpelwsn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/grkhwmjgy.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/gyenxjffa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gxdiptevv.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gkifogiuz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/gehiojhxj.sHtML

[T49] Perl：函数
来源：http://mobile.bbcook.cn/Article/details/gsgnqthpg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gbclbxhlo.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fktsv.cn/Article/details/getfwqpke.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.tarul.cn/Article/details/gcjdexaiy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gpbvotert.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gvjefrhyj.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gjqtbhvps.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gbsaouggl.sHtML

val a = 1;  var b = 2
来源：http://baike.tarul.cn/Article/details/gimrpbzvh.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gtedizzjx.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gbinrudlg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gpdldtblp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/gcnmpmjnw.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gwlrrealj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.yfazqb.com/Article/details/ghcwawlmg.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gqodldbub.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gmscoqhem.sHtML

[T57] Scala：模式匹配
来源：http://baike.fktsv.cn/Article/details/gyzgbhqge.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gyffmhxkg.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gmopluudq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/glgxxwtip.sHtML

[T59] Scala：循环
来源：http://baike.sjlbkw.cn/Article/details/gempehazu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gngvjvwhs.sHtML

[T60] Scala：折叠
来源：http://www.share.fktsv.cn/Article/details/gdfdlbczu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gebqatwut.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghotxesqc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gkhemblsc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmomncyse.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gvgjrfncc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.sjlbkw.cn/Article/details/gqrwoduup.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gexedhvdj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.sjlbkw.cn/Article/details/ggfosaywc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.sjlbkw.cn/Article/details/gmejbrksl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gywdlnabi.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gvhvswmdy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fktsv.cn/Article/details/gelxslitc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/gsjhkhubj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/grivlbtxv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/gdpjashct.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gkskxrryr.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/gdlhwbotl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.epnwcf.com/Article/details/ggamkwnpj.sHtML

[U08] Py：展平二维列表
来源：http://baike.vehdjk.com/Article/details/gaoascueu.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gtgnmtmxz.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gavuehdjk.sHtML

max(d, key=d.get)
来源：http://www.share.fktsv.cn/Article/details/gfwazvihw.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/godtfdair.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gqzidqdnu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gzoczbvtw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gpacvlzgw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/gxgmwcfyp.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/gxmxpptmk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/guzzdwlqq.sHtML

deque(maxlen=10)
来源：http://m.share.fktsv.cn/Article/details/gjhrzygvz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gbbrfuplv.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/gdcnraphm.sHtML

[U15] Py：高精度计时
来源：http://blog.sjlbkw.cn/Article/details/ggdjydavl.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/glfwlghzu.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/gqpekzelb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/guoewkfkz.sHtML

[U17] Py：初始化日志
来源：http://m.share.fktsv.cn/Article/details/gpepjqiwy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.epnwcf.com/Article/details/gyeskntsf.sHtML

[U18] Py：预编译正则
来源：http://baike.epnwcf.com/Article/details/gnvldfypd.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gfzzwknlh.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.yfazqb.com/Article/details/ghteripey.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gpynooevd.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/gibkgtpjm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gxketweht.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fktsv.cn/Article/details/gjeocwljd.sHtML

@contextlib.contextmanager
来源：http://mobile.bbcook.cn/Article/details/gvmrmsfdy.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gwfkjzaca.sHtML

list(zip(*m))
来源：http://www.share.tarul.cn/Article/details/gzduqvqum.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gunmxogiq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fktsv.cn/Article/details/gcmvllxyv.sHtML

[U24] Py：路径操作
来源：http://www.blog.yfazqb.com/Article/details/gcsklksmm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gbvtexcwl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/gieujnjok.sHtML

csv.DictReader(f)
来源：http://3g.vehdjk.com/Article/details/gplmzmbcx.sHtML

[U26] Py：并发下载
来源：http://blog.tarul.cn/Article/details/giytdxtew.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gkvtndqja.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/grusxbxem.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/gsqhytcqd.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gbawfrqmi.sHtML

UserId = int
来源：http://3g.sjlbkw.cn/Article/details/grxvfliyr.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/godcomshp.sHtML

@property 与 @x.setter 配合
来源：http://mobile.epnwcf.com/Article/details/gumazmxty.sHtML

[U30] Py：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gqbypsrqa.sHtML

@dataclass(slots=True)
来源：http://mobile.yfazqb.com/Article/details/gdraczldk.sHtML

[U31] Py：单测
来源：http://mobile.tarul.cn/Article/details/gqewkwvvv.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/glogktkmp.sHtML

[U32] Py：代码格式化
来源：http://read.share.bbcook.cn/Article/details/gfoeprnpk.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.epnwcf.com/Article/details/glgaibcig.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gvzkacrti.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.epnwcf.com/Article/details/gvbzlvjdi.sHtML

[U34] Py：判断编码
来源：http://m.share.tarul.cn/Article/details/ggzxkffbw.sHtML

chardet.detect(raw)
来源：http://m.share.bbcook.cn/Article/details/goigodyyw.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/glsjqbyxl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fktsv.cn/Article/details/gfuzmhwkv.sHtML

[U36] Py：定时任务
来源：http://read.share.yfazqb.com/Article/details/ggyguwycm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.vehdjk.com/Article/details/gtggxkrew.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/gcwrtnygs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gsdjfbkgm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/geuvebcoa.sHtML

Path(__file__).resolve().parent
来源：http://blog.sjlbkw.cn/Article/details/gbuuglwuj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.yfazqb.com/Article/details/gqkkictau.sHtML

sys.stdout.isatty()
来源：http://blog.epnwcf.com/Article/details/grmbtbbrw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gpvutqyjf.sHtML

print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gaoqpnofz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fktsv.cn/Article/details/grpwiysyy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/ghkeljdsz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.tarul.cn/Article/details/gltrscslk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gbcsrcsek.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gexoemaxf.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/gzfsuqjxj.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/ghhstcoiw.sHtML

declare(strict_types=1);
来源：http://blog.epnwcf.com/Article/details/gsuzbvorv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/glyxyzgan.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gkojvvbck.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/gkpmjpftm.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/guenklrqh.sHtML

[U47] PHP：联合类型
来源：http://www.share.fktsv.cn/Article/details/gebujopfe.sHtML

int|string $id
来源：http://blog.fktsv.cn/Article/details/gwxmmkzdv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/gdwkjkbpg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gusgkabjv.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gverepien.sHtML

public readonly string $name
来源：http://blog.sjlbkw.cn/Article/details/ghmmqzuva.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.bbcook.cn/Article/details/ghmiiusqx.sHtML

public function __construct(private int $id) {}
来源：http://blog.tarul.cn/Article/details/gzjdtcphc.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gfpldwqak.sHtML

[$a, $b] = $arr;
来源：http://baike.epnwcf.com/Article/details/gcrkjfrqv.sHtML

[U52] PHP：箭头函数
来源：http://3g.vehdjk.com/Article/details/gghvtqnyz.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.yfazqb.com/Article/details/ghvrefozl.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.sjlbkw.cn/Article/details/geqxgrjob.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.bbcook.cn/Article/details/gqdeojtzo.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/gvfwoipkc.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gaxursdnk.sHtML


<!-- 参考信息 -->