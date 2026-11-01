代发 wailian999

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/glithrtux.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/glpowawed.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/grnnwzxus.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gowvkuegz.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gwajhsozg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gqevfviab.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gpmokpglw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.tarul.cn/Article/details/ganncmqfs.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/gfbbdzbhz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gdbzvlggr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gtxnfjzik.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gcuqmxdtp.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gfmhrajhi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gizzrmkde.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gnmqwskdl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gulumbfns.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/ggrlupetu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gprljjsev.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/geekdjuxt.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gnhxfozhb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gmsqclrot.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fktsv.cn/Article/details/gkdholfdv.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/gweetbudr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gcvqyatxo.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gkxeftswo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gfymwnayq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkteodwhf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.yfazqb.com/Article/details/gpqgkpqqo.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/gwuyuales.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/ghonbbgyj.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gwvxhfghh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gyuzggqdy.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/gavkueejx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.bbcook.cn/Article/details/gfgerikxa.sHtML

[S46] C++：函数模板
来源：http://blog.bbcook.cn/Article/details/gvovodwoj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gryehhdvx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/ggntrxmwo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gbhqaiyer.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gflwgxnfi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gagirtavc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/gjnqmhtpw.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gmyvidopr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gbecxrjqv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gyfwwbsgt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gbgstmdtn.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gggglyfno.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gjzkchgyg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gwpexxjdv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gysxjzdyy.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/gwtijqyen.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/geohcrfwv.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/grtzsnrek.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gqkucoraf.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gafiyyret.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.tarul.cn/Article/details/gqgwtzqiq.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/gebbmkebv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/goaureuyt.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/ggdbxognt.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gnqkslirw.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/gtzggofpu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gvjkobrwd.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/ggwqddxmy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/gdrsosnvp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.sjlbkw.cn/Article/details/giqykbans.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gctiinstq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvrcqyqcw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gswixrkyc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvbghtnka.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/govgwmliw.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gvirvipna.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gjlzjjlvg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gplvjqmht.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gbijsrbln.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gpdgeizhd.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gtbxcvymh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gioixxcmm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/gmwlkqwmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/gxyottsrv.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gcgpuygmv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gykanxilt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gerrudeih.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gsgewcaft.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gongvcplh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gtjjqqaej.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.vehdjk.com/Article/details/gnlnhiqbd.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gwxzylcdd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gsecxfjcl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gbsemigdw.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gezupvgfv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/ggwovyjtc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gujaoqlqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/grobvzvjf.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gkqpbatry.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gkvntjohf.sHtML

[T14] Kotlin：循环
来源：http://3g.bbcook.cn/Article/details/ggloyizik.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gxqpbmtol.sHtML

[T15] Kotlin：接口
来源：http://mobile.vehdjk.com/Article/details/gchmdcfzq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/gmghurhrz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gflwuhgav.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/goxyphvuy.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gfpkksdxa.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/gktelwpaa.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gjegvudra.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/ghyeiewfy.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.bbcook.cn/Article/details/gqkdrvyex.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/gdqsnoidg.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gwbvvsycw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/giujsbeah.sHtML

[T21] Swift：遍历
来源：http://wap.epnwcf.com/Article/details/gkaqnywdj.sHtML

for x in a { print(x) }
来源：http://mobile.fktsv.cn/Article/details/gbthfvuim.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gaoufhdwx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/gmyqpbbjh.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/guhmzewae.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fktsv.cn/Article/details/goixdkpeb.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/guknizjuu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gxmmfjrkf.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/gkecfqmvj.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/glxxfxmlt.sHtML

[T26] Swift：类与重写
来源：http://wap.yfazqb.com/Article/details/gnvafpnla.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gujyfrvtw.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gqfrwbfkh.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gxzxbyche.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gpqfneagi.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gyoehsprf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/gbvmsdrql.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gwqrldcde.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gsymywicz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gakoujaeg.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gbpgiodau.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gkzowcytt.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/ggrxkjdyg.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gwekxsqlf.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gcbdfghze.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.bbcook.cn/Article/details/gupeuicze.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gscpyxxkf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gqpjyznis.sHtML

[T35] Lua：字典表
来源：http://wap.yfazqb.com/Article/details/gxnynvovo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gfknwpzek.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/gluwssvjw.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gcammjbac.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/gyvyfllyx.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gklsygnns.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/ghxyqjhjo.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/genqiidjd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gkijyiysy.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/gyccnxafm.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/gtprrondr.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gorpskveq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gwxacyevm.sHtML

print "Hello\n";
来源：http://wap.vehdjk.com/Article/details/gaurncozl.sHtML

[T42] Perl：变量类型
来源：http://blog.tarul.cn/Article/details/gqhzzemfz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/gkmfyreot.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gpyfkoefc.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gthmfauig.sHtML

[T44] Perl：条件
来源：http://www.m.share.tarul.cn/Article/details/gjrheqfpr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/gtavbjchj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gsjzcfomj.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gxxfcnits.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/gfjksrhbg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gracgwhkl.sHtML

[T47] Perl：正则捕获
来源：http://baike.sjlbkw.cn/Article/details/gxadxvzij.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gtqsfeovx.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gthbkqsqi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.tarul.cn/Article/details/gfdafuvbn.sHtML

[T49] Perl：函数
来源：http://read.share.tarul.cn/Article/details/ggrskgych.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/grsznbvvg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gujwcehlt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/gxqzhfosj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gprxbbxta.sHtML

[T51] Scala：Hello World
来源：http://baike.tarul.cn/Article/details/gnvlttisx.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gjfezsxxx.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gpiqlrchy.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/gkmzjwnpo.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/gmcffptdu.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gjipprmaq.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gvlnuouex.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gqesoakul.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gindrkhxg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gzrmqapdz.sHtML

[T56] Scala：样例类
来源：http://read.share.fktsv.cn/Article/details/gsnximqie.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gsfbhlcfp.sHtML

[T57] Scala：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/grfkrjsys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gvseradee.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/gwflteapt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gvhvvnxcn.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gxrtxmczg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gbfizowsz.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gklzapivn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.tarul.cn/Article/details/givmvborb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gayvukjoe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gnaaidbas.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gheasgezk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.sjlbkw.cn/Article/details/gsicnorrj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gbghjrlov.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gecfwzxvl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gpdktufmh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gptqryobh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gxjhedibz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gnvabbfpc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/grxfjcyqd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fktsv.cn/Article/details/gwdamjxxa.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gklhfgtix.sHtML

[U06] Py：合并两个字典
来源：http://www.share.sjlbkw.cn/Article/details/gdpdqnxll.sHtML

{**a, **b}
来源：http://blog.bbcook.cn/Article/details/grkjepayw.sHtML

[U07] Py：反转字典键值
来源：http://baike.fktsv.cn/Article/details/gsgakaqbg.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/gfocemmtn.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.vehdjk.com/Article/details/gxyqwgpeb.sHtML

[y for x in nested for y in x]
来源：http://blog.yfazqb.com/Article/details/gufsbwsdk.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.vehdjk.com/Article/details/gtnznrkts.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/glzefyrbv.sHtML

[U10] Py：按值排序字典
来源：http://blog.sjlbkw.cn/Article/details/gjsfbkmrk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.epnwcf.com/Article/details/gkximhlhq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gizsyxwot.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gppffpdcg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/gsibjfptp.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gazyoiuzl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/gvdgmymdb.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gqlqzitlk.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/gkgdsgbnh.sHtML

defaultdict(list)
来源：http://wap.epnwcf.com/Article/details/gmclzbind.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gfubryspd.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gwddfajvx.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/gqsmshxxf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/gkaycfdlf.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/glglsollw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.sjlbkw.cn/Article/details/gzjhoqxmp.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/gzeockenv.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gyjwphjuw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.sjlbkw.cn/Article/details/gjqsjwktc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/gxudmcvso.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqgankmn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/gxlpxgqoe.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.vehdjk.com/Article/details/gyqnwnyqq.sHtML

@contextlib.contextmanager
来源：http://mobile.bbcook.cn/Article/details/gqgpuetxw.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gekogwukj.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/guxbmelus.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gnvalcrpn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/gcbllqiiw.sHtML

[U24] Py：路径操作
来源：http://m.share.epnwcf.com/Article/details/gldgyrfag.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gxavjdhkl.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gtwiglgpe.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/gzzzbscca.sHtML

[U26] Py：并发下载
来源：http://3g.sjlbkw.cn/Article/details/gsafmxobd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.epnwcf.com/Article/details/gelkbpqpk.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/gomngubpm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gvvfovokw.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/getofdhzj.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfvylklo.sHtML

[U29] Py：属性校验
来源：http://www.blog.yfazqb.com/Article/details/gwpiefvgi.sHtML

@property 与 @x.setter 配合
来源：http://read.share.yfazqb.com/Article/details/gvqyviekz.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/guvxcmosf.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gpdxrfbjf.sHtML

[U31] Py：单测
来源：http://blog.vehdjk.com/Article/details/gautzbyeg.sHtML

python -m pytest -q
来源：http://wap.sjlbkw.cn/Article/details/gusweqevu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/gfciqymyk.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gtoxqiwcp.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/gafjgnozy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/geimkvayo.sHtML

[U34] Py：判断编码
来源：http://mobile.fktsv.cn/Article/details/gzlqyfftn.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gcxtqseef.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/goyqjyahr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fktsv.cn/Article/details/gvtrcvwkh.sHtML

[U36] Py：定时任务
来源：http://m.share.vehdjk.com/Article/details/gzhabziom.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/gpokuocrw.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gkdpmbswi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/grmqsdcnu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.sjlbkw.cn/Article/details/gnkiunzvc.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gnssckreg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.sjlbkw.cn/Article/details/gdptqspcf.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gtkmsqzyt.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gscfdoadn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gyzkmkorm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/gmndqswfi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gjpeddcif.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.sjlbkw.cn/Article/details/gldysthhl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fktsv.cn/Article/details/gktzekvpe.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.bbcook.cn/Article/details/ggmamgwyh.sHtML

namespace App\Http;
来源：http://read.share.fktsv.cn/Article/details/gxmsfsitz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gegvlflvu.sHtML

declare(strict_types=1);
来源：http://blog.bbcook.cn/Article/details/goitrlyvx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.yfazqb.com/Article/details/gtzwakijr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gykrradoa.sHtML

[U46] PHP：可空类型
来源：http://blog.tarul.cn/Article/details/glmbpmefc.sHtML

?string $name = null
来源：http://www.share.tarul.cn/Article/details/ghhxgphqe.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/gxbjtoxfq.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/gtwxlqklb.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/gkgoczdnl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.vehdjk.com/Article/details/gzncbqtxr.sHtML

[U49] PHP：只读属性
来源：http://read.share.epnwcf.com/Article/details/gdpqzoygz.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gqmgyfxjm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.bbcook.cn/Article/details/gudjqzshs.sHtML

public function __construct(private int $id) {}
来源：http://3g.sjlbkw.cn/Article/details/gdkhxmvqh.sHtML

[U51] PHP：数组解构
来源：http://m.share.epnwcf.com/Article/details/gbyzwwfoh.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/gvayppibk.sHtML

[U52] PHP：箭头函数
来源：http://read.share.vehdjk.com/Article/details/ghvpqcqff.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/grusfmdkm.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/goiolrwyu.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.yfazqb.com/Article/details/gsmxzimss.sHtML

[U54] PHP：空安全调用
来源：http://m.share.vehdjk.com/Article/details/gucnwspud.sHtML

$obj?->method()
来源：http://m.share.yfazqb.com/Article/details/gwuapsnsw.sHtML


<!-- 参考信息 -->