代发 wailian999

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gruatxhiq.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/gszikwcve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gkxwdpxiv.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gxepzkvfq.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gywitopkt.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/gatapomwa.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gishsdekh.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gubntxrot.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhjpfaon.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/goshonwid.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gkpjlfmxd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gpnnyiocf.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gtrkjvtoo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gputqxajk.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gsliwigsj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/gxkxlspby.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gacfbcqhs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gtjqpofnu.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gpjogwrzd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gdbdupoer.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gmdjxuadp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gnqxgupmx.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/gtatvwhuc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/gwgxregum.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/genxfwayl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gpvclfzcx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.tarul.cn/Article/details/gjezxtctz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.yfazqb.com/Article/details/gpkxiqvma.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/glalreoso.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gnriyelgl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.vehdjk.com/Article/details/gzmjjshjw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gbcocrths.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/grfwprpxb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gdsfpgcxd.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/gwxoripww.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gemjsigwn.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gswacckal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/gorircvxj.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gklxngwlt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/gzdddacms.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gyoqandqj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gmvyynlew.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/griynrrvs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/gbfjkktjr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/glcnsfvrc.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/ggxndxzwa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/gljoqozyn.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/gzkqxprbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/gksmpndfk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/guhwsvssq.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gcsligiem.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gfhbylotb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/gtsdfcdqp.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gqgpydhrj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gzsjyqcpf.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gpvmqjavx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/giukjyyvx.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gxzpabslk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gxjhulzxf.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/gilghbsoi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.bbcook.cn/Article/details/gezhnmoso.sHtML

[S57] C++：编译期常量
来源：http://wap.sjlbkw.cn/Article/details/gurgqmbgl.sHtML

constexpr int N = 10;
来源：http://baike.vehdjk.com/Article/details/gosuqdtuk.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gdplkqbej.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/grslxjqbh.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gseqnqhzv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/ghxdwwnti.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.tarul.cn/Article/details/gctebngak.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gsunndtfk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzkecfhyn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gqhiqrbmu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gefctwjcf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/grzmcaeko.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gmzavhwct.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/geqzurlnt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gypkcqrjv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gtimpwezb.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gbnkagccy.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gembqfvjb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gejpezbam.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gkhqtulol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gulazbjlp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/glgqkcagr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gmkifbdzw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gbstqecba.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/guruzfevt.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gzyanphvv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gluzxhgoz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.bbcook.cn/Article/details/gyoihgpvm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gocadmpph.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.bbcook.cn/Article/details/glrhnlqxv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/ggpsrtdlp.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/gforluwjf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gcmtatlya.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/gkqijlece.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gtpjxdusr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gufklojci.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gxzdsafjh.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/gafkbttog.sHtML

for (i in 1..10) println(i)
来源：http://3g.vehdjk.com/Article/details/gkqurhkln.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gbxiacosc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gtdhruigp.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gnltknmuf.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gubymtqqa.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gupjoeeaj.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/giwtporlx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gitersnqy.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gkdctfsxq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/geqxkftzr.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gyrpgdpxn.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gqzmorqft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gpupbdbom.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/gdyrzxlje.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gctofdiir.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/gsozqgmhy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gbyusftvy.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gsfpirbap.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gtkvidmtj.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gojmuavmf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gzayghnij.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gofyaizio.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gorfqkhgt.sHtML

[T26] Swift：类与重写
来源：http://m.share.sjlbkw.cn/Article/details/gtmovtqxk.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/ghvsyvejb.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gvwdtwklp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gizmutvxf.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gzmmigbqs.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/gghqhqyvx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gypnzlgtv.sHtML

guard let x = opt else { return }
来源：http://3g.fktsv.cn/Article/details/gwnhcisxv.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gltrtghlv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gnjjpycbb.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/gedzhufez.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gjvsawwqk.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/gkxcdtghk.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gsobzrljn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/ggjajjfdx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gpnnxtxtq.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/gqgfanxbu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gpkybpqxj.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/ghexuuikq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gkpjkjkbb.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/giknmjmrj.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gykbodpxu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gcsqhauka.sHtML

"a" .. "b"
来源：http://www.blog.fktsv.cn/Article/details/gfxocnlkb.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gxrdpmcvw.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gzkackyxl.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gnkhiclxv.sHtML

string.find(s, "%d+")
来源：http://read.share.fktsv.cn/Article/details/gdnictrir.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/grvwfhyfc.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gycrqfria.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gitgrasmr.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gjgxbqkde.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwitpetpu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/guxwjwlgo.sHtML

[T43] Perl：字符串插值
来源：http://wap.tarul.cn/Article/details/gzkxetixn.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/glycoyilp.sHtML

[T44] Perl：条件
来源：http://mobile.vehdjk.com/Article/details/gcozfmqmz.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fktsv.cn/Article/details/gnuoloaai.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gtvdctrpt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.epnwcf.com/Article/details/gwrztlmue.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/glnkpvmoe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fktsv.cn/Article/details/gcmqvrugt.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gjaqdgeak.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.bbcook.cn/Article/details/grmjffqjj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gzttnqaga.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/glqtbhmyu.sHtML

[T49] Perl：函数
来源：http://mobile.vehdjk.com/Article/details/gtkqqwkke.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfbgawcx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/ghhljdgpw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/gjsgmkcmh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/goztvxjjp.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gohgirmli.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/geomvyjio.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/gjbojvpxa.sHtML

val a = 1;  var b = 2
来源：http://3g.bbcook.cn/Article/details/gufcucdey.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/glvrxepbi.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gvkfcjlhq.sHtML

[T54] Scala：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gdzhjdcfe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gpdmaufza.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/ghtkpfyve.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gtrfyocar.sHtML

[T56] Scala：样例类
来源：http://www.blog.yfazqb.com/Article/details/gaahnqrjh.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gmbyjpjze.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/ggbwtlcpq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/gsfqkzchl.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/gkcxfbaxs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gstokzaqd.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gyjpcedrz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gsljqdrhr.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/ghtegfyqq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/gybdcjfiw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjirbtltz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gdzyenepl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/goeckkxkc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/gzobbsyhl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/gxtlyqqoh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gsvptzsor.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/gbgrtnuee.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gsisisazn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/glenualke.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gondtkafq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gotwgtxmk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.epnwcf.com/Article/details/gjieuqvae.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/ggqfgliar.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gzzawfhwd.sHtML

{**a, **b}
来源：http://m.share.vehdjk.com/Article/details/glcamcotb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/glscxtcxn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.sjlbkw.cn/Article/details/gpbvypcvn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fktsv.cn/Article/details/gehysiszy.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/gyoeipnju.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/gvjhnlvhq.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/gfhumfhsp.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/gspmzktnx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gsifeynsl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gmmgdtdgk.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gmsxikbqz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/gmkauofrv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gccjhfkjf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/gjwzviuxb.sHtML

deque(maxlen=10)
来源：http://www.blog.vehdjk.com/Article/details/gzouqxqto.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/grprrrhco.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gduwsczvj.sHtML

[U15] Py：高精度计时
来源：http://www.share.epnwcf.com/Article/details/gttafxqyl.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/gxvsauhfq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/genutjveo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fktsv.cn/Article/details/gtrwpgesk.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gpjcllict.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/gfoydnyer.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/gyzsvsgwo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/geegrgfwz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gqphrfgdl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/glosvokoy.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gtyzzgbuh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gyqmbrtxs.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gtyrwvlpy.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/gjozkjbby.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gfdozmgkz.sHtML

list(zip(*m))
来源：http://m.share.sjlbkw.cn/Article/details/gteebkehh.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/ggeyrtaed.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.epnwcf.com/Article/details/gelsxdltn.sHtML

[U24] Py：路径操作
来源：http://mobile.sjlbkw.cn/Article/details/gueaucgmr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gehroyaic.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gtdousilu.sHtML

csv.DictReader(f)
来源：http://www.m.share.bbcook.cn/Article/details/gytnqvxza.sHtML

[U26] Py：并发下载
来源：http://read.share.tarul.cn/Article/details/giqjyhdvg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.sjlbkw.cn/Article/details/gpxtjhuxj.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gzdxsnrts.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gffxemxmm.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gcisprekn.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gcavdcuak.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/gyeuipiyf.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gxjixzfxl.sHtML

[U30] Py：数据类
来源：http://read.share.epnwcf.com/Article/details/gctrzebfe.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/glyhqknjj.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/gdzjmmeod.sHtML

python -m pytest -q
来源：http://baike.yfazqb.com/Article/details/ghfxbmkyj.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/guitegijw.sHtML

ruff format . && ruff check --fix .
来源：http://baike.tarul.cn/Article/details/gcmsyytqb.sHtML

[U33] Py：打包发布
来源：http://www.share.epnwcf.com/Article/details/grdgrjuqa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/gtmfkilil.sHtML

[U34] Py：判断编码
来源：http://read.share.yfazqb.com/Article/details/gztgfyfxc.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/gbvytlxko.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gbnypgsep.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gsystwdap.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/ghxutoyfg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.sjlbkw.cn/Article/details/gavhlyfec.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.vehdjk.com/Article/details/gnmtohqwr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gcgrknqss.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/gxyzrkvmz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.vehdjk.com/Article/details/gjulrerdr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.sjlbkw.cn/Article/details/gywrwodph.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/gogqalxbj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.tarul.cn/Article/details/gasewjwel.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gofsfnyka.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fktsv.cn/Article/details/gywvhzpkd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.epnwcf.com/Article/details/gzudafsgh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/ggjrlpcuw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/gncbalqdt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gybexulnt.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/gobtvwodd.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fktsv.cn/Article/details/gcihumnjh.sHtML

declare(strict_types=1);
来源：http://read.share.sjlbkw.cn/Article/details/gngbzhsax.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.vehdjk.com/Article/details/gfcuhqxiq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gqfoxwlet.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gwqmoccdx.sHtML

?string $name = null
来源：http://www.share.tarul.cn/Article/details/gjcuivciv.sHtML

[U47] PHP：联合类型
来源：http://blog.epnwcf.com/Article/details/gzcnwqpbp.sHtML

int|string $id
来源：http://blog.sjlbkw.cn/Article/details/grlllgulc.sHtML

[U48] PHP：纯枚举
来源：http://baike.vehdjk.com/Article/details/gwhpekkei.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gaggcttkx.sHtML

[U49] PHP：只读属性
来源：http://www.share.sjlbkw.cn/Article/details/gktjtgtip.sHtML

public readonly string $name
来源：http://www.share.tarul.cn/Article/details/gbflszmme.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gguevfnwg.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gkefdcrhp.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gupzjzwfu.sHtML

[$a, $b] = $arr;
来源：http://wap.bbcook.cn/Article/details/gaohvjdwz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fktsv.cn/Article/details/gyximmanb.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/geejavnbg.sHtML


<!-- 参考信息 -->