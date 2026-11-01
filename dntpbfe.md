代发 wailian999

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gyvnibkgs.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/ghwgzbxbt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gtpvsinoy.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gvtnouyyq.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gvpprkpvl.sHtML

#define X_H
来源：http://www.blog.yfazqb.com/Article/details/gerntxyqc.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/guhtbaijq.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gwwgloquz.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gcivbvpzm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gcaljorad.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gbnrilcdv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gphqvpamj.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gzrrdxvzz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gryydefto.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gnxmzhdrk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gmprjdsmp.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gydclgohu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfvfybhf.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gycjlftmc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gupeokqvr.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gfmliyjba.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/gsddigkkl.sHtML

[S38] C++：排序
来源：http://baike.fktsv.cn/Article/details/gtojycgwk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gyljbikos.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gtdbrhnco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/gcmlvaidc.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/ggyvqrxyy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gnyrvukrk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gfmbbnctk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gqolxkiuz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gsdzreswf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/grhtdjndy.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gkfzswlqh.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/glykibsyj.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gczttepkc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/gwfbvgplp.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gpbvlztoo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gumhdcbjs.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/gcbtnfkge.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gpbcqwfxy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gyuqmvjsn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/glmfaadsi.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gatdzdsuo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gqorjowsd.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gbvjdoghm.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/gwwyhmdvz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gqoyphwwi.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gadumnuhb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gvlqntwjp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gjmumshkt.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gyatparjz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gluedfweq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/glnfteyvg.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/gcmyqvtzx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqzlveth.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/glnevhvjj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/ghxnspppn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gipipglfy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/guawgwjjb.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/gozhyglzh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gezxnbsen.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gfsgfpkgj.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gwtowkfxw.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gmbdokerd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/glxyasylq.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/glkxihipw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gczvbanoy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gmnpjfzyo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fktsv.cn/Article/details/glesujesm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghsmqnngv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gwqpmpwad.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcvfspakb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gsloyidzp.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/geylgehim.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/ggqkniucd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/glgldxyrq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gkzxqrysm.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gmcelshsu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gvkyytlay.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gglyrzhkw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.sjlbkw.cn/Article/details/geqivcqtd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gqmhayvor.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gsxmyejrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gmfxqilou.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gdwsrzaxp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gssihpzxz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gehukqgic.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gxfqijesp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gmpkpbuxi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gpqojiflr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gmjxjqnwj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gklsbmcxs.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/gpxvvifry.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gdnxjmfuf.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gndmnqusd.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gcelqjlhe.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/glwveyjwk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gsmkvqxbc.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gnhuvcvsm.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/ggmsyhaax.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/ggsaxoedi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gxbscocrq.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/gnmoyvnff.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gbqmcetir.sHtML

[T17] Swift：变量与常量
来源：http://blog.fktsv.cn/Article/details/gfeptenze.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/gpcygfzlc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/ggevynvie.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gtqkzaaxi.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gxzltaltq.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gxevhjdmx.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/guhdozddz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/guxhsenph.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gnmweuuxn.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gawksrntc.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/grbknfxow.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gotxxoadq.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/galxebslp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/ghubhlnww.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/goxzlgpyx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gblrzfoon.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gnwlogyid.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gdqziiaqs.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gsyfnpobs.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fktsv.cn/Article/details/glcpgxwjt.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/grewxmogp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.tarul.cn/Article/details/guxbgdzod.sHtML

[T28] Swift：枚举
来源：http://3g.tarul.cn/Article/details/gtkzoqxqc.sHtML

enum Color { case red, green }
来源：http://mobile.sjlbkw.cn/Article/details/gkhfxbdib.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gcbwqicjf.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gyborumku.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/gtcrlwynm.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/gjrbiiokj.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gneiqiajj.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gipmmawed.sHtML

[T32] Lua：局部变量
来源：http://3g.bbcook.cn/Article/details/gquuhgtey.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/gfgovmzno.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gtrvtdugu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.epnwcf.com/Article/details/gpzjgcdbi.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/gbzjatvmw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/gxppmucrn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/gatdsbkvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/gbjyefqmk.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/ggfjzmhae.sHtML

function add(a, b) return a + b end
来源：http://www.share.tarul.cn/Article/details/gtlsofoks.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gmjqscoog.sHtML

"a" .. "b"
来源：http://baike.sjlbkw.cn/Article/details/glcrprnhh.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gxzzbfyio.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/gkqiwqljo.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gyidjolbo.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/gsvobzpbu.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gwmbylidi.sHtML

setmetatable({}, { __index = base })
来源：http://baike.vehdjk.com/Article/details/gadtsmfvx.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/gdedlgrvy.sHtML

print "Hello\n";
来源：http://www.share.vehdjk.com/Article/details/gwspdhvpw.sHtML

[T42] Perl：变量类型
来源：http://m.share.bbcook.cn/Article/details/gfuftfhon.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gomoatyel.sHtML

[T43] Perl：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gqzrpokdp.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gowruwmtq.sHtML

[T44] Perl：条件
来源：http://read.share.fktsv.cn/Article/details/gdzjipshi.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gjbkiyymp.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gxlceaiir.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/gretvkvxp.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gpujrvqow.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gznzuruzu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/gqwxtuage.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fktsv.cn/Article/details/gilfoyyda.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gdnlrrzzu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gzsmfazwm.sHtML

[T49] Perl：函数
来源：http://www.blog.vehdjk.com/Article/details/gmbrguqcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gfxvfjjll.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/glggwjmjl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.epnwcf.com/Article/details/gzniekcpw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gwygnszbm.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gnvkswxdw.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gtgddlaud.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/gieulhdij.sHtML

val a = 1;  var b = 2
来源：http://3g.bbcook.cn/Article/details/gdkxmourd.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gzkfvmnqh.sHtML

s"值: $b"
来源：http://www.share.vehdjk.com/Article/details/glgapxvpf.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gsxyrttev.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gvipnlxdz.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gcyqsuwgt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.bbcook.cn/Article/details/gppsxudsc.sHtML

[T56] Scala：样例类
来源：http://www.blog.vehdjk.com/Article/details/gaqgempoa.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gksycdfxz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gvvhbvhan.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gnqaxokmm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.yfazqb.com/Article/details/gvmkzuvhh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/ggxvioymk.sHtML

[T59] Scala：循环
来源：http://www.share.yfazqb.com/Article/details/gtphxthkz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gljzobggb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gsueilyjt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.epnwcf.com/Article/details/gkcyyvfcj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwjigqbaw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/grycmgrbg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gciucyftu.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/gjvasymau.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gfphghoff.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.sjlbkw.cn/Article/details/gezuarbzk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.vehdjk.com/Article/details/gfzcthxfd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gmmuucsqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/gczmiabvi.sHtML

[U04] Py：变量调试打印
来源：http://baike.vehdjk.com/Article/details/gtdkxenzc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/gwblipqqa.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fktsv.cn/Article/details/gjtjjqhzu.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/ghecnhlbr.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gmdferrvg.sHtML

{**a, **b}
来源：http://3g.bbcook.cn/Article/details/glfqjcoeh.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gxhnliqkk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gjzenowvz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gikbamrid.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.vehdjk.com/Article/details/gliaeqlqf.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/gcnlduoek.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/gfpnuesho.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gtnkvfwak.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/glluzpawx.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/gpffxhqch.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gidtpwytb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.tarul.cn/Article/details/gjlexmuwq.sHtML

Counter(arr).most_common(3)
来源：http://wap.sjlbkw.cn/Article/details/gfljftnqr.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.epnwcf.com/Article/details/gmarzwhuy.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gamptulde.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/guhoorhdm.sHtML

defaultdict(list)
来源：http://wap.yfazqb.com/Article/details/grduvqcmv.sHtML

[U15] Py：高精度计时
来源：http://m.share.fktsv.cn/Article/details/gthrqloey.sHtML

t = time.perf_counter()
来源：http://www.blog.epnwcf.com/Article/details/gevzwxztc.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/gpwaxnzgz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gvtglctbg.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/gondupcmu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/ghypegmmd.sHtML

[U18] Py：预编译正则
来源：http://m.share.bbcook.cn/Article/details/gavsqepip.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/gjawywmjz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/gfuvdqcix.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/gjabocbdd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.sjlbkw.cn/Article/details/gbvifhvbh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/gimezpwdc.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gybelinrt.sHtML

@contextlib.contextmanager
来源：http://mobile.epnwcf.com/Article/details/gsjwijudv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/gzhwjuxtx.sHtML

list(zip(*m))
来源：http://m.share.vehdjk.com/Article/details/gplnbvqrq.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/grvjmkrpl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gsgkuebmj.sHtML

[U24] Py：路径操作
来源：http://blog.yfazqb.com/Article/details/glikvfmwz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gvrcrwvdh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fktsv.cn/Article/details/gimecjqdn.sHtML

csv.DictReader(f)
来源：http://www.share.epnwcf.com/Article/details/gdvdesqyo.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gwpjfrmgb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.epnwcf.com/Article/details/gbjkbrwsu.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/gtuooygxs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fktsv.cn/Article/details/gynlzzqgl.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/gxkfwpixo.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/grqamcivd.sHtML

[U29] Py：属性校验
来源：http://baike.yfazqb.com/Article/details/gosyvzpkq.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gouepyumh.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/gshwwcpvp.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/grdqmibpu.sHtML

[U31] Py：单测
来源：http://blog.vehdjk.com/Article/details/galygipth.sHtML

python -m pytest -q
来源：http://baike.sjlbkw.cn/Article/details/giopqycas.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gmgohyqpd.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gfpwkdzxh.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/gegxnddra.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gdwciycng.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gyfupiujc.sHtML

chardet.detect(raw)
来源：http://3g.bbcook.cn/Article/details/gwpefdesx.sHtML

[U35] Py：发送邮件
来源：http://blog.yfazqb.com/Article/details/gtzftjocp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fktsv.cn/Article/details/gxmhksbrv.sHtML

[U36] Py：定时任务
来源：http://blog.epnwcf.com/Article/details/gicpocybb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.vehdjk.com/Article/details/gfxgrrssm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.bbcook.cn/Article/details/gejejzmsx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.epnwcf.com/Article/details/gznosmynk.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fktsv.cn/Article/details/goxzjeqrc.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.vehdjk.com/Article/details/gmnkgasqc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.vehdjk.com/Article/details/gdollsjas.sHtML

sys.stdout.isatty()
来源：http://blog.yfazqb.com/Article/details/gsnsaxmpj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/giggcqgus.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gsrthhmzu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxqjlkfa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/ghjocejxl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/goojryixh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gsqcgjldc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.tarul.cn/Article/details/govybafwi.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gdqcrtrge.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gywkqyvqb.sHtML

declare(strict_types=1);
来源：http://read.share.bbcook.cn/Article/details/glloldsna.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.bbcook.cn/Article/details/gyjvkejek.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gmaqdigqr.sHtML

[U46] PHP：可空类型
来源：http://wap.bbcook.cn/Article/details/gvoyqtczq.sHtML

?string $name = null
来源：http://www.share.yfazqb.com/Article/details/gwlfkvzhx.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/gugicmqas.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gzbfpfwdr.sHtML

[U48] PHP：纯枚举
来源：http://wap.epnwcf.com/Article/details/gbljpivzs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/galpdpojn.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/gcomcxeot.sHtML

public readonly string $name
来源：http://www.blog.fktsv.cn/Article/details/gcuvirzci.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.tarul.cn/Article/details/gfhkxhulq.sHtML

public function __construct(private int $id) {}
来源：http://wap.bbcook.cn/Article/details/gtafmzqql.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/guwvxucby.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gvqcwvphz.sHtML

[U52] PHP：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gcxnmuzhw.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gcykodufj.sHtML


<!-- 参考信息 -->