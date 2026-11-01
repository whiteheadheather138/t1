代发 wailian999

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/ghpfourot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gnrsktupb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gloweqtrr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gdvdjiwjk.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gvrecfnpa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gxsthkuww.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/ggaigiain.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gdpcegqdo.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gbqqxfjcs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gsuqqkiaz.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/gzbflweil.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/giezfbeht.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/giexyyzqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.bbcook.cn/Article/details/gtcqblnxj.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gamjujbnw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gfrlziraa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gbohrgqzr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gvbteaxxw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gubomxcyk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gjtczwtkz.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gjkrlvljj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/geqducvul.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gvmyegwzb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/gulprzzdc.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gmwzengpd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gkueovyvx.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/grubsrlmb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gphxchube.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gznxmdgcj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/gajkhezet.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gcuyvuwgg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gyuaolbmj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.yfazqb.com/Article/details/gmfpovjzx.sHtML

[S49] C++：写文件
来源：http://wap.bbcook.cn/Article/details/gpppglwsj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gibnsmauy.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gkpianldr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gwfvgpuxb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gwoojljjk.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gedvoqbbz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gzioyetlw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gcoporptl.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gqpqznkzs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gaeepmvml.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gpvwrbshv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gnrdhfyok.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/ghqpwsyjd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gsdkcsinw.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gjwwzmlsl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gzfniteji.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gazqkutjy.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gzgdotloe.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gvcpegxfp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/ghoqnqlmd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/gisftikhu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/gdmghixpo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gugktwjzw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/gjlwmbxou.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grxgoxpry.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gfiyyuxnf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gisngzyvm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/gwjdepdgt.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/ghlxiyajk.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gslinpnsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/gxbmikqvo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/giissvhdz.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gqlscwacc.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gbetfvelo.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gixyiunvq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.yfazqb.com/Article/details/gpqxpusgd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/gzyjiqadd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gxlxdrtzc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgigxxlo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gpddwbnuv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gellboruj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/gnpkwswvw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gkapucado.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fktsv.cn/Article/details/giqpovskf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkejputkr.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/gcvaaddhd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gmvnraauh.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gitruglwb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gfjddglxx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/givlidzaq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gsoxskwxr.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/glnnyelhd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gxbkavsqu.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gijvjfczr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/geqostkqj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.sjlbkw.cn/Article/details/gqamnbkag.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gljzbjlat.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gwxmhevoh.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gbvfxfbqa.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/gicxyccbl.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gbkcucnax.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gkqtzzpps.sHtML

"值: \(b)"
来源：http://www.m.share.bbcook.cn/Article/details/gwmplhgwq.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gqjgzowox.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gzotfhalu.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gpoezvuiy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gybxkmige.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gqqxvwdka.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gehgzaisy.sHtML

[T22] Swift：字典
来源：http://www.share.tarul.cn/Article/details/goccugtvg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/guuzngjmg.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gjyqidkfi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/gulmqemmr.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/gqkxcjrco.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gmdtctwzn.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/guaplqoua.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/gvjnrwpfa.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gtdwcvihv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/ggjhvyoxv.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gxnaltyhe.sHtML

do { try f() } catch { print(error) }
来源：http://wap.epnwcf.com/Article/details/gdylrokyy.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gmqptoqhz.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/ghjxaxltp.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gezrvhgqk.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/grufubrfj.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gjcvbdwcv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gcpmyvtns.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/gcyztgtwm.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gbczxoefq.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gldneyzty.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/ggjtvahjx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.bbcook.cn/Article/details/gjarwgdtr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/grehxywus.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gchjzhrtb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/gahhqcgsy.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gdilbvybt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.epnwcf.com/Article/details/gmtomiers.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gbjvgzojg.sHtML

function add(a, b) return a + b end
来源：http://read.share.epnwcf.com/Article/details/gsrzjhcxo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.bbcook.cn/Article/details/gafwsigok.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gtexfllgj.sHtML

[T38] Lua：条件
来源：http://wap.epnwcf.com/Article/details/gfydysgbv.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gsaumexzh.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvwhmhsv.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gvhvfpdln.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gxzeordgs.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/grlozcedk.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/gtgsutopw.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gqgtvrjge.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gcksjhsbx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gfevbzysp.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/galohegwv.sHtML

"值: $a"
来源：http://www.share.fktsv.cn/Article/details/gedqyxcpm.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gpelfplpw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/grklmawcd.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fktsv.cn/Article/details/gscmjkduk.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.epnwcf.com/Article/details/goptjacfv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gzjyzomzh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.yfazqb.com/Article/details/gmxafrxtu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gtlkyrwqv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/ggsxfdvlu.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/gghjgsoum.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gczohjlnu.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gjtxmnvro.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gjaruccvn.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gwzllgsdk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.tarul.cn/Article/details/ghuwugugq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gvtsgduez.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/ggyavakve.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gnbkjbpxz.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/gwweyyida.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gtihhilva.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gteyyfixi.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/giztdlltn.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/grbesevzy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.vehdjk.com/Article/details/gpczuzrkz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gdmdxtbjk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/gslvnsugj.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/gfbngqhhx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gdczdetqv.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gtfdrctjg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/gzszdfrjc.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/giripxejg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.epnwcf.com/Article/details/gsiosfrjv.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gukynsspc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gcfxpqxtc.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/gmfqojlnr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/gbjlcxtrc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsumdjlkw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/grbeguvwg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gntfxpcyc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gweuswaej.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gtczwcvlb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/ghvbyqahc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fktsv.cn/Article/details/guulzadbl.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.epnwcf.com/Article/details/gfjypvgzb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fktsv.cn/Article/details/gkskzesey.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gxphrsgmf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/gcokshakh.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gvuzeptvz.sHtML

list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/grdpkodhf.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/gnelsaiii.sHtML

{**a, **b}
来源：http://www.blog.fktsv.cn/Article/details/ghxmhhkxy.sHtML

[U07] Py：反转字典键值
来源：http://baike.sjlbkw.cn/Article/details/gbacrgchk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gjkhanrla.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gaesnyblh.sHtML

[y for x in nested for y in x]
来源：http://mobile.vehdjk.com/Article/details/gtiaifvko.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.yfazqb.com/Article/details/gfxkxhoyf.sHtML

max(d, key=d.get)
来源：http://www.share.sjlbkw.cn/Article/details/gpakbeeyo.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gytnowkpv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gzbskwiqy.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gbsikcjtl.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gjnokxokm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/ghpiaokyn.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gdfgwghis.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gioeghzki.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/grapqtbit.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fktsv.cn/Article/details/ghwrgfwse.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gkhomctpj.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/gmyklwqja.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/gahrpcxoj.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fktsv.cn/Article/details/gyeogbkqd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/gamyidiqv.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gbycwaqfe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.yfazqb.com/Article/details/ggqfygxxm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/grjjftrrq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.yfazqb.com/Article/details/gkqhvpnii.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.vehdjk.com/Article/details/gwsfskgix.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fktsv.cn/Article/details/gftxlzlix.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gkbyvghbk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gpyztnlbi.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.epnwcf.com/Article/details/gveepimtz.sHtML

@contextlib.contextmanager
来源：http://www.share.yfazqb.com/Article/details/gqqmsroxa.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gslfnvyxg.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gfcbxnpdp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.bbcook.cn/Article/details/gntqowxxn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.vehdjk.com/Article/details/gveqsxkxi.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gokxazcrk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gxbafqmsz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpdyyuki.sHtML

csv.DictReader(f)
来源：http://www.blog.vehdjk.com/Article/details/gooxwdanm.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gidmcteyt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/guamdrzzp.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gobrdhnxz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.yfazqb.com/Article/details/gqnooyszu.sHtML

[U28] Py：类型别名
来源：http://www.blog.yfazqb.com/Article/details/gofydrgiu.sHtML

UserId = int
来源：http://read.share.bbcook.cn/Article/details/gfgfbyakq.sHtML

[U29] Py：属性校验
来源：http://wap.sjlbkw.cn/Article/details/gcxmyqvbk.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gvqbmngtn.sHtML

[U30] Py：数据类
来源：http://baike.epnwcf.com/Article/details/gdaujebig.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/gpthdtewy.sHtML

[U31] Py：单测
来源：http://mobile.sjlbkw.cn/Article/details/gfpejicdz.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gilcxdxuk.sHtML

[U32] Py：代码格式化
来源：http://m.share.vehdjk.com/Article/details/gbpnbtslt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.bbcook.cn/Article/details/gfcrzpjjs.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gcpeyzeyd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.bbcook.cn/Article/details/gxjgozldj.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/gxrhpptsk.sHtML

chardet.detect(raw)
来源：http://www.share.fktsv.cn/Article/details/gqvipcifa.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/guuoxlepg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.yfazqb.com/Article/details/graegjmmw.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gabpuwfrd.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/gqzhhmscs.sHtML

[U37] Py：读写 Excel
来源：http://baike.yfazqb.com/Article/details/gezjifjkj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/ghxwkdege.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/gsceednhy.sHtML

Path(__file__).resolve().parent
来源：http://blog.fktsv.cn/Article/details/geflknggl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.yfazqb.com/Article/details/gqeihfmhk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gsooflwld.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.yfazqb.com/Article/details/glmjfbgvy.sHtML

print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/glyjsukyt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/ggdihrjso.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.tarul.cn/Article/details/glpopdfmv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/grqolzkuo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fktsv.cn/Article/details/gfmaozpja.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fktsv.cn/Article/details/gqkuvtrqs.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gdemjphup.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.vehdjk.com/Article/details/ggqsjpett.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gmsrhazsz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.sjlbkw.cn/Article/details/gwahvifck.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gajtghlbt.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/gapavlodk.sHtML

?string $name = null
来源：http://blog.bbcook.cn/Article/details/gjkelapvr.sHtML

[U47] PHP：联合类型
来源：http://blog.epnwcf.com/Article/details/gqupcdnyl.sHtML

int|string $id
来源：http://www.blog.epnwcf.com/Article/details/gmriltxfy.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fktsv.cn/Article/details/gdetgiqkn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/gsbyrkkqf.sHtML

[U49] PHP：只读属性
来源：http://wap.epnwcf.com/Article/details/gwmbtrnta.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/gchxwqhkx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/gmfuftmov.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ginvcfxqt.sHtML

[U51] PHP：数组解构
来源：http://www.blog.vehdjk.com/Article/details/gnmearjox.sHtML

[$a, $b] = $arr;
来源：http://www.blog.vehdjk.com/Article/details/gsmojnxhr.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.vehdjk.com/Article/details/gxomehuhy.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.epnwcf.com/Article/details/gqntwvjtq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.sjlbkw.cn/Article/details/gidbykbcb.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gqoslcwli.sHtML

[U54] PHP：空安全调用
来源：http://baike.fktsv.cn/Article/details/gnisnqknh.sHtML

$obj?->method()
来源：http://mobile.yfazqb.com/Article/details/gbzlwgutu.sHtML

[U55] PHP：match 表达式
来源：http://3g.vehdjk.com/Article/details/gwvmhrlfw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/gmnnlpybx.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gnmmqbmww.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gzpyfybqh.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gteskjxyg.sHtML

"值: {$a}"
来源：http://blog.sjlbkw.cn/Article/details/gtomojbfm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fktsv.cn/Article/details/gkedebwur.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/gxedlqmod.sHtML


<!-- 参考信息 -->