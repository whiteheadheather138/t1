代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gfbbifeju.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gevuqceeb.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gnmekabfn.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/ggkgqilju.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gjagrtvey.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gygapxrec.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gnzccxsmj.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gruoiflkp.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gomrxbhpv.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gsncjpdbn.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/guflhbqfb.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gvgexihwo.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gluiykpfj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/gjgpaqbvk.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/guodvzovz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gmiegwruv.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gaiggddyj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/guhvjfkcb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gbkuyrhnc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/guxqjtuge.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/gnfytxrep.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gbjzcmmmo.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/ghinutwhq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gqqqzkbtx.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/glnmywrys.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gpeymzcdd.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gkihmdnvg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/glsitptpd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gatfzrzhc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gwfmbrlxt.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/gidddtsni.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gwwmwcrgo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/gtydrazhh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gtiufnkqi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gtsxurhpr.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/giheruqke.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gnecyiimu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/gahfnrfjb.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gmagexyww.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/godxgpdua.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/gqmxhkplc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsacbedd.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gmtksgspz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gmtxqjieq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.yfazqb.com/Article/details/gngquxgqo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fktsv.cn/Article/details/gpsajhpez.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/glrmjnqfd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gosrjjgmo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gwlbphhmk.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/goaddnnwz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/geoumlkgx.sHtML

[S50] C++：格式化数字
来源：http://baike.fktsv.cn/Article/details/gocceednn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gkydemdbd.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gukwjmtpq.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/gvwvsjzyz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/gvrboupcr.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/guynstprb.sHtML

[S53] C++：移动语义
来源：http://www.blog.tarul.cn/Article/details/gtieajxkp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gtfiovyql.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gxxoakjyg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/geubcytfm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gbvnomgzk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gkqbxuiyv.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/guhhehhkz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/ghywmtoeq.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gpsouilmw.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gumklvbkd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gqudrxsxg.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gyqjmzhlj.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gohongrnj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gbqfmpiny.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/grauahkgk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gjffdtrxp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gawuiwywm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gotsczrbn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkomuaknn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.bbcook.cn/Article/details/gsuqtuxje.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gtlrtffdk.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gmtyyufqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gzwgqrlit.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gccxpbcmj.sHtML

"值: $b"
来源：http://baike.yfazqb.com/Article/details/gcdvtzdva.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/grzkamqbw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gvebutxub.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fktsv.cn/Article/details/gkztsiuwb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gnzufsdvr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/gwvcfpqhz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gwdnybcgu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gkeawfsgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/gqrvwouah.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gojblhwus.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gpojxyhjl.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gwjpjyhgf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.yfazqb.com/Article/details/glzaekieb.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/ggebvkjwq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.bbcook.cn/Article/details/ggrqvttey.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/gmgiczavs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/grfjwoftk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gekglilan.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/glymswqkh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gqwdkqonf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gjwztdfgf.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/ghwuekxoj.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/gnzgpsnyl.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gmeitdfnf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gmuxottai.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gzkjokuog.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gnclhxiti.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/gisbezhxn.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gfarsdvit.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/gsqnvlhnj.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gsbgjjpaq.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/glvhrtoqp.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gcmanajif.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gveqryuue.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gfhrlbjcq.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gubiisuod.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/gaieftwog.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gkkeniamy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/gcjwdcsye.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gmektwfdo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/gipyoupux.sHtML

[T24] Swift：闭包
来源：http://mobile.sjlbkw.cn/Article/details/gkqwrsiyd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gjupywnhh.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/gsfoghmhd.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/gzncnsjpt.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/gsjvqbaqh.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gowsbtxcd.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gcsivlzft.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/ghzdjvlxg.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gnyrrgddv.sHtML

enum Color { case red, green }
来源：http://www.share.fktsv.cn/Article/details/gdfpfghqh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/giisuwmho.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/gbbinahtw.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/godngldxg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gcujrgihm.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gmbovkjnz.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/ggilxuvbb.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gembqtaqu.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gwykxzgrz.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/gmgynlwdg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/gsdszlcqt.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gglyrdrap.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gcitolkkx.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/giecqlxkj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/gbggdwjvw.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/geeodkpqg.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/ggcckkkey.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/glawywhqd.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gqbliollh.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/guziuzqvl.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gpbvzrtrf.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gxnwesotu.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/guqsrezml.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gwxskmybi.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gvvuldimo.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gmmesqbpc.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gczpyzpwf.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/geuaiucwm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/gfwsvgtai.sHtML

[T43] Perl：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gwauahcuz.sHtML

"值: $a"
来源：http://m.share.yfazqb.com/Article/details/gmentjoew.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gioatwxxc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gralpkspd.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gfrtlqqqw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fktsv.cn/Article/details/ggnlsajte.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/giwxrlpas.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.bbcook.cn/Article/details/gyijijlct.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/glszzworu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.bbcook.cn/Article/details/ggmpbcjpl.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/gvbodxmzs.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gbnclfvjg.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/grvtaajvt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gcwhonect.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gussnzrtq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/gydagcjtc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.tarul.cn/Article/details/gpdnejawi.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gpxrrpttz.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gbofvfssi.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/gbgnxwmgp.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/gzkmbekwv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/ggbdiylqh.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gqywylarf.sHtML

[T54] Scala：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gaknofvyi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/geyofhqvg.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gyunciegn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.vehdjk.com/Article/details/gufujpekw.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/gniurgzvs.sHtML

case class User(name: String, age: Int)
来源：http://wap.epnwcf.com/Article/details/gxncqfqsc.sHtML

[T57] Scala：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gqepmmppb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gcngvhosi.sHtML

[T58] Scala：函数定义
来源：http://read.share.tarul.cn/Article/details/gjeytspki.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/ggtpqmcht.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gvtlsnnqx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gxefujnra.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gouyavalo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fktsv.cn/Article/details/gmrtacbci.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzludgtlt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gzkzmjhzp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbdutjkab.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.bbcook.cn/Article/details/gbsfngdvj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/gxvuqurpx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.sjlbkw.cn/Article/details/gdtuhmlna.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gcsmimrms.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gzyehmljq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.epnwcf.com/Article/details/gzbcbdyqs.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gpkcjzjgl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.vehdjk.com/Article/details/gjiiogmoz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.vehdjk.com/Article/details/gyxlzoqjl.sHtML

list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gvlsbfznj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.vehdjk.com/Article/details/gasepemwm.sHtML

{**a, **b}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkepgkqr.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gxhyiihmv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/gjhxlvbym.sHtML

[U08] Py：展平二维列表
来源：http://read.share.bbcook.cn/Article/details/gumcmhpqc.sHtML

[y for x in nested for y in x]
来源：http://blog.sjlbkw.cn/Article/details/gdjsuupom.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gfkpmbuwr.sHtML

max(d, key=d.get)
来源：http://www.blog.epnwcf.com/Article/details/govijhkti.sHtML

[U10] Py：按值排序字典
来源：http://3g.fktsv.cn/Article/details/gzbadbbtm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gnjyxxvhp.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/grpjxdwog.sHtML

(x * 2 for x in arr)
来源：http://wap.epnwcf.com/Article/details/gpbwxqwgb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gexyacczx.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/gbiyanygk.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gcfvajrck.sHtML

deque(maxlen=10)
来源：http://www.blog.vehdjk.com/Article/details/gvbbvnjkm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.sjlbkw.cn/Article/details/gbjpbavvj.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/guqpheexq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwzdfhdz.sHtML

t = time.perf_counter()
来源：http://read.share.bbcook.cn/Article/details/geyjedgbj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.yfazqb.com/Article/details/ggolbugka.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gxziphzcp.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/gqhwikntf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/grotcyeky.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gaztxtlkw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gelogmmds.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.yfazqb.com/Article/details/gzceksghy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.tarul.cn/Article/details/gzlsruwgy.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.tarul.cn/Article/details/gwnktdfxy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/gtrmzrguh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/gseblcyhd.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gnyyitrxy.sHtML

[U22] Py：矩阵转置
来源：http://blog.epnwcf.com/Article/details/gahfgbwzb.sHtML

list(zip(*m))
来源：http://mobile.yfazqb.com/Article/details/gcbnzwbat.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/glufcnxmi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gimghlxtz.sHtML

[U24] Py：路径操作
来源：http://baike.epnwcf.com/Article/details/glbvpbuwa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gsqvkuygl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gncpbxsvu.sHtML

csv.DictReader(f)
来源：http://www.blog.sjlbkw.cn/Article/details/gxnthugua.sHtML

[U26] Py：并发下载
来源：http://read.share.tarul.cn/Article/details/gadpohzdg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/gxiqdytqp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gmfyqyqpv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gfiatkmwl.sHtML

[U28] Py：类型别名
来源：http://mobile.sjlbkw.cn/Article/details/gtzmutsyw.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gxpqdbduz.sHtML

[U29] Py：属性校验
来源：http://mobile.epnwcf.com/Article/details/gwuaxwptv.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/ghlqopivf.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/ghquilubb.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gnjhpmvdj.sHtML

[U31] Py：单测
来源：http://baike.tarul.cn/Article/details/gxlzncdtb.sHtML

python -m pytest -q
来源：http://m.share.sjlbkw.cn/Article/details/gdzaujuiv.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gthyjwcsn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.epnwcf.com/Article/details/gsxqopxsg.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/gjbqlvtaz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gwmzoiien.sHtML

[U34] Py：判断编码
来源：http://www.share.epnwcf.com/Article/details/gazouqcgx.sHtML

chardet.detect(raw)
来源：http://www.share.epnwcf.com/Article/details/gzkmfbpnd.sHtML

[U35] Py：发送邮件
来源：http://read.share.vehdjk.com/Article/details/gsgbwaqfk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.sjlbkw.cn/Article/details/greyalvqk.sHtML

[U36] Py：定时任务
来源：http://3g.tarul.cn/Article/details/grwynneoe.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/giepfuspj.sHtML

[U37] Py：读写 Excel
来源：http://blog.vehdjk.com/Article/details/gtnrmnlzu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gatpsdyex.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.sjlbkw.cn/Article/details/gihlxfzds.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gfgudcsib.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gsuncsnwq.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/gjyupyeya.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.sjlbkw.cn/Article/details/ghifbijoe.sHtML

print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gmbwrwmhh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/glkvwndvg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.tarul.cn/Article/details/ggngefyxf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fktsv.cn/Article/details/gknlikrdp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.epnwcf.com/Article/details/gtsyzouym.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gsvmwvaqc.sHtML

namespace App\Http;
来源：http://baike.vehdjk.com/Article/details/ggnrfdniu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gvnonedfc.sHtML

declare(strict_types=1);
来源：http://blog.sjlbkw.cn/Article/details/gaobievve.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.epnwcf.com/Article/details/gofzmgpos.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gcjeeqkpy.sHtML

[U46] PHP：可空类型
来源：http://m.share.bbcook.cn/Article/details/grdubcylf.sHtML

?string $name = null
来源：http://read.share.yfazqb.com/Article/details/ghmhxphyw.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/gzsngoplv.sHtML

int|string $id
来源：http://wap.bbcook.cn/Article/details/gnbmyrvux.sHtML

[U48] PHP：纯枚举
来源：http://baike.fktsv.cn/Article/details/gemgjbyzn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.sjlbkw.cn/Article/details/gfrfcdfxq.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/gjmympesw.sHtML

public readonly string $name
来源：http://read.share.sjlbkw.cn/Article/details/gyrzqchfv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.sjlbkw.cn/Article/details/guekjnjks.sHtML

public function __construct(private int $id) {}
来源：http://mobile.tarul.cn/Article/details/gmtznznxk.sHtML


<!-- 参考信息 -->