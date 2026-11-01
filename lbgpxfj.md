代发 wailian999

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gmkzqigqd.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/gigosdpit.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gtytygzqb.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gqgbbnqxv.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gxiizuqpd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/grioujrtk.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gxirnncmd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gwiizmcpz.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/gemrdgxvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gexqvkotc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gpgzmgklu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gtqqdphoq.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gjapedawq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ggtwukmsn.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gnuooyhmg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gbqvweptu.sHtML

[S37] C++：set
来源：http://www.blog.epnwcf.com/Article/details/gmqkckvuo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/guqxzykrt.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/ggzkrzaxx.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/gwlwutpqs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gbifdhvcs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gfpwujxan.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/gwksfqrtr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gjnwopcqb.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gkcvvejgm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gwuwsrqlt.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gxhztzcvo.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gsmgdmeay.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gwupwisck.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/ggqnyayfy.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gxlfilhhc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gwwnnyzil.sHtML

[S45] C++：lambda
来源：http://baike.sjlbkw.cn/Article/details/gtbkoiyas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gtiwjyldz.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gywypiptt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gfmuhzzue.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gtlczywuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gmcbrhmuq.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gdqclkyfa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/ggpuumtzq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/goyfrbtpc.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/gtqwxxjrm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.tarul.cn/Article/details/gadigupfx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gngmqxxgl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/glazzbyev.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gzuplvssy.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/ghgwoxasl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/glppymccb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gbhajdjpy.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/gvweugfoo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/gnmqinsrt.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gowxupygr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gilvlrclf.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gqibnzpxa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gkwwdlqtx.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/gibfnsqcf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.yfazqb.com/Article/details/gznxaexso.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/gkvqikdvq.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gmubchven.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gqvhlwizd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gzhgcirbf.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gtdpgofcw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gxjrongnd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gqhwucggm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gnwkqrclg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/galdziavj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gkbsaqbmi.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpwdtpkzt.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gwvijctif.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gukdokcka.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gisgtxali.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gfhuickzr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/gbtacavxr.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gdxtqbuui.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gmffjnmii.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/givejmiit.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/gstwhjjre.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gzfglmxsf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gknjphlkg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gleitctex.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gmsnesosi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gzgiiwndz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/grvtkxigv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gxoyrmokf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/gbmjmouvs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/grwthizha.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gkpjatsvj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gvukncrqg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gysuylelh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gdkmicbrj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gvoenokzw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/glwchcwkh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gowpdzeix.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/gpxykhifd.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gbwelwgbx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gekdjwztv.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gtgofxioh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gnxojnlds.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gejpgvjbg.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gqgahkdkc.sHtML

[T17] Swift：变量与常量
来源：http://m.share.epnwcf.com/Article/details/gjtczijcl.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/gtsqjlxyv.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gwmusajji.sHtML

"值: \(b)"
来源：http://wap.sjlbkw.cn/Article/details/ghnbmiklo.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gxvswmfni.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gzfpahdsf.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/gfphlnxda.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gyqfpknbb.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/grpsovali.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gtzabisnk.sHtML

[T22] Swift：字典
来源：http://3g.yfazqb.com/Article/details/gbexduoim.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gsqeyasxd.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/ghmeeuoxv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gmivtfmag.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gsuoieeqk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/grooljecu.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/gxfyzmrvd.sHtML

struct P { var x: Int }
来源：http://www.blog.bbcook.cn/Article/details/gxzlzafrf.sHtML

[T26] Swift：类与重写
来源：http://baike.epnwcf.com/Article/details/gvbrlnlgt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gvzxdgvpp.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gihzjwlah.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gbbrcfskl.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gemjhzeah.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/giksnlvde.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/goaaodyxe.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gmdbbjhhj.sHtML

[T30] Swift：协议
来源：http://wap.yfazqb.com/Article/details/gmjjwokke.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gyzcirvfm.sHtML

[T31] Lua：Hello World
来源：http://www.share.tarul.cn/Article/details/gfumycoau.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gwuxmmusl.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/gevrmlhle.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gtaytmnbf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/guektkwle.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gqmutdwic.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/grbodqksk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/ganvolgls.sHtML

[T35] Lua：字典表
来源：http://www.blog.vehdjk.com/Article/details/gjymqmgzi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.tarul.cn/Article/details/gseufcndb.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/gpbchgfiv.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gysqolxeb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gxmrtotqa.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/gdqwyufyi.sHtML

[T38] Lua：条件
来源：http://mobile.epnwcf.com/Article/details/gdqavxbed.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/gtkpjmwjf.sHtML

[T39] Lua：模式匹配
来源：http://3g.tarul.cn/Article/details/gdosedlgf.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/grtfridsf.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/gxveqhnvf.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/glrpmxwxc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gbrjonmby.sHtML

print "Hello\n";
来源：http://m.share.sjlbkw.cn/Article/details/gtkuhrwgw.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gmaedvnis.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fktsv.cn/Article/details/gdwxhcumg.sHtML

[T43] Perl：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/guwixxppq.sHtML

"值: $a"
来源：http://mobile.vehdjk.com/Article/details/ghwbbasdr.sHtML

[T44] Perl：条件
来源：http://m.share.tarul.cn/Article/details/gpdynbfck.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gfduiycrm.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/gwvtmkdax.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.yfazqb.com/Article/details/gvmpgzpxf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gaxqmvxzq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/gvxrgaqpz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gktmpavxi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/gsmcxvpsy.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gifvaqxru.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gpundwicf.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gvvflctgm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gobovnucg.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gdcikjsjj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gagjmcpxq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gzcmpjukh.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/gaxuumzdm.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/grkundlhc.sHtML

[T52] Scala：变量
来源：http://www.share.vehdjk.com/Article/details/gtxbulskc.sHtML

val a = 1;  var b = 2
来源：http://www.share.epnwcf.com/Article/details/goxeppblf.sHtML

[T53] Scala：字符串插值
来源：http://blog.epnwcf.com/Article/details/gvmskpunr.sHtML

s"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gcenycenu.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gmzojxfmd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.yfazqb.com/Article/details/gpatdflnn.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gmlsvwzbc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gyymqhflh.sHtML

[T56] Scala：样例类
来源：http://mobile.vehdjk.com/Article/details/gqumhmgrc.sHtML

case class User(name: String, age: Int)
来源：http://3g.vehdjk.com/Article/details/gmmsrvsuz.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gkfifqlun.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gtphiabvi.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/gigpbxsmv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gpxryjmci.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/gjxllddeo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.vehdjk.com/Article/details/gkbvnchvu.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gybcrxaoh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/ghkxecidz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/guozlimoe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gaohwwvfh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxgdpuebk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gnrdbwokc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.sjlbkw.cn/Article/details/ghmeyyjkn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gsnticljg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/gybuwjafq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.epnwcf.com/Article/details/gcsozbnje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gtwhoipkm.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/guenfipsr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gtodxrkwr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/gxrepkrkv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gzbidcetu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gzirxgzmc.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/goookncgv.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/gendsxsdy.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fktsv.cn/Article/details/ghuizzwye.sHtML

[U08] Py：展平二维列表
来源：http://blog.sjlbkw.cn/Article/details/gjsdrvpql.sHtML

[y for x in nested for y in x]
来源：http://mobile.epnwcf.com/Article/details/gbzzfmdzv.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.epnwcf.com/Article/details/grtrabhra.sHtML

max(d, key=d.get)
来源：http://www.m.share.tarul.cn/Article/details/gkwyojddp.sHtML

[U10] Py：按值排序字典
来源：http://baike.tarul.cn/Article/details/gbmfqwjuj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fktsv.cn/Article/details/giyijqyyk.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gudvnjpcq.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/gkshvyblc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/glgsggber.sHtML

Counter(arr).most_common(3)
来源：http://blog.epnwcf.com/Article/details/gqiyuajwr.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/gqxloyvsw.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/guhrlpohb.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.bbcook.cn/Article/details/guzpmhsce.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/glkchaiut.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/gtlmrenlj.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gclxsebrz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fktsv.cn/Article/details/gklhkhini.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/gnmyxxemn.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/garqrywgp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gefvrbzwh.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/gmzzyudtc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gpzpkgxwg.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gxgsmkpmz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.yfazqb.com/Article/details/glzozkxwz.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/ghhfowljd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/gnugmpazd.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/gwzhauxek.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/ghvdfjirq.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gqcyjjpkh.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gwstkkzmp.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/gavrqsshz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.epnwcf.com/Article/details/gcclrmtld.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gchlngygd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/godhieiqp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.yfazqb.com/Article/details/gqvwiyggy.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/gdohfijho.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gtqntumzo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fktsv.cn/Article/details/gkzxoflkm.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/geliqrlsn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.vehdjk.com/Article/details/gsgvtdayr.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gklirlhbi.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/gsizvdtbf.sHtML

[U29] Py：属性校验
来源：http://m.share.yfazqb.com/Article/details/gwbwtjmfw.sHtML

@property 与 @x.setter 配合
来源：http://mobile.yfazqb.com/Article/details/gczpxfelv.sHtML

[U30] Py：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gomjnxksb.sHtML

@dataclass(slots=True)
来源：http://3g.bbcook.cn/Article/details/ghypcndib.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/geivyuurn.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gkkmpzush.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/gnollxzbe.sHtML

ruff format . && ruff check --fix .
来源：http://wap.tarul.cn/Article/details/gcfgqkpvk.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/ggpjhsrcx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.tarul.cn/Article/details/gtflnfnyn.sHtML

[U34] Py：判断编码
来源：http://read.share.tarul.cn/Article/details/gxupovktr.sHtML

chardet.detect(raw)
来源：http://www.blog.fktsv.cn/Article/details/ghjfblmxn.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gkjsxziua.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.epnwcf.com/Article/details/gsniendfc.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/gjcukuzhh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gtvomtftr.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/greotbgcx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gyvmtauqb.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.epnwcf.com/Article/details/gljuotlif.sHtML

Path(__file__).resolve().parent
来源：http://wap.epnwcf.com/Article/details/gvakpaown.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/gxmhfpolv.sHtML

sys.stdout.isatty()
来源：http://www.blog.sjlbkw.cn/Article/details/gmyldgcer.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fktsv.cn/Article/details/gbdwmzohx.sHtML

print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/goxtbmelh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/gvgkxvdzn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gszkryllb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.bbcook.cn/Article/details/gjsdqeqcn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/gukpknfer.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gjevbrqzk.sHtML

namespace App\Http;
来源：http://mobile.epnwcf.com/Article/details/gwilgpvvo.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.yfazqb.com/Article/details/gaxxeoeoy.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/gnfatgfgy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fktsv.cn/Article/details/gpchxmfdf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gxlwxaszr.sHtML

[U46] PHP：可空类型
来源：http://wap.sjlbkw.cn/Article/details/gunzhyjdo.sHtML

?string $name = null
来源：http://www.blog.bbcook.cn/Article/details/gexqmjurb.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/gpwnrvwhl.sHtML

int|string $id
来源：http://3g.sjlbkw.cn/Article/details/gzirhfkmf.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/gsiduunwf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fktsv.cn/Article/details/gkerzrfyp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.epnwcf.com/Article/details/gfdvlpaav.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/gnzlpadyq.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.bbcook.cn/Article/details/gsatxtnjw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/gbczuolqr.sHtML

[U51] PHP：数组解构
来源：http://3g.bbcook.cn/Article/details/glloxlthv.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/gyvoowzcp.sHtML

[U52] PHP：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gmatxrlyk.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.epnwcf.com/Article/details/grjnsectu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.vehdjk.com/Article/details/giowkszfg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gqrkddnob.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gelxdbshf.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gbdgpuiiy.sHtML


<!-- 参考信息 -->