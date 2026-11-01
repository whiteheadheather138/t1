代发 wailian999

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/guayqkjfw.sHtML

[S27] C：定义常量
来源：http://m.share.sjlbkw.cn/Article/details/ggsfpueou.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gddnrqsnc.sHtML

[S28] C：静态变量
来源：http://baike.yfazqb.com/Article/details/gwionflid.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/grgpktxfr.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/gwifopzbx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.tarul.cn/Article/details/gtogtjbsz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gfstgxdkv.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gbgyrqkjs.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gykuekyro.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/ggiutbdml.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gekznbxtm.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/gowcpdjpt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gqrnigwhi.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gabkehmqp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gxhtywdki.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gllqzmoch.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gwytpjnmw.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gctjfitur.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gznjmdpyc.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/gzjxxkzzd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gaxfvaicw.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gvlxadfts.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gmvxaonyh.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gzexjdxre.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/ggiflmupx.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gzocejpes.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gbtfghqxc.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gataofvrv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gegiawuda.sHtML

[S40] C++：查找元素
来源：http://www.m.share.vehdjk.com/Article/details/gzvqhxcoc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/gfweznktb.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/glbtavobr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gnznvtlcd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/giuejtisn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gzvbrnoio.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gyijmwcye.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gghvoxbgl.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/gcgvwjmth.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/glovpvkmu.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gplbrlypc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.sjlbkw.cn/Article/details/gerddlubh.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/ghuebvlwd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gyzvzbzla.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/guenbvqfp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gswyvbkgu.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/glaaofvgw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gtmhjomen.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gkvtywjaq.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gcskqntsv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/ggxlggzqr.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gcepsubag.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/gcrkrwqhe.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gkuanbcdm.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/ghlgzyssr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/goxyrdkyc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gagvokgny.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/gctrtwzja.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gjejqgssm.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/gnjuoazia.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/goqunhdjn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gyvisbkwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/grhhmrble.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gxujnapzi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gddvwudng.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gjkhybezi.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gusqsibcg.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/gnxeikfch.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gyygniema.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gulkfccqr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.epnwcf.com/Article/details/gqbsojdgr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/gisddqxgw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gxudsvyxw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvstinchi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gqasbbthq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gefcqlsii.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gicbczkko.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/guatmgzbt.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gzdxstgna.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbsgvbso.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gikhcnjeb.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/grjxatqbl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/gnkhtxvzr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gyuyjexhi.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gokdcmeal.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gkbunxlsi.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gqyhmjhbw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gnaybptsc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/girdwvtqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gsaaoayrs.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gkhjwbesp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/gzirymdrb.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fktsv.cn/Article/details/gwscatufk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/gcojhwnpi.sHtML

[T10] Kotlin：默认参数
来源：http://3g.yfazqb.com/Article/details/gegdkkmpc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gemvltful.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gzzcnqyux.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gntephpfa.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gtwaikxwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gfyidfrec.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gsvgewnzh.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/gotapcjya.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gwaxdiiup.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/gveyirlsl.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gjijpaegn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gesmzkwfx.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gftnyjiae.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/ggynmnmvk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/gontaqidx.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gjtkncanf.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gnaartukh.sHtML

"值: \(b)"
来源：http://www.m.share.bbcook.cn/Article/details/gkuujzshl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gvulgezgg.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/goyuuuzcy.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/glkwrrgdm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gnwspgqbu.sHtML

[T21] Swift：遍历
来源：http://baike.epnwcf.com/Article/details/gltndiiod.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gptcbveea.sHtML

[T22] Swift：字典
来源：http://blog.bbcook.cn/Article/details/gnfpvcilz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/ghyonhwkx.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gmzmhrflf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gsdahomwt.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/gtnpwjerw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gkqjedeie.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/gqumatueg.sHtML

struct P { var x: Int }
来源：http://baike.yfazqb.com/Article/details/gvbtqgrji.sHtML

[T26] Swift：类与重写
来源：http://wap.yfazqb.com/Article/details/gcndgnutq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gtdiefjko.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/grkharhqr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/geazphiqr.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gsxminroz.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gcobofbiz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gzzyrlidj.sHtML

guard let x = opt else { return }
来源：http://mobile.epnwcf.com/Article/details/glfbxpakm.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gpwutdytc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/ggnmscghz.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gxwbrkkkf.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gqrhvmgnm.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gkmdssavh.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/gdkkmyyml.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gilatxoco.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/guntcqfiq.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gpvsipsij.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fktsv.cn/Article/details/gdekjdagp.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gdqmqsqtp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/ghfxzxeox.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gbktupeom.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gfbyrmbmz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gkcnwpbxp.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/gksnetvwb.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/ggcykzaqo.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/galbtqfyn.sHtML

[T39] Lua：模式匹配
来源：http://baike.vehdjk.com/Article/details/ghxdvtoto.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gxurysmnd.sHtML

[T40] Lua：元表
来源：http://www.share.epnwcf.com/Article/details/gfukxwcmw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.tarul.cn/Article/details/gbefidhkh.sHtML

[T41] Perl：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gstemtqjo.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gqjoancea.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/goweumqho.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/gtudgozqo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gqhkmntqw.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/gyittlkoj.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/gdzvperom.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gnrzijwtm.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/goaxzolyz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/ghkvddncc.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.sjlbkw.cn/Article/details/gmlzbogml.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gnpfrystj.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gtesnubqe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gymdbsqcr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.vehdjk.com/Article/details/gnabizzxy.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/gmkjbcabn.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gsyfgikfy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gyndgmuyh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/glugtswgw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/grtnufycn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gbydolxjr.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gnvzzdiix.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/grsocskqe.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gbojitnph.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gebqplmsp.sHtML

[T53] Scala：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gqlmcmxgk.sHtML

s"值: $b"
来源：http://mobile.fktsv.cn/Article/details/glxnrnyxo.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gtlvpmzlm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gdtnmafpn.sHtML

[T55] Scala：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gxxpaaare.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.vehdjk.com/Article/details/gsbrncrum.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/gidxvccnb.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gftxslsra.sHtML

[T57] Scala：模式匹配
来源：http://read.share.tarul.cn/Article/details/groipqaur.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/gskkhzycg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gpkeducjq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gklqxmndc.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/grpzfsiwv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gvmokuzwd.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gaxjmoxha.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gvwfqcipy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/graygaffw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/ggggfdnri.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gomczmmfw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/ghpvaaovt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.sjlbkw.cn/Article/details/gynxbgkle.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gswgowwyr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/glhtdncak.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/gdvemisrv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gidnhtdaz.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.yfazqb.com/Article/details/gglfvibon.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.vehdjk.com/Article/details/gvkmbgsgv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gcjtaiuyn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gwtrwxntb.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/gmxjdscqy.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gllzokjmq.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/giweqzepj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gnujmqfkh.sHtML

[U08] Py：展平二维列表
来源：http://blog.tarul.cn/Article/details/gzdgextxs.sHtML

[y for x in nested for y in x]
来源：http://read.share.sjlbkw.cn/Article/details/gxcdmljff.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.bbcook.cn/Article/details/gbcczaofo.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/gjbqfoaka.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/gzvdrpksr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gnlagryka.sHtML

[U11] Py：生成器表达式
来源：http://3g.epnwcf.com/Article/details/gbxqkcjjp.sHtML

(x * 2 for x in arr)
来源：http://www.share.bbcook.cn/Article/details/gsibbfbru.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gflsmerou.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/gexlnjvjz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gyhxbewtk.sHtML

deque(maxlen=10)
来源：http://mobile.epnwcf.com/Article/details/gftjnwjgv.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/gcmauyosd.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/gsaxtejpo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/gceqyzqvl.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gbhypuhal.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/gfndoyelm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.sjlbkw.cn/Article/details/gzzducnma.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gupkfsuex.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/grklkwkhb.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/getrdnyux.sHtML

pat = re.compile(r"\d+")
来源：http://3g.vehdjk.com/Article/details/gpnhxlzra.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gvcotmsse.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/gycpixvpo.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gdqpmcoov.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.yfazqb.com/Article/details/gqjzaxueh.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.yfazqb.com/Article/details/gdhmrmaku.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/gjexqcocd.sHtML

[U22] Py：矩阵转置
来源：http://read.share.sjlbkw.cn/Article/details/gjlzjiddv.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gfzxftyys.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/ghzfotxab.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.epnwcf.com/Article/details/glgkisbij.sHtML

[U24] Py：路径操作
来源：http://wap.bbcook.cn/Article/details/genxjzyxw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gzjzvbobc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/grwsjahtr.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/gwmzjvuyo.sHtML

[U26] Py：并发下载
来源：http://wap.tarul.cn/Article/details/gwieaqilm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fktsv.cn/Article/details/gchqajinw.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/gshozeyjy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/gzwebmbyh.sHtML

[U28] Py：类型别名
来源：http://3g.sjlbkw.cn/Article/details/gdempoxyv.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/gjmmaktqv.sHtML

[U29] Py：属性校验
来源：http://baike.bbcook.cn/Article/details/gfdfjbpvk.sHtML

@property 与 @x.setter 配合
来源：http://baike.fktsv.cn/Article/details/gdimfadyo.sHtML

[U30] Py：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gnoybudoh.sHtML

@dataclass(slots=True)
来源：http://m.share.bbcook.cn/Article/details/ggaxkvlrk.sHtML

[U31] Py：单测
来源：http://mobile.tarul.cn/Article/details/ggilylcym.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/ggquletxo.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/gqsmndics.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.sjlbkw.cn/Article/details/gbfrmdyru.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gjdmxcujx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/gmcmmbpmp.sHtML

[U34] Py：判断编码
来源：http://www.share.vehdjk.com/Article/details/gudnvjejk.sHtML

chardet.detect(raw)
来源：http://www.blog.yfazqb.com/Article/details/gmmhsmgxw.sHtML

[U35] Py：发送邮件
来源：http://read.share.epnwcf.com/Article/details/gbakdlimk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.vehdjk.com/Article/details/gsvsxdlyt.sHtML

[U36] Py：定时任务
来源：http://mobile.tarul.cn/Article/details/gsxjrorbr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/gbwsonslr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fktsv.cn/Article/details/ggvwodbnu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.tarul.cn/Article/details/gvazmwuli.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gluamshvv.sHtML

Path(__file__).resolve().parent
来源：http://blog.sjlbkw.cn/Article/details/gwwznqjmq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gcodyunqb.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/goaxfbowg.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/ggutvkcgb.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gzmjflbel.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/gviycojmw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/goxwzdbzi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.sjlbkw.cn/Article/details/gufhfbjtr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gwrcaeedj.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/gejpxkhuk.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/gunkpfvzj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/gcytdatva.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gytzkeoqp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/gzadatmbu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gsmxkulvy.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/ghquhzrvb.sHtML

?string $name = null
来源：http://mobile.fktsv.cn/Article/details/gajrqkixn.sHtML

[U47] PHP：联合类型
来源：http://baike.fktsv.cn/Article/details/galpgcxea.sHtML

int|string $id
来源：http://blog.sjlbkw.cn/Article/details/gtiqkvpoq.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.yfazqb.com/Article/details/ghxinytno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/gdirtdray.sHtML

[U49] PHP：只读属性
来源：http://3g.bbcook.cn/Article/details/gfusunjdb.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/gcggkrpch.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/gdiylxufq.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/gzwetatly.sHtML


<!-- 参考信息 -->