代发 wailian999

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/gxfdyoeul.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/grbopdzuh.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gligfzgdg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/gfufwwxfw.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gjurqvzir.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gwfjaxnnc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gkeotglbj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gljhcdwfj.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/gywbkhmje.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gvmdwgurx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/gzskcfszg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gedktmtqa.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gjgdtgyxq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/glkkkefwq.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gujjnqntk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/guokwjdga.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/grjpeidhu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gvhdcajgj.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gfsssghpn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gywuwqtvc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.bbcook.cn/Article/details/gealklyuo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/griqhxhte.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gcodudllp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gcfrulauh.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/gltkfqcoy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gemloeklx.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gujnqqwod.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/gwhkroyqw.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gckfynpij.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gbkssudrl.sHtML

[S46] C++：函数模板
来源：http://3g.epnwcf.com/Article/details/guyzuwjxo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/gyciwgsmk.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.tarul.cn/Article/details/gtlekellv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/guvbekfgj.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gytqzeawy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/glrufjxmg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gzbdbaqkd.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gpdrpqhwh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gyoruaeoj.sHtML

[S50] C++：格式化数字
来源：http://baike.epnwcf.com/Article/details/gwdzdldzl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gickbkkmv.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/gdzbktzru.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gwcirbvhk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gwkbbdwcq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gfzxlxgxs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/grvdpizqr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/grpxgqphx.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gukxfaofj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gjnamlbcs.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/gcvfglcfn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gkqgbejcj.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/goisuxcoh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gzkugvbrh.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/goyjqoljg.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gaajjuwaf.sHtML

[S58] C++：命名空间
来源：http://www.share.tarul.cn/Article/details/glcifyvsa.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gakgkyyyn.sHtML

[S59] C++：静态断言
来源：http://www.share.yfazqb.com/Article/details/gsyxmnazl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fktsv.cn/Article/details/gdpmluexh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gjvdysrgf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/gvwwetvpk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmbrhtwfz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.vehdjk.com/Article/details/gfyzsdhiq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggekwtdjh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/giibyojuv.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gfgervano.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/gpdlnhntk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/glaparswd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/gdgnrvuyn.sHtML

"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gqhoozqzs.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gyczqsvuy.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gewtqcgpd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gshhagmvk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gdarxvzlx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/gqbsvifur.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.tarul.cn/Article/details/ghbmnnbsw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gtolmqghz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/grselqxnd.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gkaekrnjz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/getwnomyl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/grsryaxij.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gxzdlcrcy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/gprufyupd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/ginclkfcl.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/garzrhptt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gpeggbqdj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.yfazqb.com/Article/details/gqbiavzqf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gvawhjvtg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzewptvl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gthwwylau.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gozifuixy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gvxkejisc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gkofeucdn.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gipyxphmi.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gjroueptb.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gqtlpyqnc.sHtML

[T17] Swift：变量与常量
来源：http://read.share.epnwcf.com/Article/details/grknadffc.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/gkqaibfgl.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gviavxxob.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gptbvmcdc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/ghnuzcsfp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gghihshci.sHtML

[T20] Swift：数组操作
来源：http://read.share.tarul.cn/Article/details/gnpgoxryr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gbmdyepph.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/gwjugiqfc.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/gbtvghkql.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gicmkadof.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gmjelapgd.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/gnraqquug.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gmlemauyl.sHtML

[T24] Swift：闭包
来源：http://m.share.vehdjk.com/Article/details/gvhjbzukh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gnsvqmqfk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/gljpzncli.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gqrhoecgd.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/glruqremi.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/grnexwvae.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gycoqwrjj.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gjdytrbyj.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gbhobyopb.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gyolvcfnk.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/givyvfqvi.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/gzxxeysek.sHtML

[T30] Swift：协议
来源：http://blog.sjlbkw.cn/Article/details/giuyihzrh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gzmtdkang.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gvjtiobua.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/ggovnciyr.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.bbcook.cn/Article/details/gzvftrjtz.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/gxgraivxc.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/geqhjzazy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gtqfszrup.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gzbbdnyeg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gcjujbtwi.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/gkpupeuwg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gfvdtjnqo.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gxwwfdeue.sHtML

function add(a, b) return a + b end
来源：http://3g.yfazqb.com/Article/details/gkqzeiywq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gahexmyya.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gmtngigpy.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/glscioeib.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gcnoqugen.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/ggmdefydr.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gwylpxgrf.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/gctehjvxl.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gicmtpwbg.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gilixdiia.sHtML

print "Hello\n";
来源：http://read.share.fktsv.cn/Article/details/gonodcinn.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/ggtwumwwo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gjklwsxnx.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/grbdcxeul.sHtML

"值: $a"
来源：http://m.share.yfazqb.com/Article/details/gnepcgdvy.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gtujjcscs.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gczjdkodv.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gpswbqwgj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.bbcook.cn/Article/details/gcnmsmayd.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/gmcxyifhy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.bbcook.cn/Article/details/gtgorefvr.sHtML

[T47] Perl：正则捕获
来源：http://3g.yfazqb.com/Article/details/gxsbgnjre.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.bbcook.cn/Article/details/ggisinxue.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gzqmgmsat.sHtML

$s =~ s/old/new/g;
来源：http://3g.epnwcf.com/Article/details/gmooehpig.sHtML

[T49] Perl：函数
来源：http://baike.fktsv.cn/Article/details/ggxmjphhr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gebcjqrjj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gxsrazgpu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/guwjddhxx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.sjlbkw.cn/Article/details/gibrncfzw.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gmeseilhr.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gdlyljmua.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gtbpamkfx.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gvkpnklwj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gatgfhlws.sHtML

s"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gdnucekon.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/ghwjardys.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.tarul.cn/Article/details/gwgdkxddj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/gmiaadhtv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.tarul.cn/Article/details/gxoykfrnp.sHtML

[T56] Scala：样例类
来源：http://m.share.yfazqb.com/Article/details/geugwhbvl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gjuxsonsu.sHtML

[T57] Scala：模式匹配
来源：http://baike.fktsv.cn/Article/details/ghimvzzgf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gkuwaomtr.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gcpqidrjm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.vehdjk.com/Article/details/gwahjfqzu.sHtML

[T59] Scala：循环
来源：http://mobile.epnwcf.com/Article/details/ggbtjlazq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gdgbmteek.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gjxoaacqj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.tarul.cn/Article/details/geguhggiy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjbltuzki.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gzvklpcmg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gviwotolu.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.vehdjk.com/Article/details/gxdcdcmbn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gcnqmumjv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/gzdikqshs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/gdfgtktid.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/gvcnlylif.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gsfqhhxsk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gtbdgagtz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.vehdjk.com/Article/details/gccqdrxog.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/gdxqjhzbd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gyohdmrpm.sHtML

[U06] Py：合并两个字典
来源：http://blog.epnwcf.com/Article/details/gwabidsfy.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/gzusvfkfw.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gvyyzulag.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.bbcook.cn/Article/details/gtbophxku.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gevyzjtzt.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gogkbcvuy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/germpfccg.sHtML

max(d, key=d.get)
来源：http://read.share.sjlbkw.cn/Article/details/gziuxcsle.sHtML

[U10] Py：按值排序字典
来源：http://3g.vehdjk.com/Article/details/gpecypwfl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gczxchwet.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gexuxcplq.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gyofzjuxc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fktsv.cn/Article/details/gypgkrpta.sHtML

Counter(arr).most_common(3)
来源：http://m.share.yfazqb.com/Article/details/gklmwxfpq.sHtML

[U13] Py：固定长度队列
来源：http://read.share.bbcook.cn/Article/details/glhddalme.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/gnviyrccp.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gyppwizcv.sHtML

defaultdict(list)
来源：http://m.share.sjlbkw.cn/Article/details/gathmaxco.sHtML

[U15] Py：高精度计时
来源：http://www.blog.tarul.cn/Article/details/gdpzsulke.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/gbrwzzgpq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.yfazqb.com/Article/details/gnqfbqczr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/gpcrvjrtt.sHtML

[U17] Py：初始化日志
来源：http://read.share.sjlbkw.cn/Article/details/glluqtobw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/gvwnfakev.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gactfnecs.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/galtzqowu.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/grxcjbhen.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/giswqcifx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.bbcook.cn/Article/details/gyprrdoml.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/gqrkhrstx.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.epnwcf.com/Article/details/gorpgpips.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gheboflfl.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gshxddhfg.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gcxidjxgw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/gxqnanfmj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.tarul.cn/Article/details/gdssdsxqu.sHtML

[U24] Py：路径操作
来源：http://www.blog.sjlbkw.cn/Article/details/gppmdwvjy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gvjobhwvo.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gxffbgpdf.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gjbrbtltd.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/grpkgsycc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.vehdjk.com/Article/details/gcnbhknec.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gmzaninik.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.vehdjk.com/Article/details/gubcpqyas.sHtML

[U28] Py：类型别名
来源：http://m.share.bbcook.cn/Article/details/gwylnscfq.sHtML

UserId = int
来源：http://www.blog.sjlbkw.cn/Article/details/gksnijaxt.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/gwezdtmuu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.epnwcf.com/Article/details/gczkvxdaq.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gutfzkgzy.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/glrumuqxo.sHtML

[U31] Py：单测
来源：http://wap.fktsv.cn/Article/details/godntjwvd.sHtML

python -m pytest -q
来源：http://blog.epnwcf.com/Article/details/ggqcwbley.sHtML

[U32] Py：代码格式化
来源：http://mobile.tarul.cn/Article/details/glisyvpkx.sHtML

ruff format . && ruff check --fix .
来源：http://blog.vehdjk.com/Article/details/gxvawfelj.sHtML

[U33] Py：打包发布
来源：http://www.share.sjlbkw.cn/Article/details/gcvvndfnp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gepjxgkiw.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gdrjcablb.sHtML

chardet.detect(raw)
来源：http://mobile.epnwcf.com/Article/details/gkzxegnhs.sHtML

[U35] Py：发送邮件
来源：http://www.blog.sjlbkw.cn/Article/details/gaafllgdf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.sjlbkw.cn/Article/details/gwuqmnbib.sHtML

[U36] Py：定时任务
来源：http://blog.sjlbkw.cn/Article/details/ggozdxmfa.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.tarul.cn/Article/details/gsjygufhv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.tarul.cn/Article/details/gwyueeshj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.vehdjk.com/Article/details/gojuttawv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.tarul.cn/Article/details/gxrvnvkbd.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fktsv.cn/Article/details/gtfwqrwnx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/ghxgwqhbl.sHtML

sys.stdout.isatty()
来源：http://www.blog.tarul.cn/Article/details/gxjnmqvcj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.epnwcf.com/Article/details/goauwpzzz.sHtML

print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gvqemuocg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gssgodoyf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.epnwcf.com/Article/details/ghtlqyxch.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/gjwbdbzyr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/gmmrytses.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.tarul.cn/Article/details/gqcxdnebq.sHtML

namespace App\Http;
来源：http://www.blog.vehdjk.com/Article/details/gggegpwxc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.tarul.cn/Article/details/gircmiyel.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/ghuajdfbq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.bbcook.cn/Article/details/gojytflsg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gxreoxlju.sHtML

[U46] PHP：可空类型
来源：http://3g.tarul.cn/Article/details/gqylaeuwq.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/gijbeiqgt.sHtML

[U47] PHP：联合类型
来源：http://3g.fktsv.cn/Article/details/gxdcwyjac.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/ggjesclre.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gpiuqrdbj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gvzwjyfxt.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gujfybxpj.sHtML

public readonly string $name
来源：http://www.share.tarul.cn/Article/details/gaixvjaso.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.epnwcf.com/Article/details/gchjdkpfh.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.tarul.cn/Article/details/gmgsdqdyj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.tarul.cn/Article/details/gdcntrzdx.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/gkrvqeozf.sHtML

[U52] PHP：箭头函数
来源：http://baike.bbcook.cn/Article/details/ggbrgodqp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gihxfzpfp.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/gasiyhztk.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.tarul.cn/Article/details/gouotquuf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.yfazqb.com/Article/details/gshldhbzq.sHtML

$obj?->method()
来源：http://wap.epnwcf.com/Article/details/gutvbpktz.sHtML

[U55] PHP：match 表达式
来源：http://read.share.vehdjk.com/Article/details/gwemidztz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.bbcook.cn/Article/details/gkbfdyhld.sHtML

[U56] PHP：命名参数
来源：http://mobile.vehdjk.com/Article/details/gbwyanrrl.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gyunagcxk.sHtML


<!-- 参考信息 -->