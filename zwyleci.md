代发 wailian999

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/gdzsstzam.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.tarul.cn/Article/details/gztgxjnin.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/ggujsqufz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/gngbszzxy.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gpetoxbvu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gbhmbyrnv.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gvjxlkuzf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gvhfyvwfm.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/greyvrktr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gjlcfvmrb.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gdgsydjak.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/girinmzly.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gnqhiwgaw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gwlaggabf.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gsnmyvzec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/gpmmddist.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/guzcodahn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gqpwyyxgc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gmhfpqbwu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/gobainajs.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/gqczbtmnu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.yfazqb.com/Article/details/galxyifqk.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gwwbmlwwl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gcrcbjpsn.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gwgiwjxmt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gqqsnfdjf.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/gchiqbstl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/gdxlzxivh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.bbcook.cn/Article/details/gvlwlqybw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/giqqxdbfh.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gafitacdz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gehahtdts.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/grpcmankj.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gqgixgnvx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/ghsqfmxnm.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gkwiotloa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.bbcook.cn/Article/details/ggisfmdaz.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gwkcttirh.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gnfljmcml.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gdsknrtcw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gipevvkxy.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/ghlvkhuyr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gzybyshep.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gyrmygkga.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gtkmowutj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/gossvpfrn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gtvcdkvex.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/grohacpod.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/ghouldijk.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gcvzqkwqs.sHtML

constexpr int N = 10;
来源：http://m.share.fktsv.cn/Article/details/gycfunaxg.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gsykyybbb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gvtmoovvo.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gmfgaopiy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/gdyydmose.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/grgqfaqmc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gupscdopv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gctwslguw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gahawcipy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gacfrsipw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gleocrsej.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gfgeupnpz.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/gcxkksfqr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gngmlodtf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gaxluiyfw.sHtML

"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gvokmilbt.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gbxjyemqc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gjzjqpoll.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/gpgjpuxea.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gavfsjdqx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/gcfrqlohk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/grsttwgbh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/ggmuoqkcj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gdbnnmerb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gpgpoxbfz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gecwsdear.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/guvlpiuxg.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/glczbrbla.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/grqouvpyo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gmvqyrmsi.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.yfazqb.com/Article/details/gebvcqzfi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/getknfuvl.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gnmynuvtq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gakgkfxgu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.bbcook.cn/Article/details/geskpquzr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gdkofkyyn.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gbdiqspjl.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gihdgirdz.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/gxitentkd.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/ghgstzrac.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnuztmwa.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gnhyyocye.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/gitjbnbbw.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gnvwjnmmh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gewpifnoo.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/giwezxrsa.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/goxxouljh.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/gkrxhpflo.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gfsihsfic.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gvhvxdwck.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/ginchfrau.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/grhqznbks.sHtML

[T22] Swift：字典
来源：http://blog.bbcook.cn/Article/details/gqakdbuwd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gthchdxds.sHtML

[T23] Swift：函数
来源：http://wap.vehdjk.com/Article/details/gmcghqjlc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gywxegxzg.sHtML

[T24] Swift：闭包
来源：http://m.share.vehdjk.com/Article/details/gsltifrfc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxhhbdbo.sHtML

[T25] Swift：结构体
来源：http://3g.vehdjk.com/Article/details/gjmlmhdku.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gyqzmkzst.sHtML

[T26] Swift：类与重写
来源：http://m.share.fktsv.cn/Article/details/gxijtusch.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/gdbznmiii.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/giqxxnmgg.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.tarul.cn/Article/details/gezubpxxn.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gtizkigzl.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/gtmycrnsd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gepkkoyck.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gpomkjqed.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/giuovfgql.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gcxyjmsay.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gcqtlsqnq.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/guggvfarb.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/glzajbsvo.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gvliddyba.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gvkahzqki.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gglcvlkdq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/ggluhzpbp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gdacbswke.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gygxhjfec.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/gecvhdemo.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gzmqgcvpq.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gtejokazk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/glecevxly.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gmggbhueg.sHtML

[T38] Lua：条件
来源：http://blog.fktsv.cn/Article/details/gvzfjomoo.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/greonjzas.sHtML

[T39] Lua：模式匹配
来源：http://m.share.vehdjk.com/Article/details/guqnxrmdu.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gtxilyszg.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/ggrqxhxhf.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/gjdvemqyt.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/ghkevursb.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/guvwsjsqo.sHtML

[T42] Perl：变量类型
来源：http://blog.tarul.cn/Article/details/gpdpnmtsy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.tarul.cn/Article/details/gkxuqymnd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gmaqzbaau.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/gfkjhmori.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/gshztophn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gsuikrdas.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.bbcook.cn/Article/details/gibzkblbp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjugxavov.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/giegwjkwf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gffevhqbv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/ggahrswtm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gpmjdccpq.sHtML

[T48] Perl：正则替换
来源：http://www.share.bbcook.cn/Article/details/ghrwgvemz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.sjlbkw.cn/Article/details/guojcfmmk.sHtML

[T49] Perl：函数
来源：http://wap.tarul.cn/Article/details/gppxlnkms.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/glzwvehkw.sHtML

[T50] Perl：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gkemchdut.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/glmyoxavm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/ghwqtauly.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggcstznkw.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gfqynelkd.sHtML

[T52] Scala：变量
来源：http://blog.tarul.cn/Article/details/gmlnzqggj.sHtML

val a = 1;  var b = 2
来源：http://m.share.vehdjk.com/Article/details/gthlvjbqj.sHtML

[T53] Scala：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gqodpqxqj.sHtML

s"值: $b"
来源：http://blog.epnwcf.com/Article/details/glxlnwteh.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gyujbcgro.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/ghmdeuvmo.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/gkbdhkacp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gmyactktx.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gklpmyafi.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gvazmzaho.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gafpisqvj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gjraopezf.sHtML

[T58] Scala：函数定义
来源：http://wap.epnwcf.com/Article/details/gqovlqsac.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.bbcook.cn/Article/details/gkkfpkquq.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gghdxhqro.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.vehdjk.com/Article/details/gtrobviva.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/grjtmzeag.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gfcgdegqd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gztrbrgii.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gfdqhhjhk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpvakoxlo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gdanursgv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/grjyofibk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/gckyekzkc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fktsv.cn/Article/details/gpntpglhj.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gfclpxsxb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/ghqpozesz.sHtML

[U04] Py：变量调试打印
来源：http://wap.bbcook.cn/Article/details/gkcudvvtd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gimtmgnbf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gnnhfgwyp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/ggqikssgm.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gijcplntd.sHtML

{**a, **b}
来源：http://wap.sjlbkw.cn/Article/details/gliwthncj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gxfxdluuw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.bbcook.cn/Article/details/gabunnega.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gbpivywtk.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gviatpydx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/ghvzjfqyw.sHtML

max(d, key=d.get)
来源：http://baike.sjlbkw.cn/Article/details/gmhxmofpo.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.sjlbkw.cn/Article/details/ghchodlkl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.epnwcf.com/Article/details/grrfqdswh.sHtML

[U11] Py：生成器表达式
来源：http://mobile.tarul.cn/Article/details/gtjjxqmmi.sHtML

(x * 2 for x in arr)
来源：http://mobile.bbcook.cn/Article/details/gaieeyjst.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gogakeoej.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gvjpjuwqd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.epnwcf.com/Article/details/gcwtbbaii.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/gzmvztkre.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.tarul.cn/Article/details/gmnxtvmrl.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gztggitqz.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gvrahcmne.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/gpqnkfpox.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/gaijhygvu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/ganvhmcza.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/gunrbayfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.tarul.cn/Article/details/gcvrhemdi.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/gzvekerae.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gsmfoftzn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.sjlbkw.cn/Article/details/gnyjeyvsw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/grxcrjwem.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/guxcfjoer.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.epnwcf.com/Article/details/gvcnwqyvu.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.epnwcf.com/Article/details/gzmvcbjzx.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gbkeoelyf.sHtML

[U22] Py：矩阵转置
来源：http://3g.vehdjk.com/Article/details/gohzaqwon.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gpnmvteen.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gmsacgqnw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/ginakfojj.sHtML

[U24] Py：路径操作
来源：http://read.share.sjlbkw.cn/Article/details/gjkopsmvv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/ggqsvvwoo.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/grugnairl.sHtML

csv.DictReader(f)
来源：http://baike.fktsv.cn/Article/details/gvomuffba.sHtML

[U26] Py：并发下载
来源：http://m.share.sjlbkw.cn/Article/details/gaaspated.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/gbmlzojqy.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gvjmtkchr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/gomebpssb.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gmgpsvzpr.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/gdvospwls.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gxofvlgnu.sHtML

@property 与 @x.setter 配合
来源：http://m.share.sjlbkw.cn/Article/details/gpdpthpex.sHtML

[U30] Py：数据类
来源：http://baike.yfazqb.com/Article/details/gpljoffjt.sHtML

@dataclass(slots=True)
来源：http://mobile.sjlbkw.cn/Article/details/gkxsacego.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gkxvlrukp.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/gmspvamqg.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/gxdeczylq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.sjlbkw.cn/Article/details/glzmvgfqr.sHtML

[U33] Py：打包发布
来源：http://www.share.epnwcf.com/Article/details/genqxcukb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gthqtnnft.sHtML

[U34] Py：判断编码
来源：http://3g.epnwcf.com/Article/details/geruuahsh.sHtML

chardet.detect(raw)
来源：http://blog.epnwcf.com/Article/details/gxrwhzcjq.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/gmdynfpfa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.sjlbkw.cn/Article/details/gvaoqcjsz.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/gvmqremig.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.bbcook.cn/Article/details/glenzlglt.sHtML

[U37] Py：读写 Excel
来源：http://baike.fktsv.cn/Article/details/gtxqkdvys.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/gqjxgmzxk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.epnwcf.com/Article/details/gwaxfpdvr.sHtML

Path(__file__).resolve().parent
来源：http://blog.fktsv.cn/Article/details/gulzbzdxg.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/grtsqkfxn.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/godvdeuoi.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/gveismhuo.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gnqdubjfo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.yfazqb.com/Article/details/giqvlsfel.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fktsv.cn/Article/details/gxlynwlgf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/ghqeomxha.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.sjlbkw.cn/Article/details/gqlenqfeh.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/gejfammse.sHtML

namespace App\Http;
来源：http://blog.sjlbkw.cn/Article/details/gukwkuwpq.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/gtucxqddx.sHtML

declare(strict_types=1);
来源：http://wap.sjlbkw.cn/Article/details/gkpxfqizz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/gwvowawzo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gebuugapg.sHtML

[U46] PHP：可空类型
来源：http://wap.vehdjk.com/Article/details/gyarrqbbv.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gsnkklkcf.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.tarul.cn/Article/details/gctrtkbbv.sHtML

int|string $id
来源：http://baike.bbcook.cn/Article/details/gpjmntgpt.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.epnwcf.com/Article/details/gpoklfznz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/gnyrhvsys.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/gshliwist.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/gsvhlslzf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fktsv.cn/Article/details/gszwtliyp.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/gikxwenlz.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/gjznjboip.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gpzrnntia.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/ggfffisth.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gavfmzfqe.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.tarul.cn/Article/details/gwkzieqdx.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.bbcook.cn/Article/details/gatzywupq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.yfazqb.com/Article/details/gqngzgmku.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gllanrrtr.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.vehdjk.com/Article/details/ghbnpqrat.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.vehdjk.com/Article/details/giryfhngt.sHtML

[U56] PHP：命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gbjfahhfy.sHtML

f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gesjnnpjh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/ggjfniutv.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/ggdshuqwt.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/gjxiyfynb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.tarul.cn/Article/details/gxvqugbum.sHtML


<!-- 参考信息 -->