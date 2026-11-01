代发 wailian999

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gaoufughr.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gvsebntup.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gbqyjzzaf.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/ghkwzmkrw.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gnovxyprp.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gkpctjoyk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gbbwedpbt.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gaonvoshk.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gbcbkrzxi.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gcbnhbkaz.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gqyytkcuv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gisflemhi.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gyyykcscc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gnvktolnd.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gnmilzqnj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gjxadqlhv.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gwknqfljb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/gfqixjazw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gvaltyhsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gkhvqkxql.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gjjwwadtb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/grkclblcc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gdjucesih.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gydlgmqby.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/ghuljwkdy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gryggaqek.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gktiocytw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gxqtqqqdf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/ghlnbkurx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gvlnkglcc.sHtML

[S40] C++：查找元素
来源：http://mobile.bbcook.cn/Article/details/gozacljag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/gjbqhhwok.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/grcasgqgz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gwvldalyu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gygzaupvb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/gmrhddiip.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gaaekwolh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gnamxcbwk.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gtmcznnbc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gwgoocjzb.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gtqifytwx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/giujxcyfb.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gbbcglfzm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gsfjeuzow.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.sjlbkw.cn/Article/details/gtptuhuyt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gpdgajqrw.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gdrskttbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gtpywvvru.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/grpimbuiz.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gcfulkgyt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gdwkrjzuq.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gfppjqnrj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gnmgkrmul.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gyaspegym.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gsmcuuxnu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/gjfuxlocy.sHtML

int size() const noexcept { return n_; }
来源：http://3g.epnwcf.com/Article/details/gdhsxfbgn.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gxvfxgnky.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/ghwhzykas.sHtML

[S54] C++：异常处理
来源：http://baike.sjlbkw.cn/Article/details/gmopkhzdy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gozuovbzj.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/grdfwpynz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/getjazuau.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gxghrxczj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/ggtibonfl.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/geljcyvzd.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gvhibthhc.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gwznsyxuo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gkciozrks.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gohkshshx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gpexnfbmf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/ggdztclai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gkzfhykii.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gujtxaefl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/ghuptazds.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvqdxayxm.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gjukddfkm.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gfwmsyxcr.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/gudcessnk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gpgbqiujm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gapqoiuji.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/ggmuyqzbi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gomhrovuu.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/galeiyqpz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/guensqcfe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/gicwfdfhk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/goavbcfmy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gvwqwnaxn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/guteolzet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gwhqjrzlb.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gmuuylqyz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.bbcook.cn/Article/details/gjbuibqor.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gjmofvqwj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gtoyafvup.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gfetuurwt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gfxyndakz.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gtsstmbtc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gihmtgtmd.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/glrppkyiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gaxjfcumx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gjbukdomh.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/gvnuuvanl.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gxzqykqcj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gwnynjneq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fktsv.cn/Article/details/geuwcnprv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.bbcook.cn/Article/details/gcattetlp.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gprayjnpg.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gjvtdsrrj.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gawzvxnxv.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/gwgentrsv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/givghiqtm.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gryvxzulx.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gjzgxclqb.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gkvvultvb.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gjjmdwezr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/ghhluymck.sHtML

[T21] Swift：遍历
来源：http://www.share.sjlbkw.cn/Article/details/gdfkoyycs.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/ganxhyilb.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gmqkekazo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gikgrulzn.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gonymiipj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gimzdwlnl.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gjdselcwk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gxbouucye.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gsogfjsju.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gmymzyouf.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gtqvxnbzh.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/ggbqpuvgh.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/giwrvhady.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gimdmuota.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/guuzazkbn.sHtML

enum Color { case red, green }
来源：http://baike.sjlbkw.cn/Article/details/ghpkceejs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/gsrqgspcl.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/goiztgrok.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/gnacsbysa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/giasleuyd.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/ggzzklgal.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gnbzmnayo.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gaglvnech.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gdhppvkzf.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/gptspzgst.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.sjlbkw.cn/Article/details/gklolcdmm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gfjsuhwbc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gvbbxytmr.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/gwjfaighp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.bbcook.cn/Article/details/gossrrzds.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gffaydxeb.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gsbfdlooq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gddzwidwv.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/gistksicd.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gtjchqtjo.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gcchdgdjc.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gtjsjdmyz.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gdfexxakw.sHtML

[T40] Lua：元表
来源：http://wap.tarul.cn/Article/details/gtgpdsfth.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gdmvwvpck.sHtML

[T41] Perl：Hello World
来源：http://www.share.fktsv.cn/Article/details/gqipfbwmt.sHtML

print "Hello\n";
来源：http://read.share.epnwcf.com/Article/details/gxsxvltye.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gzddhxufz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gcgsotzdn.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/guvvpiocv.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/ggphutyft.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gbfntayih.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fktsv.cn/Article/details/grdvabnko.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/ghqvyrmiw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gizhsoqvn.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gwkgudsmt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/gvtdbtzen.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/gemsjlmgw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gsxcwdsji.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gkzoiejjq.sHtML

$s =~ s/old/new/g;
来源：http://www.share.epnwcf.com/Article/details/gwxhhfiyt.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/ggmvwqrvm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gnopyhnyn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gkolztsqk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/ggvfdwttz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gxrpoynmx.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gqrygwgak.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gouzalvma.sHtML

[T52] Scala：变量
来源：http://blog.tarul.cn/Article/details/gtpsorcjd.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gyqpigwju.sHtML

[T53] Scala：字符串插值
来源：http://www.share.bbcook.cn/Article/details/goexwcofb.sHtML

s"值: $b"
来源：http://m.share.bbcook.cn/Article/details/giulymoyr.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gcihehbsv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.sjlbkw.cn/Article/details/ghznsmcpo.sHtML

[T55] Scala：集合过滤
来源：http://3g.fktsv.cn/Article/details/geiqfanjz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gixyzwnrb.sHtML

[T56] Scala：样例类
来源：http://m.share.fktsv.cn/Article/details/gsnymzsoi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gabgecngr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gnkvmzbms.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gnutlxjey.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/genyiixpv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.bbcook.cn/Article/details/glxyqnazd.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gtsjiclnf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/ghhmfalba.sHtML

[T60] Scala：折叠
来源：http://read.share.bbcook.cn/Article/details/gatraqdci.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/galqcunqe.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggcslflfd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gveyedbur.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjplmbbvf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/gauegkevu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/glbrqeoff.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.vehdjk.com/Article/details/gqitwxoyz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/gkdrixghs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gvyfksaua.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.vehdjk.com/Article/details/gwxenimzt.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/gwmxdmitj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.vehdjk.com/Article/details/gxdsdvczn.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/govvxovtj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gciohreth.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gdhwqsrdp.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/gqfdcchyu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/gfwngkkjz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/gthsnwdhc.sHtML

[U08] Py：展平二维列表
来源：http://blog.vehdjk.com/Article/details/gbttgtqet.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/gzphlnxzl.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/gqkbqbskm.sHtML

max(d, key=d.get)
来源：http://read.share.epnwcf.com/Article/details/gdniwpcpi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.vehdjk.com/Article/details/gezbwqfje.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.epnwcf.com/Article/details/gewuhtnwj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gxslssqhm.sHtML

(x * 2 for x in arr)
来源：http://wap.bbcook.cn/Article/details/gywiesgez.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/gcmceammv.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/geqcsmyzo.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/gvqohvciv.sHtML

deque(maxlen=10)
来源：http://www.blog.tarul.cn/Article/details/geovcwdrz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.bbcook.cn/Article/details/gztmtnwmd.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/glzpiekcu.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gbgykrwlr.sHtML

t = time.perf_counter()
来源：http://3g.vehdjk.com/Article/details/gifkjevng.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/ghcfdrirb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gafvqpejo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkbyyemk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gcqxpufqc.sHtML

[U18] Py：预编译正则
来源：http://www.share.vehdjk.com/Article/details/gomaoplje.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/ghogjrrbc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/gcqivvvdx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.tarul.cn/Article/details/gngbmsmed.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.tarul.cn/Article/details/gxdopabuz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.vehdjk.com/Article/details/gtfpylvev.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.tarul.cn/Article/details/gadsihedv.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gigkzdari.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gzjiyczyx.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gqumvocdk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.epnwcf.com/Article/details/gwuzoghmo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/gfqguvcyb.sHtML

[U24] Py：路径操作
来源：http://m.share.vehdjk.com/Article/details/guwmcewya.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/grjubzwyt.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/giiepzyma.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/gqvkeneoy.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gltkuxkwg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/gvwtzdxzi.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gcjvvtiah.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.sjlbkw.cn/Article/details/gbzktjccs.sHtML

[U28] Py：类型别名
来源：http://wap.sjlbkw.cn/Article/details/gydnslbqy.sHtML

UserId = int
来源：http://blog.tarul.cn/Article/details/gkvkpkoqr.sHtML

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/gteczutpa.sHtML

@property 与 @x.setter 配合
来源：http://mobile.yfazqb.com/Article/details/gvkddwbqf.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gtbryankn.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gcavfqlja.sHtML

[U31] Py：单测
来源：http://m.share.yfazqb.com/Article/details/gsdafyihq.sHtML

python -m pytest -q
来源：http://blog.tarul.cn/Article/details/gspavgtcg.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/gprbwzizq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gfnnwlnhc.sHtML

[U33] Py：打包发布
来源：http://blog.fktsv.cn/Article/details/gmmompivs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gribbalbn.sHtML

[U34] Py：判断编码
来源：http://www.share.epnwcf.com/Article/details/gxqtbocrh.sHtML

chardet.detect(raw)
来源：http://www.blog.vehdjk.com/Article/details/gpugctgsw.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gjjxmfmbt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.sjlbkw.cn/Article/details/gkezfjjhh.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gbokcrzmk.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gmgnaqnsu.sHtML

[U37] Py：读写 Excel
来源：http://3g.bbcook.cn/Article/details/gehzqwwdq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/gfnopbwwg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/gxducpfsm.sHtML

Path(__file__).resolve().parent
来源：http://baike.sjlbkw.cn/Article/details/gqxlzmuik.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.vehdjk.com/Article/details/guohttvte.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gwriotxzh.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/gkwdfaenp.sHtML

print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gtyirsdup.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gcwlbqgnb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/ghkvfwlyp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/gyrxlgghl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.sjlbkw.cn/Article/details/gedaljsmu.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fktsv.cn/Article/details/gksdgvnps.sHtML

namespace App\Http;
来源：http://www.m.share.yfazqb.com/Article/details/gnnyvrizu.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fktsv.cn/Article/details/gintffmox.sHtML

declare(strict_types=1);
来源：http://mobile.fktsv.cn/Article/details/gypclrvnh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.bbcook.cn/Article/details/gavctnfuf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gkbxyaxux.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/goragxqsw.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gmyuvlvdl.sHtML

[U47] PHP：联合类型
来源：http://wap.fktsv.cn/Article/details/gzqppsyub.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/gmftlkuvx.sHtML

[U48] PHP：纯枚举
来源：http://3g.vehdjk.com/Article/details/gbfzayijr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gawemyqnp.sHtML

[U49] PHP：只读属性
来源：http://mobile.sjlbkw.cn/Article/details/gslthihfz.sHtML

public readonly string $name
来源：http://baike.fktsv.cn/Article/details/gttwjefvl.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.bbcook.cn/Article/details/gabibfkfb.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/gucluqadz.sHtML


<!-- 参考信息 -->