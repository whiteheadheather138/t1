代发 wailian999

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gaqwcztyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gfujccezl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gltcnontm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/goxibreix.sHtML

[S37] C++：set
来源：http://www.m.share.epnwcf.com/Article/details/gvoqllruk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/gvuvvzuul.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/gdswtlkcp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/giuntthdt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gwdqboywe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.tarul.cn/Article/details/gjzgvpjra.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/ggmbfeoxo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gsiwgvawc.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/gjnrhifod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gaqmeirhq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gcrpwxkcs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gkxcyrpje.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gbnaqsnlh.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gnlczymdc.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gkccyhxoh.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/gqgjmyeno.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gdtpjwnek.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.vehdjk.com/Article/details/gqvhgrpks.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gwsnpmnyv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gpcfbxtoq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/grwugdfcy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gwzbqdroq.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gqklbxafc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gdwhflpbf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/geyequxqt.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gjxzajpsd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gcwyckkkm.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gcfzdcjsi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gegdkhdjs.sHtML

[S51] C++：显式类型转换
来源：http://www.share.tarul.cn/Article/details/gouwpbpvo.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/glsvybunq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gcnciasuf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.tarul.cn/Article/details/gsdtwkcov.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gicxlvqtk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/getjwluav.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gztqsetqc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.epnwcf.com/Article/details/gjzylhrez.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/guejdazzv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/goihdisvg.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/grvyqsjac.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.yfazqb.com/Article/details/gunqipgsv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gdchjqlos.sHtML

constexpr int N = 10;
来源：http://3g.yfazqb.com/Article/details/gopyawtqa.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gmoxpvofr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gwonjptuq.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gjtrxzddo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.tarul.cn/Article/details/gujuayanw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gffyajzih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gyksdxwzr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ginoiwgtx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gaixwhkjv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcrpxrhna.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/ggaqjmbap.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gvfuhaecc.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/galpfkyvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/ggvkgnjim.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gffkljdcy.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gpqplaiwk.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/griblprsu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fktsv.cn/Article/details/gkwselbcy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gzdiskcsi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.yfazqb.com/Article/details/gvbufwtwk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gycjrpzoc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gcnlbpqui.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/ghhlclzuu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gkgvyysas.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/glgrsqcji.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gfqkjxyrf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gwggcssip.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/ghzcawlsp.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gennfterr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gxcdapdft.sHtML

[T11] Kotlin：协程
来源：http://mobile.vehdjk.com/Article/details/gbtabmxeg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gipqmvuaw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/gmcdrrqlb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gbcbrnuog.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gakdyfiad.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gdisojyln.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/glreersry.sHtML

for (i in 1..10) println(i)
来源：http://baike.fktsv.cn/Article/details/gfbnqoktg.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/gzdqneswz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.vehdjk.com/Article/details/gcwexiuzm.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gelsorsfa.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gtqpblmjk.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gvqppfvbh.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gsxbbahlz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gyaoywtsm.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gmjfhgtyn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gcczvyusw.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/ggutshzdv.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/grrhzjayt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gslbekfmn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.vehdjk.com/Article/details/glyakowcc.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gqfwpjwag.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gxmikquek.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gnzmgovgx.sHtML

[T23] Swift：函数
来源：http://read.share.tarul.cn/Article/details/goliniwmb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/gupcchmhv.sHtML

[T24] Swift：闭包
来源：http://read.share.sjlbkw.cn/Article/details/gehsjmiod.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/greuvhplw.sHtML

[T25] Swift：结构体
来源：http://baike.sjlbkw.cn/Article/details/gbqgmfwqt.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gvxafolrm.sHtML

[T26] Swift：类与重写
来源：http://wap.sjlbkw.cn/Article/details/gfwrcwcnt.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/gpdwptrkf.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/glmrmkalv.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gcejgbvcv.sHtML

[T28] Swift：枚举
来源：http://blog.yfazqb.com/Article/details/ghbstqltj.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gypocdevd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gzptevskj.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/gbbgluqnk.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/ghybpzcej.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gksibbasi.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/giavkeply.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gbnjzpjmx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.vehdjk.com/Article/details/gppizfwrw.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gzbtvnsap.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/gplsikxza.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/glfbptrrd.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gfydxuezb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gpgtoxsae.sHtML

[T35] Lua：字典表
来源：http://read.share.vehdjk.com/Article/details/gfokqkhai.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.vehdjk.com/Article/details/gdtunehoa.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/gspxblmzs.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gsrxdwjlw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gapfqibpx.sHtML

"a" .. "b"
来源：http://wap.vehdjk.com/Article/details/gviwewxwc.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gbjgfirxs.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/gdkimksyu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gucmxaovx.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gapkklkqj.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gfbqnrrvz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.tarul.cn/Article/details/gdhxnjhsu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gwblfqsrl.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/gyhdaryzy.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/girwesvyw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gmizmahex.sHtML

[T43] Perl：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gqsstwgpb.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/gfhgemjrh.sHtML

[T44] Perl：条件
来源：http://wap.bbcook.cn/Article/details/gicrbpmeo.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.epnwcf.com/Article/details/gfgshyelm.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gubvtwsfz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvvtwejvf.sHtML

[T46] Perl：哈希操作
来源：http://wap.fktsv.cn/Article/details/giijfhwwu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/grpcalfmx.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/gsmvpdosa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gilfudiid.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/gszrbzees.sHtML

$s =~ s/old/new/g;
来源：http://3g.epnwcf.com/Article/details/gsoyqommm.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gjfntvjpm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/glqrlhztj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gqlpumwvf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/gsrnxciqt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gujhyxbcc.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gxitqlsbr.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/guulkvogq.sHtML

[T52] Scala：变量
来源：http://baike.tarul.cn/Article/details/gbbgtivbi.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/guqqdvkay.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gdyqmcnwy.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/gfcddbxch.sHtML

[T54] Scala：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gcrdetqdn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/gsijglvfd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gyzhmjneh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.yfazqb.com/Article/details/gyqmbznug.sHtML

[T56] Scala：样例类
来源：http://www.m.share.sjlbkw.cn/Article/details/gszsqkhub.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gpappgkbh.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gihdwrwfq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gmtmnlmwy.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gctwgdtyf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/grglfthxe.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/gwkwchwxm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gnlarisak.sHtML

[T60] Scala：折叠
来源：http://www.blog.vehdjk.com/Article/details/gpmnhhoxz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.yfazqb.com/Article/details/gyewxrdrd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gsbeqbevz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gefkmjmkb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzohvsodz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/ggijzvmzz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/ghduzbecg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/ggomclggv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/gpujpdkel.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/gxbmqhxtg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gusdoqjwf.sHtML

[U04] Py：变量调试打印
来源：http://mobile.tarul.cn/Article/details/gchfrmnfz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fktsv.cn/Article/details/gbnezkkyi.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/gmgzuafxs.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlmizidn.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/giwcldqhw.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gtgzcrtvm.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/gcaldfrvy.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gvotfogtn.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/ggswvqmpp.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/grfrbpeor.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.yfazqb.com/Article/details/gdvpvuboh.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/ggtnbuxrm.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/gkqsglicx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/glviqzuqo.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gizapmgpt.sHtML

(x * 2 for x in arr)
来源：http://www.share.vehdjk.com/Article/details/gdfdlprkf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.yfazqb.com/Article/details/gdytcosza.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/ghnnzkosn.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gnlwlwiqa.sHtML

deque(maxlen=10)
来源：http://3g.vehdjk.com/Article/details/gpvrpbcff.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/gztpkbqqp.sHtML

defaultdict(list)
来源：http://m.share.fktsv.cn/Article/details/gomsnscua.sHtML

[U15] Py：高精度计时
来源：http://www.blog.tarul.cn/Article/details/grzvfaxol.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gdtlxqwsl.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/giypsplua.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhqfnmcd.sHtML

[U17] Py：初始化日志
来源：http://www.share.epnwcf.com/Article/details/glgtcnpny.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.tarul.cn/Article/details/gulxsorhb.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gacmcfrym.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.vehdjk.com/Article/details/gfultysyb.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/gqxycoalo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gfftxwucq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/gfciaowoc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gxzptrgsc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.epnwcf.com/Article/details/gkgyazkmi.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gwbskjpyy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/guqqytver.sHtML

list(zip(*m))
来源：http://m.share.bbcook.cn/Article/details/gywpjrwxb.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gijiellom.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.tarul.cn/Article/details/gmryuqlko.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gzxzojgoe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gciobzglj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.epnwcf.com/Article/details/gazbyqbmi.sHtML

csv.DictReader(f)
来源：http://mobile.fktsv.cn/Article/details/gxuwqjetq.sHtML

[U26] Py：并发下载
来源：http://read.share.fktsv.cn/Article/details/grjnlaeeq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/grgovdrbs.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.sjlbkw.cn/Article/details/gmbqmtgvq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/gouwnamxy.sHtML

[U28] Py：类型别名
来源：http://wap.tarul.cn/Article/details/gfcymavlf.sHtML

UserId = int
来源：http://www.share.tarul.cn/Article/details/gfcwakcbf.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/ggipjaico.sHtML

@property 与 @x.setter 配合
来源：http://www.share.sjlbkw.cn/Article/details/gdicyxzdx.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gzcruwzdu.sHtML

@dataclass(slots=True)
来源：http://read.share.fktsv.cn/Article/details/gzthchtgg.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/gabbzeaxy.sHtML

python -m pytest -q
来源：http://read.share.sjlbkw.cn/Article/details/gecqtqhsm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gzunbzjxr.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gemdavdhz.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/guynvoepn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.yfazqb.com/Article/details/gddxtyrho.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/gbbepfhck.sHtML

chardet.detect(raw)
来源：http://mobile.fktsv.cn/Article/details/glzmxdlpb.sHtML

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/gualqmryw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/gxrdnzwhc.sHtML

[U36] Py：定时任务
来源：http://read.share.epnwcf.com/Article/details/gxvejnfhg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.bbcook.cn/Article/details/gzhfvgmir.sHtML

[U37] Py：读写 Excel
来源：http://read.share.tarul.cn/Article/details/gtccdzyhc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.vehdjk.com/Article/details/gpahlgndg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/galkapjky.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gwphydcpr.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gvqyuapyv.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gootlxzlq.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gysjdrust.sHtML

print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gkbvgchzk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fktsv.cn/Article/details/gzsxfliky.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gbuucywmx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/ggikmcdqt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.tarul.cn/Article/details/gsiluonca.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gjstcuvpx.sHtML

namespace App\Http;
来源：http://www.share.fktsv.cn/Article/details/ggnrdcwtl.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gtwhcudme.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/gptyulsdx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.vehdjk.com/Article/details/gstqozwpw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gbdeegctc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/giicdplny.sHtML

?string $name = null
来源：http://mobile.yfazqb.com/Article/details/getxpeznh.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/geqprkiar.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gaamppcvc.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gmblxfguq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.tarul.cn/Article/details/gyozqtlax.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.tarul.cn/Article/details/gkzlwzxcz.sHtML

public readonly string $name
来源：http://m.share.sjlbkw.cn/Article/details/gerdvgtdf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/gmiexrihk.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/gtgzbwpsd.sHtML

[U51] PHP：数组解构
来源：http://www.share.bbcook.cn/Article/details/ghhmhlmem.sHtML

[$a, $b] = $arr;
来源：http://baike.vehdjk.com/Article/details/gydqspvou.sHtML

[U52] PHP：箭头函数
来源：http://mobile.tarul.cn/Article/details/gjabevwyd.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.bbcook.cn/Article/details/gzhuedllc.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.vehdjk.com/Article/details/gjakbirot.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.epnwcf.com/Article/details/gqebaniwk.sHtML

[U54] PHP：空安全调用
来源：http://3g.bbcook.cn/Article/details/gtzptxpnd.sHtML

$obj?->method()
来源：http://www.share.epnwcf.com/Article/details/gwguoefrn.sHtML

[U55] PHP：match 表达式
来源：http://baike.epnwcf.com/Article/details/gmxqbcxob.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gtadylcea.sHtML

[U56] PHP：命名参数
来源：http://wap.bbcook.cn/Article/details/ggexddmje.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/geowzyoju.sHtML

[U57] PHP：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gqplonwhr.sHtML

"值: {$a}"
来源：http://baike.epnwcf.com/Article/details/gicatsuxm.sHtML

[U58] PHP：数组三件套
来源：http://3g.epnwcf.com/Article/details/gnrlfmvcq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/gxxuzobel.sHtML

[U59] PHP：自定义排序
来源：http://blog.sjlbkw.cn/Article/details/gjsghahep.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gljcddzjc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gxsamgjuq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.vehdjk.com/Article/details/gywewaety.sHtML


<!-- 参考信息 -->