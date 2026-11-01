代发 wailian999

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gbhhrbrkk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/gjxismops.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gehibzqew.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.sjlbkw.cn/Article/details/giwgloskb.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/guvhwvehv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gprakbqts.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gzlmimysu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gwpieogpl.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gvtferpsu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gqcbtzocr.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gxufedcta.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gzghxtsql.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gxzkiuzdq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gjuyvwdux.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gooikvaxj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gnblomqda.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gextwfbxh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/gdwcmuczs.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gbhguayyl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/grugactwn.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/gtkzcsgwd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.tarul.cn/Article/details/ghzmbirru.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gyfwptvvy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gghgpkjfw.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/gqikaawrm.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/goobcuust.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gknisnrzp.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.vehdjk.com/Article/details/gfuvvpuax.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/gqryyputi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gywuypnen.sHtML

[S46] C++：函数模板
来源：http://3g.yfazqb.com/Article/details/gsevyexrj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gacmcqthm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gyivwebia.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gzgrmikqc.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gnnbzrmzp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/gztojaogt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gwvkpcruh.sHtML

[S49] C++：写文件
来源：http://wap.epnwcf.com/Article/details/gwbxfohmf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gxywowpwi.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gqnfcdlkh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gzipkedso.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gfhcefbmm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gqkhoklxk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/ggsyrnids.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/giumkxxnh.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gmjkuhajs.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gqcvlhrvk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/gbouogfhx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gvgfbijvn.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gtwpimvwk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/glnqbtfad.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/gjfqdeybo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/gwcxdpapp.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gqcwavfnd.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gxjfadrly.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/ginfpciff.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.vehdjk.com/Article/details/geejbvyse.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gkwohgpzt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/geysmekdi.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gksrgfhvg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/guorxiwbn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gblccfmnb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gyyeybwnm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkttcurca.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gqgoochup.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gcborqofx.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/gpbukvkud.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gdaibuyli.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gszuumtbd.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/glimpcowl.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gfwbgpjzd.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/gcclfjrnd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gklfhytgk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gprqqlyop.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gpfrgltbr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gofulfkiu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/geavoyfek.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.vehdjk.com/Article/details/glzjhfonl.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gjlamduav.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gmigruwbp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gcpuszwwc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.tarul.cn/Article/details/giaxpwylc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gulxbqwpq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/gtzsxdgjj.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/goyghjbuy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gtwpmgurb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gmoykiuks.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gozneamum.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/ghpmkztka.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyzkbrixq.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gnudtpfuv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/geenxqfpw.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gbvpmgvwy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gcaspueat.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gcawrdqtd.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gnfqsflip.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gjjwfnvud.sHtML

var a = 1;  let b = 2
来源：http://blog.epnwcf.com/Article/details/gvsjhtvwy.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gwzaiskne.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gzjzhyhve.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gmgszeogk.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/gozajtmcu.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/geobdxxid.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gnolvdvkj.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gqbaxtvir.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gvcjfhzav.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/ghjkpxnuu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gkxlvrkxg.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/gynxhwgvp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gflzupozw.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gsrjoescl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gvzxpyyks.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/gzghbnuzk.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gevuwwsmq.sHtML

[T26] Swift：类与重写
来源：http://m.share.fktsv.cn/Article/details/gcyoeojqg.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/gnetjhyms.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gvzftqsep.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gshgwmrho.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/gwtsdjuyv.sHtML

enum Color { case red, green }
来源：http://mobile.bbcook.cn/Article/details/gklfvisny.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/gwsmgnjpc.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gxzucmvfg.sHtML

[T30] Swift：协议
来源：http://baike.bbcook.cn/Article/details/gnrequnub.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/giaonycnf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gxqufgwdj.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gwfoftyfz.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/gbyjctrra.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gieltqkkq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gahgczcuf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.sjlbkw.cn/Article/details/gbkpkiyfz.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gkhmkofeq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/ghndwpndn.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/giwunlhrp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/gajialhtt.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/ghmcfqjdu.sHtML

function add(a, b) return a + b end
来源：http://www.share.tarul.cn/Article/details/gbggvbrew.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/gutjchvef.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gbcqcucex.sHtML

[T38] Lua：条件
来源：http://www.share.sjlbkw.cn/Article/details/gkkkovuql.sHtML

if x > 0 then print("正") end
来源：http://3g.yfazqb.com/Article/details/gevtzgeaj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gqlgsyvwb.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gweisvzuw.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gzdttpvrl.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/gufifgxen.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gfvjtiyfz.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gvjuzxokk.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gapwswakh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/gffrfljqd.sHtML

[T43] Perl：字符串插值
来源：http://3g.yfazqb.com/Article/details/gqtjnckik.sHtML

"值: $a"
来源：http://3g.vehdjk.com/Article/details/gdzzvgkbv.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gqmucedgn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gltadoges.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fktsv.cn/Article/details/gslgninau.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjuzdstlg.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gbfxafqbm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gavgwinby.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gjchbozcd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/gqxjdwxga.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gynuibnzq.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gxjqhljtx.sHtML

[T49] Perl：函数
来源：http://read.share.epnwcf.com/Article/details/glplmmmaa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/goufhdamq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gfnftanll.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gjvxfzbri.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gfbavgooq.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/gbpsaipvd.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gclzkrxwx.sHtML

[T52] Scala：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gphrnolst.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/gnmnrrflq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gkrmlzvwo.sHtML

s"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gqewfnenm.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gmprydhrh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.tarul.cn/Article/details/gngeqqncp.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/gxamlinty.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gmcbxbrkm.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/gjeyrqhml.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gqdwxaaov.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/ghgelkocc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/gfcylnouo.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/gmwzsevqf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gvnexzynb.sHtML

[T59] Scala：循环
来源：http://www.blog.vehdjk.com/Article/details/gryejihqr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gbdlfplew.sHtML

[T60] Scala：折叠
来源：http://www.m.share.yfazqb.com/Article/details/gmuzyslrp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/gjtosdzfn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpaeqvria.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gkspkaohz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdevzlhwn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gwaojcdlc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/gtmdnhpjw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/ggjgnbrhp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fktsv.cn/Article/details/gybjwwmko.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gotccveqc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gkmjzflzm.sHtML

[U04] Py：变量调试打印
来源：http://wap.epnwcf.com/Article/details/gqdrjbbwj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.sjlbkw.cn/Article/details/grlbghbej.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gnonmafgx.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gdezfltzk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/gfkwjvhzd.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/ghfaocuxk.sHtML

[U07] Py：反转字典键值
来源：http://wap.fktsv.cn/Article/details/gzdbvayqj.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/ghovvciij.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gffialduz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/gmlcdzjxi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/gwykmdgyh.sHtML

max(d, key=d.get)
来源：http://blog.epnwcf.com/Article/details/giuzvugga.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gkfbqvhjx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gpiyagycq.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/gbspxzvwq.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdxvfosvt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/gfxqpatdj.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gmnoimwyy.sHtML

[U13] Py：固定长度队列
来源：http://3g.bbcook.cn/Article/details/gegtfycfl.sHtML

deque(maxlen=10)
来源：http://mobile.epnwcf.com/Article/details/gpwxwwqci.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gxnmokvuz.sHtML

defaultdict(list)
来源：http://mobile.sjlbkw.cn/Article/details/gixnmcxsi.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/ghpfibsgu.sHtML

t = time.perf_counter()
来源：http://read.share.tarul.cn/Article/details/gbbmwgpdu.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.tarul.cn/Article/details/gogsjtkhj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.sjlbkw.cn/Article/details/gkgfhfoiv.sHtML

[U17] Py：初始化日志
来源：http://www.blog.yfazqb.com/Article/details/gpmpopghs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.yfazqb.com/Article/details/gnernnotl.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/gwkcvzjjq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/guhijlkyb.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/glxitozaa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gvyapexxn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/gbnxhvovx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/ggdhxmeja.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fktsv.cn/Article/details/geqtalpwa.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gydugbhtl.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gbepjklab.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/grfhvtidf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gawzvlnis.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gpebmhjyu.sHtML

[U24] Py：路径操作
来源：http://mobile.vehdjk.com/Article/details/gknrwdbhl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/geyumswad.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.vehdjk.com/Article/details/ghtqibmhx.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/ghkcwnign.sHtML

[U26] Py：并发下载
来源：http://read.share.yfazqb.com/Article/details/gignjcwkt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.yfazqb.com/Article/details/gbjdiuieu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gtqmfqnyr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gzzaquctv.sHtML

[U28] Py：类型别名
来源：http://read.share.yfazqb.com/Article/details/gdtrbvjtj.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gnociosqc.sHtML

[U29] Py：属性校验
来源：http://mobile.fktsv.cn/Article/details/gopqymlqa.sHtML

@property 与 @x.setter 配合
来源：http://m.share.epnwcf.com/Article/details/gqvdlkyeo.sHtML

[U30] Py：数据类
来源：http://www.m.share.yfazqb.com/Article/details/guaidultb.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/grxfcmhvp.sHtML

[U31] Py：单测
来源：http://www.share.yfazqb.com/Article/details/gemhqaywd.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/ggzpwdbnn.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gmdxwhiua.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.vehdjk.com/Article/details/gkgeakdsi.sHtML

[U33] Py：打包发布
来源：http://www.blog.epnwcf.com/Article/details/gfsqortcz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/glgdqctcv.sHtML

[U34] Py：判断编码
来源：http://baike.tarul.cn/Article/details/grdseblki.sHtML

chardet.detect(raw)
来源：http://www.m.share.bbcook.cn/Article/details/gqkmwthgf.sHtML

[U35] Py：发送邮件
来源：http://mobile.tarul.cn/Article/details/gdgodemeg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/gsymdcjix.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gobrffrbw.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/guzyimcee.sHtML

[U37] Py：读写 Excel
来源：http://baike.tarul.cn/Article/details/gpbzovxgs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/gjujzpfgc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.bbcook.cn/Article/details/gobbzkkgz.sHtML

Path(__file__).resolve().parent
来源：http://read.share.sjlbkw.cn/Article/details/gqjpbzdeo.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.vehdjk.com/Article/details/gaeuzrzoi.sHtML

sys.stdout.isatty()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmbajfiq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gkxebyfyw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gmfjtntyy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/ggrsgquoo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.epnwcf.com/Article/details/gmvxjvrxp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/gjjurcgak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.epnwcf.com/Article/details/gecnvrmqb.sHtML

[U43] PHP：声明命名空间
来源：http://wap.yfazqb.com/Article/details/gtfydyoei.sHtML

namespace App\Http;
来源：http://mobile.yfazqb.com/Article/details/gixpbsdnv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/gwomyprvw.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/gfyyxcnlu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.tarul.cn/Article/details/gezceyqyz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/ghgnhcvza.sHtML

[U46] PHP：可空类型
来源：http://3g.sjlbkw.cn/Article/details/ghaswffcs.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gjsfwxzso.sHtML

[U47] PHP：联合类型
来源：http://www.share.bbcook.cn/Article/details/gcrcgivwz.sHtML

int|string $id
来源：http://blog.bbcook.cn/Article/details/gjjihhqra.sHtML

[U48] PHP：纯枚举
来源：http://baike.epnwcf.com/Article/details/gjtrertqc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/gjrdvmppe.sHtML

[U49] PHP：只读属性
来源：http://wap.epnwcf.com/Article/details/gbdxcikfd.sHtML

public readonly string $name
来源：http://baike.vehdjk.com/Article/details/gftvqxryi.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.vehdjk.com/Article/details/gtgtoizki.sHtML

public function __construct(private int $id) {}
来源：http://wap.bbcook.cn/Article/details/ggdpfpxnq.sHtML

[U51] PHP：数组解构
来源：http://www.share.sjlbkw.cn/Article/details/gsxjwcxcj.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gextbhruu.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gwttjmrcr.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fktsv.cn/Article/details/gksrwihnu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.vehdjk.com/Article/details/gfmkyerus.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/gyxidiyvz.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gczzpmgwj.sHtML

$obj?->method()
来源：http://read.share.sjlbkw.cn/Article/details/gqrxvkdar.sHtML

[U55] PHP：match 表达式
来源：http://mobile.yfazqb.com/Article/details/gcysjmpag.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.epnwcf.com/Article/details/ghjdbwinp.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gnhlklxhl.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gjisbzomj.sHtML


<!-- 参考信息 -->