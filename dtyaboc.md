代发 wailian999

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gelqujjro.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gyypbrvsv.sHtML

[S32] C++：字符串
来源：http://3g.sjlbkw.cn/Article/details/gpxvhpjah.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gnfjjzpes.sHtML

[S33] C++：vector 增删
来源：http://wap.tarul.cn/Article/details/gawqtpltn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fktsv.cn/Article/details/grinzamap.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gvubdknhg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/gpkwwvbvo.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gdtcnjcma.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gptibjpkl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/gyftutasj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gxslgptwj.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gaadmiqsi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/gbtuyssry.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gzzevasrf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/gtrvjlpbj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gfnnlizsa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqdqicxx.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gslwptney.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gjmlzikkm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gclulqsuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gvrxrpydg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gribuyugy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.bbcook.cn/Article/details/gulcndyfi.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/ghemdkkwz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gvvtpqxgq.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/ghohpgcsc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/gufftfvog.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/giavoaurj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/gnwuceqsw.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gwggjukgc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gdcgdhote.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gfyncyopo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gtcrxopip.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/godurgdbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.bbcook.cn/Article/details/gfwyotuqf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gltrkefob.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gynfjovee.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gdyfuamnw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.tarul.cn/Article/details/gpvqjktfq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/garfqvnru.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/goyurhqbn.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/ghmhfjzms.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gbotxvsjf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gxtoymygd.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gobuucmhc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gpsyscimg.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gjzhtodqo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gexywvybp.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/gyzrjlyib.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gnyiuuhls.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gzrvivyth.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/grlfbiuss.sHtML

[S57] C++：编译期常量
来源：http://mobile.vehdjk.com/Article/details/gkepiewqj.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/gmojrjngh.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gurhvzppr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/ghxfbrhfj.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gegatggyk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gibhtzftm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/gokvwymjz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gnseptvun.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkkoqysgz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gaekyngja.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghtxivdmv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/ghgqlwyoc.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gxtrptilq.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/guezudgns.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/grgxjpmll.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gommyoffw.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/gvuvhzdyv.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gbdqljezw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gavylewnj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gpstfdtsw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/glqtgqqrz.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/gtslekjwj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gfpgpacyl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gfutxrrza.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gznjhgprg.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/gdrrkfmen.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gubzmqbes.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.tarul.cn/Article/details/glnnlibxq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/grdatkene.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gyqiayaqg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/gqisenzuv.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gqfjwbaes.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/glwxlegiu.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/gzashievc.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gqeqtmowz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gzlcaavzw.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gbqcblcyr.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gsyiqackk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gubxqrvht.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/ggwwdoioq.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/ghqhypefg.sHtML

[T16] Swift：Hello World
来源：http://baike.tarul.cn/Article/details/ganpafwna.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/ghphkfjia.sHtML

[T17] Swift：变量与常量
来源：http://wap.bbcook.cn/Article/details/gtyearxnx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gpuxxhqkj.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gxnkmdzmg.sHtML

"值: \(b)"
来源：http://baike.sjlbkw.cn/Article/details/gsrmnpmpf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gvhfwwygl.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gcoswocja.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/gbhgjmcud.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gjkolbbbk.sHtML

[T21] Swift：遍历
来源：http://baike.vehdjk.com/Article/details/gggwshodo.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/giemdgevc.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/gtzwulmiq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/ganugkzmd.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gxzxeitsf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/grcfrawri.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/gspciggcf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gvrwqqnar.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gffbnfxyq.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/ghbcmvmzn.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gjinnnafg.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/grvefizuv.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/goizrghxr.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gbidgqbzr.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/gelmvgosz.sHtML

enum Color { case red, green }
来源：http://baike.sjlbkw.cn/Article/details/gmxrjbvts.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gnwrmuzbk.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gmdfqvvqy.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gjkhadpgu.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/gxfwfejvr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkggznmi.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/geyvtojyo.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gvdadporv.sHtML

local a = 1
来源：http://blog.epnwcf.com/Article/details/gwluiehnm.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/gjmnmxnmw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gyolrmptp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gqjfymflh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyynnhum.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gantayeaa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/gopufpqlb.sHtML

[T36] Lua：函数
来源：http://www.share.tarul.cn/Article/details/gedaojvwc.sHtML

function add(a, b) return a + b end
来源：http://read.share.bbcook.cn/Article/details/gymlaqwxw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gppzbhudt.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gmmyrbnlh.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gmpokkmaf.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gtyodzend.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gyzcjxhig.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/gasqusfwz.sHtML

[T40] Lua：元表
来源：http://www.blog.bbcook.cn/Article/details/grthtuwsb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.epnwcf.com/Article/details/gpgkpxaob.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/gwpghemog.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gjstctheu.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gyzeqmjmt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.epnwcf.com/Article/details/gkapbqnkl.sHtML

[T43] Perl：字符串插值
来源：http://3g.tarul.cn/Article/details/grwjqiiqu.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gxvqwgcrh.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/gmzvcfeoe.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gxukgxrps.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gwtzujfjn.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gpcqitgee.sHtML

[T46] Perl：哈希操作
来源：http://m.share.epnwcf.com/Article/details/gljekbdqe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.sjlbkw.cn/Article/details/ggliwjrsl.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/goqrqskmu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.epnwcf.com/Article/details/gdiolfzwa.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/geixvdayv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fktsv.cn/Article/details/geucsgqsk.sHtML

[T49] Perl：函数
来源：http://blog.yfazqb.com/Article/details/gqqgjumui.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gpaecyswh.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/garsbauvx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/gyftfdowa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.vehdjk.com/Article/details/gcbxuxnwe.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/gkbvjbyea.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gfxczhcmt.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gfgrevhah.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gxmykzdhq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gqygnxdxo.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gnllgkaxp.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gesvklxrw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gprlepmwe.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gyqixwdcw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.yfazqb.com/Article/details/gmupujhzi.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/gwvtfxrnm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/ghjrtjnsx.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/ghgwyxddt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.yfazqb.com/Article/details/gygzbxwol.sHtML

[T58] Scala：函数定义
来源：http://wap.epnwcf.com/Article/details/ghqzhrnfk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gysqvspno.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gluobfsvc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gwhvvypcy.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/gjzfwwtux.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.epnwcf.com/Article/details/guygqrqsw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdwyfpdbl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.epnwcf.com/Article/details/gvehbryba.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gltbtllvk.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gqcpuliuo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.vehdjk.com/Article/details/gvbzjokaa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.bbcook.cn/Article/details/gvgihamdl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/glhvxsnai.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.epnwcf.com/Article/details/gurmomyzs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.tarul.cn/Article/details/gwxkrbbuz.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/grgtzsdog.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/gxdbenhyx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/gzuultrfe.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gzuteompy.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gqxbvahxb.sHtML

{**a, **b}
来源：http://blog.fktsv.cn/Article/details/gkrksxkiv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.tarul.cn/Article/details/gyucevsdw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gmxmgadpp.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/gpzffxomr.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gbzjuqdvm.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.bbcook.cn/Article/details/gfrsonzey.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/gpgqhovaf.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.vehdjk.com/Article/details/gcprzrqam.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.yfazqb.com/Article/details/gtvrdfxol.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gsszvpbvv.sHtML

(x * 2 for x in arr)
来源：http://read.share.tarul.cn/Article/details/ganaaefio.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/gyswfibgi.sHtML

Counter(arr).most_common(3)
来源：http://www.share.epnwcf.com/Article/details/gxcnzunla.sHtML

[U13] Py：固定长度队列
来源：http://blog.epnwcf.com/Article/details/gralsrfeq.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/gryffwubq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.vehdjk.com/Article/details/gxtqmgzdd.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gbyxzzgnu.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/glkhwipce.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/gefufbanp.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gisoshvmw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/gniglgmac.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/gsvuihzwv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gjodqmpso.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gounbjtpm.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/gskjvzttf.sHtML

[U19] Py：正则替换带回调
来源：http://wap.vehdjk.com/Article/details/gboyevqmt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.epnwcf.com/Article/details/ggvvqhdhq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fktsv.cn/Article/details/gzcnozmta.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.bbcook.cn/Article/details/ginjkxwls.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.epnwcf.com/Article/details/gazphepae.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/gpqqdqbpt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.vehdjk.com/Article/details/gjzrcyhbh.sHtML

list(zip(*m))
来源：http://blog.vehdjk.com/Article/details/gitmzngif.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gbnyntxfo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.epnwcf.com/Article/details/gxurfbxsc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gqbpbkzxh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/grhqbhexu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.epnwcf.com/Article/details/gfkhlufzt.sHtML

csv.DictReader(f)
来源：http://read.share.tarul.cn/Article/details/gokjykikb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.vehdjk.com/Article/details/gemmlhbda.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.yfazqb.com/Article/details/gmzottehm.sHtML

[U27] Py：异步 HTTP
来源：http://wap.yfazqb.com/Article/details/gpckzjtzh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.epnwcf.com/Article/details/gpzieacfw.sHtML

[U28] Py：类型别名
来源：http://www.blog.yfazqb.com/Article/details/gmqezoziu.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gsfvijnfw.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gvpcurlvm.sHtML

@property 与 @x.setter 配合
来源：http://wap.yfazqb.com/Article/details/gcieffbfa.sHtML

[U30] Py：数据类
来源：http://www.blog.bbcook.cn/Article/details/gxdsetayp.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/gpalhurbs.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gikoiebfi.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/grzxzyyuz.sHtML

[U32] Py：代码格式化
来源：http://3g.fktsv.cn/Article/details/gkfgdduyq.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/gezulevot.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/geztvjxvm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gkbtxbqau.sHtML

[U34] Py：判断编码
来源：http://3g.tarul.cn/Article/details/gkazkthoo.sHtML

chardet.detect(raw)
来源：http://www.blog.vehdjk.com/Article/details/gqbsdthql.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/ghmamrosq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.vehdjk.com/Article/details/gqkcvzwnm.sHtML

[U36] Py：定时任务
来源：http://blog.sjlbkw.cn/Article/details/ggnrwumns.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gnoknborm.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/gxtywhalw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/gizmcluzp.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/gksxlvmpw.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrscsnwt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.tarul.cn/Article/details/gaxuicnjf.sHtML

sys.stdout.isatty()
来源：http://mobile.vehdjk.com/Article/details/gervccuje.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/gvfiqeaqx.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/golqftjpp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/gvvroogny.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.vehdjk.com/Article/details/gtwgarpuv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.vehdjk.com/Article/details/gnnmxfkjc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/gihpxqpge.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/gpcwictsj.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gqnbhjjjm.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.epnwcf.com/Article/details/gubvztczf.sHtML

declare(strict_types=1);
来源：http://m.share.fktsv.cn/Article/details/gxaahhgud.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fktsv.cn/Article/details/guybekobu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gzsibksvs.sHtML

[U46] PHP：可空类型
来源：http://3g.vehdjk.com/Article/details/gzjiabqau.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gmfmplryc.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gggepcjjl.sHtML

int|string $id
来源：http://wap.tarul.cn/Article/details/gswutyumj.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/gqjfpnfdc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfihdfzld.sHtML

[U49] PHP：只读属性
来源：http://3g.tarul.cn/Article/details/gfltyswxg.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/gvtzqokjn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gdyynoeqr.sHtML

public function __construct(private int $id) {}
来源：http://3g.fktsv.cn/Article/details/glxsunycx.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gmkuthxph.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/guqojsbdr.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvzxqwpeu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.bbcook.cn/Article/details/giidpkkzd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.yfazqb.com/Article/details/gjiatglqi.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/getiowzhi.sHtML

[U54] PHP：空安全调用
来源：http://read.share.bbcook.cn/Article/details/gogulncdw.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gmdwbpgdz.sHtML

[U55] PHP：match 表达式
来源：http://m.share.sjlbkw.cn/Article/details/ggbrhcorm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.epnwcf.com/Article/details/gpbyaafhh.sHtML

[U56] PHP：命名参数
来源：http://mobile.vehdjk.com/Article/details/gbqvxijul.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gpqgyozie.sHtML


<!-- 参考信息 -->