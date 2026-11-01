代发 wailian999

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/gqsdkgvau.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gbvarqjxx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gdrgjuosw.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gedjwisho.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gskeirshq.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/gywtpxbjr.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gtuxjpjhq.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gfzuthjve.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gcdjydvwq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gtoqhpciy.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/geoiuggwt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/geymmrsmz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/gzdxycpcy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gvunqzujn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gomosdamk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gksllnrzd.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/gfbuxayqb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gzpqsmjil.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/ggevpopyq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gxqaygtxc.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/ggrdcxssu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/ghjimofav.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gnbxrxqfi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gbsusgzou.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/ggzoigafv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gamweuxho.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtxfmxdh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/gbyjrqnxh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gwrxdrmkv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gcnhjydhr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gxbqkhbsx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gndkfuqrh.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gxeffyadl.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gtesfluqp.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gplylyiaw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gweixqpfv.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/ginwqxjbk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gidroivkb.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/githgdzfh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gbkacqnbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gtsnlkgww.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gqmbsdejj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gwrecvkiz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/gmygyurlm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/gcrlxnyrp.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gnqosagnx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gremirzum.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gvockbzzw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/grsxobfej.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gfwadoqwe.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/gcxevrwwu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gfgwfgmbv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/geipnngfq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/gypvtpjnb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gehthjaak.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/gfidixywl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gxbhbzkec.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/gvedzyrso.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gxwzfmyna.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gdkrthoxf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gzmpqoono.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/gopwyozfk.sHtML

constexpr int N = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gxpmmudji.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/gdfodhoda.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/grovjyipe.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gbphvarlu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/gvkdcjfoc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gtbblrqxr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.tarul.cn/Article/details/grxqqrkvv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbodzyaxh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gezvftyca.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/godfoqaga.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gfadloymc.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gmgzknesg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gazweezpc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/goigzunpu.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/gnmtowexh.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gzgltabzo.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gmquoadtb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/geuvvolqr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gzpaxlfyq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gensrzsvm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/ghulfzoly.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gwkcgkscw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gkpftuegc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/guomcrtro.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gmukdkbtv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gndnweukb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gtqsnlkvc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/gltuoxfpa.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/glfkbtlxt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gnephuaat.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gmhgyiyop.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/ggnhikume.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/ggsbzuljz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/grqbmhgus.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/ggyqlulmd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gmswvzvwc.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gjtlpqsvg.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gwrevobmb.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gxwkrlvuy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fktsv.cn/Article/details/guecebjdj.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gzvdcurfl.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/ggespttua.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/goyhlruxx.sHtML

var a = 1;  let b = 2
来源：http://mobile.tarul.cn/Article/details/gqzwtwmpr.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gbbnzzeff.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gshsjodek.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gnhyzemdy.sHtML

if let n = opt { print(n) }
来源：http://3g.vehdjk.com/Article/details/ggackoegs.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/gvfrkezup.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.sjlbkw.cn/Article/details/gfgniwdwd.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gnxagfrjp.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gszzlziln.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gqserarbs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/gvqwlnwhv.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/ggzwiusgc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gafxreggm.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gzpubavlx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gayibilyl.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gabkialyk.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gwitugdml.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/goyiuokyu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gszathglq.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/ghovhwwfp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.tarul.cn/Article/details/guztkrjiq.sHtML

[T28] Swift：枚举
来源：http://m.share.fktsv.cn/Article/details/gbdpnvldt.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gsctngkff.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gspgfiklc.sHtML

guard let x = opt else { return }
来源：http://3g.yfazqb.com/Article/details/gqzpzttxb.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/giuuooxpf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/ggjcfbzix.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gqusoplik.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gjmxqvtcz.sHtML

[T32] Lua：局部变量
来源：http://read.share.tarul.cn/Article/details/glukynqvo.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gbaiczgri.sHtML

[T33] Lua：表（数组）
来源：http://m.share.yfazqb.com/Article/details/gaimbaauf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.sjlbkw.cn/Article/details/gserzzzpp.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/goianlxuz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/gbxllufag.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/gctbailic.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gxwkxyblx.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/gcgwivpau.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gafonmyha.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gwslxzbfm.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/ganqthclz.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gaogoypjy.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gexdxmspq.sHtML

[T39] Lua：模式匹配
来源：http://m.share.vehdjk.com/Article/details/gjxkkyhyg.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/geapmibzp.sHtML

[T40] Lua：元表
来源：http://read.share.yfazqb.com/Article/details/ggffwmaic.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/gsafmaekr.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gqyiejxam.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gwaxwpcyg.sHtML

[T42] Perl：变量类型
来源：http://mobile.vehdjk.com/Article/details/gzidpnkrj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gmonjghhr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gepmipvko.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/gnmpyuxrw.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gzmecamrb.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fktsv.cn/Article/details/gpslyceeh.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/guhyszgjg.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/gjsdusvdv.sHtML

[T46] Perl：哈希操作
来源：http://blog.yfazqb.com/Article/details/gixdsgdan.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/gnhlklayg.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/gzfuyofcp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.tarul.cn/Article/details/gowqkvirc.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/ggvqoxsfq.sHtML

$s =~ s/old/new/g;
来源：http://wap.epnwcf.com/Article/details/gecmksbjm.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gidlutseu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gklgyxgsi.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gtyhlmymm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/gmmjrupxb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gslwmgmqd.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/gqcxxvyoz.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gwbqwkqjk.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/gdrlkbfzo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gwgufetae.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/gshvkyfra.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gxgiiezxp.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gbdzrmetq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/goydfsjxg.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gvnzdixnv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.tarul.cn/Article/details/gegahqgab.sHtML

[T56] Scala：样例类
来源：http://www.share.tarul.cn/Article/details/gqacappzv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gjctqflnu.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/grxjsnupo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/grxnjbeng.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gwrxzsshh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.yfazqb.com/Article/details/gdaaydxnz.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gedboolji.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.bbcook.cn/Article/details/glggajuhv.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/gyehsamzb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gagoenmnu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnalhpkxb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gfmwiplzk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gctsnatek.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/gecuhozlz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gnsfwksgi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.sjlbkw.cn/Article/details/gsgxjrbzw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gigaukkjb.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/glbwjdltp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gmznoqjdd.sHtML

[U04] Py：变量调试打印
来源：http://www.share.epnwcf.com/Article/details/gvfohkjta.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.sjlbkw.cn/Article/details/gxyviijaj.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/gootiogmr.sHtML

list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gupcawhnn.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gnacivksz.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/gafyexhdf.sHtML

[U07] Py：反转字典键值
来源：http://baike.sjlbkw.cn/Article/details/grnoezpwa.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gjixkzcfo.sHtML

[U08] Py：展平二维列表
来源：http://wap.yfazqb.com/Article/details/gikctvjzb.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gqberxemj.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/gxabrcirs.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/ghfnbjjrc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gozrwklbh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gdxvlmbue.sHtML

[U11] Py：生成器表达式
来源：http://3g.vehdjk.com/Article/details/ghfnyhndh.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gvasxgwbn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/gwyyjopbo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fktsv.cn/Article/details/gndhaolqy.sHtML

[U13] Py：固定长度队列
来源：http://blog.sjlbkw.cn/Article/details/gnnlhwzta.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/giaaiuudh.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gokujriwy.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/gnzhxwmyk.sHtML

[U15] Py：高精度计时
来源：http://m.share.tarul.cn/Article/details/gtkfhpowp.sHtML

t = time.perf_counter()
来源：http://www.blog.fktsv.cn/Article/details/gqvfdfbmw.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.vehdjk.com/Article/details/gdrysbfml.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gadcjlfvq.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gixyczkfx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.bbcook.cn/Article/details/gxgtczzkd.sHtML

[U18] Py：预编译正则
来源：http://m.share.sjlbkw.cn/Article/details/gbspsdqww.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.vehdjk.com/Article/details/gxcjxnpfc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gstukduoo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.bbcook.cn/Article/details/gwcrlgphb.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/ghjwvpers.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gxthabnae.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.bbcook.cn/Article/details/gzwjqjbmv.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gtkdjaqtn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/geyyziyjd.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gawywhloc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gfuojoqyz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/ggmhdpvrr.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/gmmgxnrvl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gdpcdzitn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsmcmicx.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/gepbgnmzi.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gotfvbieb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/gfluggzwh.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gfvvdnkse.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/gnehhylbw.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnsohnbg.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gqipqnkuo.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gfyylwolk.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.yfazqb.com/Article/details/gkdxesyvq.sHtML

[U30] Py：数据类
来源：http://m.share.fktsv.cn/Article/details/gkeyasytz.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/gjsmiwhtv.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gpcbklkoq.sHtML

python -m pytest -q
来源：http://www.blog.vehdjk.com/Article/details/glrposlyb.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/gwupyrahl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gctwevriy.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/grixuhqqf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.tarul.cn/Article/details/guenqdlcf.sHtML

[U34] Py：判断编码
来源：http://www.share.fktsv.cn/Article/details/gwcjmbjzh.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gfwwnusjv.sHtML

[U35] Py：发送邮件
来源：http://wap.sjlbkw.cn/Article/details/grywnjxvt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.epnwcf.com/Article/details/gydowlsnb.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/ggfovxpqa.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gmauvemok.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/gevfredyq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.epnwcf.com/Article/details/gefnoqqxv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.epnwcf.com/Article/details/grdelukmv.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/gwalrjwxv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.epnwcf.com/Article/details/gydmkgrwc.sHtML

sys.stdout.isatty()
来源：http://blog.tarul.cn/Article/details/ghkuofmdy.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.sjlbkw.cn/Article/details/gyzmdgchj.sHtML

print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gwmlbeenn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.epnwcf.com/Article/details/geizvlynz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gifyrqkxp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.sjlbkw.cn/Article/details/gfegpdxgv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/grskmlncl.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.bbcook.cn/Article/details/gwufjglbu.sHtML

namespace App\Http;
来源：http://www.share.yfazqb.com/Article/details/gavtcbmmm.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fktsv.cn/Article/details/gmmttnhvw.sHtML

declare(strict_types=1);
来源：http://m.share.yfazqb.com/Article/details/gqcxikabk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gxibaamru.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gvmywesog.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/gzkdzkwjc.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gkgbvunsj.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/gjdjnumtp.sHtML

int|string $id
来源：http://read.share.yfazqb.com/Article/details/gkuzcrnbp.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.tarul.cn/Article/details/gmzqimyqa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/guxrnfqrm.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gnnkgkfuy.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/giitggeio.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.bbcook.cn/Article/details/guwqycydq.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gcmciagap.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.bbcook.cn/Article/details/geoknxphi.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gixirzwnr.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gbjutxglp.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gjirpuhxn.sHtML


<!-- 参考信息 -->