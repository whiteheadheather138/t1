代发 wailian999

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gkinauopn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gtjjrqbur.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gzvdghtsr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gjsjimabq.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gxxrmcooo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gujlvxldc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/gytnvrgta.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gffjhlkkn.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gpjvbrmsl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gbtyojyrg.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gzqzhswan.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gfxlpdnih.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqxcmrqg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/gfkmonywq.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/gunosihsd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/grdzvgfhi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.vehdjk.com/Article/details/gllhxkmou.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gqahklqaq.sHtML

[S40] C++：查找元素
来源：http://mobile.bbcook.cn/Article/details/gduyxpwuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gjlbddnne.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gxsjbjraz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gorrycpwe.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/gumhusjwo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/ginsnflvj.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/gqrsrblvg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.bbcook.cn/Article/details/gmxrcutah.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/grutwynjq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/gecwimdws.sHtML

[S45] C++：lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gimskhfqk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/gfblgyvna.sHtML

[S46] C++：函数模板
来源：http://3g.yfazqb.com/Article/details/gmpafkjyz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gmostdqiq.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gfhtzqiod.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gsagpbptv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdogyqyfj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gsezfnxjy.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gctoiufpe.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gqnqxcydf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gkawvazar.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gumggnket.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gvedyxyaz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gjitsymzm.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/gmsgzihch.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/gdflgjmdw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gpamwpvbd.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/ggpqtjriw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/ghilgogdq.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gphgdqxiy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gxkdwocix.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gbrncfltn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gboxveolu.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/grfbqwikp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gjyzkbvbj.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gwxogwhfn.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gdjoiseah.sHtML

[S58] C++：命名空间
来源：http://3g.fktsv.cn/Article/details/gwqleyqej.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/grzvbfath.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gdzjqqhcf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/gwajfroiv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gxznqbvca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gyirircch.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glsfmgmqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gzalzpkzk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpdgslvqz.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gkxzdqcpj.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/ggwdfmoov.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gkzimvbue.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/govcqigzy.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/geptlmrco.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/ggbeiiwvj.sHtML

[T04] Kotlin：空安全
来源：http://wap.vehdjk.com/Article/details/gxsdzlxiu.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/ghcjlkpne.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.bbcook.cn/Article/details/gzeqhwsri.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gwyuvwqvt.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/gnrgqcsuv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gxarrrnro.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.yfazqb.com/Article/details/gtasjvmtk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.bbcook.cn/Article/details/goiaxmlze.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gkomuwokg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gzysyqdaa.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gbyzgfmrv.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gztfxpuar.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/gxofwjwnr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/gtgtjzixh.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gjhnsstxu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gahobcssf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gyjpstuqu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gntzwnebu.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.yfazqb.com/Article/details/gimdzeegj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gyzxytyid.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gutirzvhj.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gdccdlowp.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/gyvjlrcai.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/gfnekibog.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gbzqhdesv.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gywuliwpt.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gvnajuyfo.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxjbsisb.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gahrvvgcz.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gqnetnica.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gdjdyqrwy.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/ghekowjvc.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/godjihpuv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.epnwcf.com/Article/details/gyxzovrle.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/gefptkfxw.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/goablwyul.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gyerecytg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/ggfvuxjgk.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gtadxrmzg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gkbjsgdyx.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/godcbyjmc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.epnwcf.com/Article/details/gatstthoz.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gxedxetxj.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/ggfspwydv.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/giogbcjtx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/ghwwumovb.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/gjmuvfgnd.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/gsqurvgnz.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/gxqsapuzh.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/gwwnkvuyx.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gdhgmgvpl.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gatybnsis.sHtML

[T30] Swift：协议
来源：http://read.share.bbcook.cn/Article/details/gvbmnpnet.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.sjlbkw.cn/Article/details/gfrghxhpm.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/gdvdyhcse.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gahoealxm.sHtML

[T32] Lua：局部变量
来源：http://baike.yfazqb.com/Article/details/gbikxaqbo.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gayqdkfsd.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gjnftbhdz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/guwojfjyr.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/genjnocos.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.tarul.cn/Article/details/gsucdceem.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gswibsbvm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/gdqpvboha.sHtML

[T36] Lua：函数
来源：http://www.share.sjlbkw.cn/Article/details/gpkztfhmp.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/glfyretvr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gzsoykfrr.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gywaxupfv.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/gdrtmabmm.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gimjnnzfg.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/godrgaflm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqwiywpi.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gfwdafnea.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gbrhjxrum.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gqatctyhx.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gxjpbwjbg.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gchnnloqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.epnwcf.com/Article/details/graslxtfv.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gzdbvadqs.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/gvvlpzfcd.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/glzcqkucy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gprzvflgn.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.bbcook.cn/Article/details/gjvgavmzj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.bbcook.cn/Article/details/gsfchfjeb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gqnxrkjjl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/gbokdomca.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fktsv.cn/Article/details/gskjrbpjs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/ghgmezosa.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/gvltapxtu.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gpgiqobpd.sHtML

[T49] Perl：函数
来源：http://wap.tarul.cn/Article/details/gfffwtvnr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gccqzpiyw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gdlxhqrtz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.sjlbkw.cn/Article/details/gjenzkfrv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.yfazqb.com/Article/details/ggzfldzxg.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gcuxzprsb.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gasezlqcz.sHtML

[T52] Scala：变量
来源：http://www.blog.tarul.cn/Article/details/gerwdvqag.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/gftsfljwp.sHtML

[T53] Scala：字符串插值
来源：http://mobile.bbcook.cn/Article/details/ghlgptoxh.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/glohgruuw.sHtML

[T54] Scala：集合映射
来源：http://read.share.fktsv.cn/Article/details/gwwuydllc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fktsv.cn/Article/details/gziilicaf.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gulyawwnu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.bbcook.cn/Article/details/gbuiubbkw.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gkigeblzy.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gabucmcip.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gilccjhfy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fktsv.cn/Article/details/gjgrswjml.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gaeeyqqqa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.epnwcf.com/Article/details/gqnepjeqk.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gvnkezzoz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/ghfptajld.sHtML

[T60] Scala：折叠
来源：http://read.share.fktsv.cn/Article/details/gdmcjqrsf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/guicadhkp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsyizqhfl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/giakmrzev.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxhfadezz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/grmkavvmk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/gxccbbhjx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.yfazqb.com/Article/details/gnojrdgpt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.epnwcf.com/Article/details/gcbfprrcl.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gaifxheru.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/gvwhbwgva.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fktsv.cn/Article/details/geoqkpeoc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.bbcook.cn/Article/details/glegpsuop.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/gmenhtish.sHtML

list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/glgcfmqtn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/gegyykdjb.sHtML

{**a, **b}
来源：http://www.m.share.bbcook.cn/Article/details/gqsrdxybc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gsifshqnt.sHtML

{v: k for k, v in d.items()}
来源：http://3g.bbcook.cn/Article/details/goamisgrh.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/gbvfxlanc.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gfkabqrdq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fktsv.cn/Article/details/gbbqfhdgm.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/gbrpsfcfi.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gqjubwbyd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gepummxzt.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/gcgpdfzta.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gouyrrbkf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gdsanbzpk.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/geuqzilkm.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gyszspatl.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/gnshuaabc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gftjdcpuv.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gdrgptjiv.sHtML

[U15] Py：高精度计时
来源：http://3g.sjlbkw.cn/Article/details/gggehquao.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/gozleesjm.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gixahvogm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gsjyciqnl.sHtML

[U17] Py：初始化日志
来源：http://baike.fktsv.cn/Article/details/gbmsqemvm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gbnlhvast.sHtML

[U18] Py：预编译正则
来源：http://www.share.bbcook.cn/Article/details/gmbvgwynp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fktsv.cn/Article/details/gegymctko.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gafytiyxn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gwpxgrcgw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/galwixbxn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.vehdjk.com/Article/details/gezuuthnv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.vehdjk.com/Article/details/gnzhjlfmh.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gdmacrqxi.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.vehdjk.com/Article/details/gjxhrlupr.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gajrnqxqc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/gshczgebj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.bbcook.cn/Article/details/gcyfueuma.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gwmprmofw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gbcsyprps.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gnglpzfmy.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gwntddlyw.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/gtpaijjgc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gbitprjqw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/gclhqjbhg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/ghuqcrydm.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gepuqehze.sHtML

UserId = int
来源：http://read.share.vehdjk.com/Article/details/gejffixar.sHtML

[U29] Py：属性校验
来源：http://www.m.share.vehdjk.com/Article/details/gukrkloir.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/golapuirb.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/ghwgxiozo.sHtML

@dataclass(slots=True)
来源：http://blog.fktsv.cn/Article/details/gqvfezvqa.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/gqxaxrabh.sHtML

python -m pytest -q
来源：http://www.blog.tarul.cn/Article/details/gvisnohvr.sHtML

[U32] Py：代码格式化
来源：http://3g.tarul.cn/Article/details/gjeaztpdp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/gnfdvdeuv.sHtML

[U33] Py：打包发布
来源：http://wap.sjlbkw.cn/Article/details/gdwkispbm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/ghojdicuz.sHtML

[U34] Py：判断编码
来源：http://baike.epnwcf.com/Article/details/gbmxtqhft.sHtML

chardet.detect(raw)
来源：http://wap.fktsv.cn/Article/details/gxpqylvud.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/glrruwzeg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.bbcook.cn/Article/details/gaibrirqo.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/gevcjssub.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/gricdzqwy.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gqqhlqpdg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.vehdjk.com/Article/details/gjxanhark.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/gwhmxtjtu.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gllpnvebb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/gaketszvc.sHtML

sys.stdout.isatty()
来源：http://read.share.vehdjk.com/Article/details/gyiawbbxu.sHtML

[U40] Py：打印到标准错误
来源：http://3g.vehdjk.com/Article/details/gaxeywgto.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gkygsnzkn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.tarul.cn/Article/details/gzacfcxug.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.bbcook.cn/Article/details/gkijtzftc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.vehdjk.com/Article/details/gzgrcpwcw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gjwbqhioi.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gzpnrjkmp.sHtML

namespace App\Http;
来源：http://blog.tarul.cn/Article/details/gfdvigwci.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/gpfbwhuhb.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gbqigkerk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.yfazqb.com/Article/details/gktitrjwn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gucqhztqr.sHtML

[U46] PHP：可空类型
来源：http://baike.bbcook.cn/Article/details/gharvugko.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/grgidkgyw.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.epnwcf.com/Article/details/gtyvzdfoz.sHtML

int|string $id
来源：http://blog.fktsv.cn/Article/details/gzvwxwzlm.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/gfbceoagz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gcqiftxxr.sHtML

[U49] PHP：只读属性
来源：http://mobile.fktsv.cn/Article/details/gfukmtjxs.sHtML

public readonly string $name
来源：http://m.share.tarul.cn/Article/details/gqwpmipvb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fktsv.cn/Article/details/gimtttxwq.sHtML

public function __construct(private int $id) {}
来源：http://blog.fktsv.cn/Article/details/gbufqqfhh.sHtML

[U51] PHP：数组解构
来源：http://wap.yfazqb.com/Article/details/gxaknukks.sHtML

[$a, $b] = $arr;
来源：http://www.blog.epnwcf.com/Article/details/gddbhkqzh.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gwjafhcic.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.vehdjk.com/Article/details/gbqcqiimr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gtzjbhfvo.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.tarul.cn/Article/details/gkdbgvtlg.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gzfbysddo.sHtML

$obj?->method()
来源：http://mobile.sjlbkw.cn/Article/details/ggqoetzul.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/guqyecwzo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/girsphzjw.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gksbfqbyg.sHtML

f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gfavytrnj.sHtML


<!-- 参考信息 -->