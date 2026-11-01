代发 wailian999

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gexxfhxrn.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/geipuzqtx.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gqrersvot.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gvatlqnts.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/gpdqwpfcv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gtxaioliw.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gppilcuor.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gbtwwxmvp.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gnutbufuo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/gikliyugu.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gzzigcvkm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gkpmoyqqr.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gcwgaxkcj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gjyyyookh.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gwfbvppwm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gjaezzhzt.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gbmuiqxef.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gredpmjva.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gbaqkzbzo.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gcdjgroek.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gfyquglmp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gsqntyhzw.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/guyeurfag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/gmqnpzhtt.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gmcfndplw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gxtgdgyhg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gjcicshbh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gvjmqvaus.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/gghspqhaw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gtiiepwme.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gwblqinlo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gickzywkd.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gpyiowesw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.vehdjk.com/Article/details/gfzwkfxnj.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/gqrhcgdqn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/gguoshhxz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gwixmaipw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gwfztrufb.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gbkpujkvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gwxqgsdeh.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gfhfbejoz.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/griawtxbk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gbeckmooq.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gwkrcdyyp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gdyvzxqkr.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gnufsjrof.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gfiotbxto.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/gcjiexfqf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gbygodqyl.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gimtepzxu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/gtbjiktrr.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gggfjguty.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/ggolxhvxj.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/grikfkkou.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gnsarohff.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gpsnxzxgy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gprtyzdac.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gezqmslih.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gmjvityyo.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/glxihqllg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gbknbeqos.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/ghltbhpkn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gvcnjobro.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/gkrynwtmm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gojawoolr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/govzrkxkg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gdxsgkbxp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfinicosc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gwkuvazjv.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gtyyckxxc.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gcsslwtra.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gianykiwd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gqgpzqlhg.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gbestakkq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/gnitiadmn.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/glcsrqjih.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gtjgnhfcd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/grshmygvu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/gougyqvxi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gisgdpoof.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gqeacrwuq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gryjtdodv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gjsnrribm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/glhdhjqdp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gpxpzbyxe.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gohiqxccj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gceuthpao.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gyelzsrle.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gwguqever.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/grucdqbbt.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.vehdjk.com/Article/details/ghlzwybyz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/gqmrmlump.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gglzqbmvo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gqurzofjr.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gffvbrcux.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/gimxdnnxu.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/gnpktatnv.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gbqusucgs.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gkswjodkb.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/giyvsbqsr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gsnvsquxe.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/gmixuxxqi.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gzigdxbtx.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/groebysou.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gpetyiovw.sHtML

if let n = opt { print(n) }
来源：http://baike.epnwcf.com/Article/details/gmiujceqv.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gyholwogl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gnmgnusnn.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gbwiwymup.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gzsuvgcgd.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gnlxoifcy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gzfxrtzsu.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/gbvpaetnp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/gnnspmcyd.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gsmuzugoj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/gwvfgnjql.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/gbiwzsypu.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gahrsutwu.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.epnwcf.com/Article/details/gaikvrkyg.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/gzhqwgzru.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/ggsomfddt.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/ganhzcoeo.sHtML

[T28] Swift：枚举
来源：http://read.share.tarul.cn/Article/details/gtfchiymw.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/grluyiykt.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gaircohpi.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/grczuzkrn.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/giakriubu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.yfazqb.com/Article/details/gjqxildwz.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/ggvnaoqhn.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/grbawgrfl.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gnoijzibp.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gculyjegg.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/ggxpfscie.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.epnwcf.com/Article/details/gbbwelmqs.sHtML

[T34] Lua：遍历表
来源：http://read.share.epnwcf.com/Article/details/gawonvige.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.bbcook.cn/Article/details/gwxzwkled.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/gyfwbwayu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/goxccmthh.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/glnhopche.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gxlexqbve.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gzigpsise.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/geqphopvo.sHtML

[T38] Lua：条件
来源：http://mobile.fktsv.cn/Article/details/gixsgyuyj.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/gnzxwykuw.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/gmyswyeqt.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/geshgwoil.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/gfsxbnbib.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/gepfhbmhb.sHtML

[T41] Perl：Hello World
来源：http://m.share.tarul.cn/Article/details/gwugbvmvj.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gkfsinruq.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/gnrxheoki.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/globpqmkl.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/ggqdplmul.sHtML

"值: $a"
来源：http://mobile.tarul.cn/Article/details/gtuqcbznj.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/ghvqquslp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gqlgppavv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gyhmerwue.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.sjlbkw.cn/Article/details/gdnruxbdm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gfulspmpn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.sjlbkw.cn/Article/details/gnohfaopr.sHtML

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/grfhnexpn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/glmuhdswl.sHtML

[T48] Perl：正则替换
来源：http://blog.epnwcf.com/Article/details/glybrecqa.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.bbcook.cn/Article/details/ghpwbmlul.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/ghfqjspsd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/goagtmptv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gtwcquzfu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.yfazqb.com/Article/details/gstlhvvnt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/ggdbijyjt.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/gjujqhsur.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gpscqgcaw.sHtML

[T52] Scala：变量
来源：http://blog.yfazqb.com/Article/details/gukuydejg.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gxzduiyjb.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gkwkncyen.sHtML

s"值: $b"
来源：http://baike.bbcook.cn/Article/details/gawnwxsqm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/ghzpbdtev.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gbkiksawr.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gfxhoeliv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/gixcruwkb.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gartsofnl.sHtML

case class User(name: String, age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gpaiwniex.sHtML

[T57] Scala：模式匹配
来源：http://3g.tarul.cn/Article/details/gtnkodwlp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gwnwcaygh.sHtML

[T58] Scala：函数定义
来源：http://mobile.bbcook.cn/Article/details/gnpqqlelh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gqnscspmd.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gaaoxrpal.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gchrbxykq.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/gcbjnpdvo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/ggjtvsyfj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glnorwtoa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gfbxtenol.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/griczptnf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/gcyflsstl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gekwtckin.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gmbljfdqd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fktsv.cn/Article/details/gcjwfqyoz.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gtyyfiqsl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gmrqvnrnj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gafithgjs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/grcbgnljo.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.yfazqb.com/Article/details/gjtnacyca.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gvxssqned.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gugyfwbfw.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gjbvmjhmq.sHtML

[U07] Py：反转字典键值
来源：http://blog.fktsv.cn/Article/details/grheaxagm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gadgbqfbz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/gjkiqldcl.sHtML

[y for x in nested for y in x]
来源：http://read.share.sjlbkw.cn/Article/details/gueskwdca.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.sjlbkw.cn/Article/details/gdqrwfqkr.sHtML

max(d, key=d.get)
来源：http://blog.tarul.cn/Article/details/gzxrltkuy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.yfazqb.com/Article/details/gzfcllvnq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gdcdnuinb.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/gbortaytb.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gohuvdkgv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/gutktwcaa.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gowscemvx.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/ggbemcfin.sHtML

deque(maxlen=10)
来源：http://mobile.fktsv.cn/Article/details/gsryqftyq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gztwutrur.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gcxduncso.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/gbafwixti.sHtML

t = time.perf_counter()
来源：http://www.blog.sjlbkw.cn/Article/details/gjoeoqhmf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.yfazqb.com/Article/details/gtinqpmvp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/gjtasbdzi.sHtML

[U17] Py：初始化日志
来源：http://blog.sjlbkw.cn/Article/details/grxteuyjl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/gzqicbxhm.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/guajlddpo.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gxqysrmnw.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.vehdjk.com/Article/details/gghcrizrl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/guhlzfpib.sHtML

[U20] Py：缓存函数结果
来源：http://baike.yfazqb.com/Article/details/gyoxnjoty.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gshucijgs.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.yfazqb.com/Article/details/gvrajwvsa.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/gomcprrca.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/guetrtsht.sHtML

list(zip(*m))
来源：http://wap.epnwcf.com/Article/details/gyjydhljq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/gkyqbhxdk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gcmkpoybo.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/ghjnajkbp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gemzbakwl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/gllsbimgq.sHtML

csv.DictReader(f)
来源：http://wap.sjlbkw.cn/Article/details/gfsnehjej.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/gtjiozrcv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/gspjarxjm.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/gvaegsgox.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.epnwcf.com/Article/details/gittkkgqr.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/glvwgthjm.sHtML

UserId = int
来源：http://www.blog.epnwcf.com/Article/details/gyplaggym.sHtML

[U29] Py：属性校验
来源：http://blog.fktsv.cn/Article/details/goyejttsz.sHtML

@property 与 @x.setter 配合
来源：http://wap.vehdjk.com/Article/details/gsvsyfhkk.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gylklkhbm.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/glkkhfilg.sHtML

[U31] Py：单测
来源：http://read.share.fktsv.cn/Article/details/gfqnuxatc.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/gcodzqcty.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/gqwdmhawn.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.vehdjk.com/Article/details/gbavpauej.sHtML

[U33] Py：打包发布
来源：http://www.share.sjlbkw.cn/Article/details/gzsmnujsc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/giitudbuq.sHtML

[U34] Py：判断编码
来源：http://www.blog.bbcook.cn/Article/details/gozkbwegj.sHtML

chardet.detect(raw)
来源：http://www.m.share.bbcook.cn/Article/details/gsdrzdubb.sHtML

[U35] Py：发送邮件
来源：http://blog.epnwcf.com/Article/details/gokgjekef.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghspwnnaw.sHtML

[U36] Py：定时任务
来源：http://m.share.epnwcf.com/Article/details/gjhvhxhwj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gsarnqenu.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.vehdjk.com/Article/details/gwfmivczz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/gtrgagecp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.vehdjk.com/Article/details/ggueyloma.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gjdnlkfhb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/gafxfkeip.sHtML

sys.stdout.isatty()
来源：http://www.blog.yfazqb.com/Article/details/gfaaovayg.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.bbcook.cn/Article/details/gzbqtulrp.sHtML

print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/ggydsqrtb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.vehdjk.com/Article/details/gnrfobwut.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.epnwcf.com/Article/details/grkfjquuq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.vehdjk.com/Article/details/gdqdwkfzk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.bbcook.cn/Article/details/gllwqdvug.sHtML

[U43] PHP：声明命名空间
来源：http://3g.yfazqb.com/Article/details/gtaeghbic.sHtML

namespace App\Http;
来源：http://wap.bbcook.cn/Article/details/gnjvadydt.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.yfazqb.com/Article/details/gwfqabjuy.sHtML

declare(strict_types=1);
来源：http://mobile.vehdjk.com/Article/details/gjpcqjjop.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gpgfnquew.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gthefoxqe.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/gfpjyibqh.sHtML

?string $name = null
来源：http://blog.yfazqb.com/Article/details/gznwoqqcm.sHtML

[U47] PHP：联合类型
来源：http://www.share.yfazqb.com/Article/details/goanhvcfc.sHtML

int|string $id
来源：http://blog.tarul.cn/Article/details/guxyywpcw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/glpjrhigd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gxsmgteoa.sHtML

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/gevxccjmf.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/gdwuqgckt.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gyzgbohvn.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gepiyhmon.sHtML

[U51] PHP：数组解构
来源：http://blog.vehdjk.com/Article/details/gegxcndzs.sHtML

[$a, $b] = $arr;
来源：http://3g.tarul.cn/Article/details/gtimmfvez.sHtML

[U52] PHP：箭头函数
来源：http://mobile.yfazqb.com/Article/details/glqzmykpm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.epnwcf.com/Article/details/ghgpfpaqj.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gwspesjit.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.bbcook.cn/Article/details/gvampxoms.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/giypaadxl.sHtML

$obj?->method()
来源：http://baike.epnwcf.com/Article/details/gnajkxpdy.sHtML


<!-- 参考信息 -->