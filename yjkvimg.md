代发 wailian999

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gcvdjttcj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gklyjankn.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/gsnqpejek.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/ghmtmzxyc.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gjrguints.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gphwhmhrf.sHtML

[S38] C++：排序
来源：http://m.share.sjlbkw.cn/Article/details/gzgqwtezr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/guwdztwpi.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/glqzlahij.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gitnnwbpo.sHtML

[S40] C++：查找元素
来源：http://www.m.share.vehdjk.com/Article/details/gtqtyamcr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gatnpsjbo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/gjuutqjbp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/gygcxsbbx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gimbcmjzt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gpznuefkj.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gvjmiplpx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gtoctrdfk.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gexpqhsii.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gowpokhbo.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gkxrotidd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gtsptvadf.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gqqwbpjhn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gbaitzwab.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/ggsxcmwnp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.sjlbkw.cn/Article/details/gkugqtses.sHtML

[S48] C++：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gzeirworx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/gcrcvyggx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/gpsvbzbkk.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gjwbhsifs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/gktyokqxp.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gulcebpte.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gopkvntlr.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gjyplutwj.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gcjvbmpqz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gfxznguvz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gyoynpuyp.sHtML

[S53] C++：移动语义
来源：http://mobile.yfazqb.com/Article/details/gtwbgpbee.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gadupwduu.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/grsydemee.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gukvpikvk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gqifhjmte.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gqdirctug.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/glaerhnlk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/gtsirtkcc.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/gbtlitdei.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gakrichgl.sHtML

[S58] C++：命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gcpifjgzx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gljoqvmei.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/glysuefma.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gcwirwkkb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/ggvcwddpa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gtkamztru.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gccugqwmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gsgnpqzfe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfyaaquai.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gjqoqnnoq.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gmbvmdaer.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/gadvgebwq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.bbcook.cn/Article/details/glidytjbc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gdgxeljej.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gfzvodqbp.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gtmzyggoc.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/gcvaashqt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gxqsarqqu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/gyfwikpew.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gybroommq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/gawydhylq.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gbgdvdkov.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gabesopqk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gjzgacrho.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gaocwonta.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gxpoggirk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeyzzssq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/gdykmcybd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/gbixsgygl.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/gbcibhzod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gtnxpjfxz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gsnbjbaox.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gwzarelkb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gdjxgrubg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.bbcook.cn/Article/details/gaydpujbg.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gzjcgspst.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/goinwlbqs.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/goqowzoxk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gtiqpyczc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gvrsthpoo.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gkgnllehf.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/guaivmegk.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gulifpelj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gcojayrrb.sHtML

"值: \(b)"
来源：http://m.share.epnwcf.com/Article/details/gcftnqdpl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gruxlphwp.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gzpemlmcn.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/givlpwloo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.vehdjk.com/Article/details/gnkiaalke.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gwqdclwbq.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gmhhinast.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/gxgebfyww.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gtuezzphb.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/gmaromzxz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gqfrfmxdi.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/grqjvtkxf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gqkhopnrq.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gpckwzism.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gsicefvdv.sHtML

[T26] Swift：类与重写
来源：http://read.share.epnwcf.com/Article/details/gcvuljmak.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gvwpjbmmz.sHtML

[T27] Swift：错误处理
来源：http://mobile.bbcook.cn/Article/details/gwndehhrx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.epnwcf.com/Article/details/gzqsbfrff.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gpfhvjioz.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gvapsscab.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gzwctczmu.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/ganwydcnw.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gbwpuwukw.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gylolitai.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gwyaxbrfs.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gfdafvwdk.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gmrtkimsc.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/gfghzocuv.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/gajwdhant.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gtuoyqkxg.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gmslaqmyk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gvfeyhyhr.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/ggfzjmfuu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/grkqxgfym.sHtML

[T36] Lua：函数
来源：http://blog.epnwcf.com/Article/details/gttsdssst.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/garqgqpbp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gwmjkqdne.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gmfbztjjm.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gbpypwpdl.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.yfazqb.com/Article/details/ggaszvqlq.sHtML

[T39] Lua：模式匹配
来源：http://3g.fktsv.cn/Article/details/gdzxqkcvu.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/ggknjynjb.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/ghwjwntla.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gbubwdnrw.sHtML

[T41] Perl：Hello World
来源：http://wap.fktsv.cn/Article/details/goweixvlf.sHtML

print "Hello\n";
来源：http://wap.epnwcf.com/Article/details/guvvhhxyf.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gvsrmvqej.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gqvfclkyo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gehcouswt.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/ggepidojb.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gwrvbhdgr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gttrjlxvw.sHtML

[T45] Perl：数组遍历
来源：http://mobile.epnwcf.com/Article/details/gcgepshlm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.bbcook.cn/Article/details/gsnwtuefs.sHtML

[T46] Perl：哈希操作
来源：http://wap.vehdjk.com/Article/details/gyvldyjyp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.yfazqb.com/Article/details/gjwfagmsh.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/gbjunfmyx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/gkmmbwwcy.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/grkgqpqwd.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gkcenhnjs.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/ggmtuwrik.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gcgaiwxtp.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/girnsxlvp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/gicyzpffh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.yfazqb.com/Article/details/gqxxlghjb.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/ggjrytcqs.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/ghyxnsafd.sHtML

[T52] Scala：变量
来源：http://baike.epnwcf.com/Article/details/grluljsfb.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gwjqfkfnu.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gfrtktyrk.sHtML

s"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gqdzlmari.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/gxlfudpbn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gukzylrit.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gsrfkzqdq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/ggtucyxhk.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gjxzrpsqc.sHtML

case class User(name: String, age: Int)
来源：http://www.share.bbcook.cn/Article/details/gegmsgdww.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gomjbxdjf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gbpaoyvar.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gyvxxrqpp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gcvngfqrb.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gonihiiqo.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/goqipmvmh.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gehzcecmd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gjyajxbhu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfaudkyig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gatoxmxsi.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmadaivfc.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.tarul.cn/Article/details/gyngyecxp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/ginzusufp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.epnwcf.com/Article/details/gcclmkgpy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/gqsjcwlqm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gsnnyeoul.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gjkhzvcna.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gcomtrefy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.vehdjk.com/Article/details/gcyprxjxx.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fktsv.cn/Article/details/guzdaegpi.sHtML

list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gupnqxqve.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gktyamjxj.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gvvrbrbtb.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gtxmswapd.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fktsv.cn/Article/details/gpsphwmww.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/gjffhbjjo.sHtML

[y for x in nested for y in x]
来源：http://3g.yfazqb.com/Article/details/gjikoyexa.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.tarul.cn/Article/details/gxcedjvyd.sHtML

max(d, key=d.get)
来源：http://blog.epnwcf.com/Article/details/gpdisprec.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gzonfuyla.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gjdjiqtsa.sHtML

[U11] Py：生成器表达式
来源：http://wap.vehdjk.com/Article/details/gbdfivwyb.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gwvewbfbs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gqmdmanyk.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/gtegwixbc.sHtML

[U13] Py：固定长度队列
来源：http://blog.bbcook.cn/Article/details/glqfxycom.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/ggjujjatn.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/gqklyhphe.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gjhmzjizh.sHtML

[U15] Py：高精度计时
来源：http://mobile.yfazqb.com/Article/details/gfamtgeys.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/ghseftzpj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.yfazqb.com/Article/details/ggjzplvpy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gmmskozea.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gvoawzdhw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gxmvquvwc.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gimvtumyd.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gqqodjaqr.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/gndcpqoke.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/grtbwilna.sHtML

[U20] Py：缓存函数结果
来源：http://baike.yfazqb.com/Article/details/gmksgyfdo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/gxyhzwhys.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.vehdjk.com/Article/details/goprpgpug.sHtML

@contextlib.contextmanager
来源：http://www.blog.epnwcf.com/Article/details/gbrrczkoa.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.bbcook.cn/Article/details/grqwijjzf.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/guugwufxz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fktsv.cn/Article/details/gddacpygx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/gebmwnzib.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gfnprdtmx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gzwkqmhsa.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/gtxbzlhuw.sHtML

csv.DictReader(f)
来源：http://wap.fktsv.cn/Article/details/gdfxugwev.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/gdpilyguw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.sjlbkw.cn/Article/details/gizhipagw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gydrxxxsp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.sjlbkw.cn/Article/details/gaagekhdt.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/gqtkgzqfy.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gfczgjrcn.sHtML

[U29] Py：属性校验
来源：http://blog.fktsv.cn/Article/details/gjzjdrmlh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.yfazqb.com/Article/details/gvmrfufmb.sHtML

[U30] Py：数据类
来源：http://baike.epnwcf.com/Article/details/graerytkd.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/gqhapkzfw.sHtML

[U31] Py：单测
来源：http://3g.vehdjk.com/Article/details/gfrybwhpm.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gdebsllxq.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/gekmybepf.sHtML

ruff format . && ruff check --fix .
来源：http://3g.bbcook.cn/Article/details/gjtxobtrn.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gdxnfzmep.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fktsv.cn/Article/details/glxhauucr.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/ghsgmlkxo.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gpxfxltrx.sHtML

[U35] Py：发送邮件
来源：http://www.blog.vehdjk.com/Article/details/gjoiamaqw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.sjlbkw.cn/Article/details/gftfivslr.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/gcvaxhbkd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gtbghlggf.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.sjlbkw.cn/Article/details/gyctalihy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.epnwcf.com/Article/details/gqqomgouu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/gxuvkfwcl.sHtML

Path(__file__).resolve().parent
来源：http://baike.yfazqb.com/Article/details/gsmxvinbu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/glrshvaez.sHtML

sys.stdout.isatty()
来源：http://www.blog.yfazqb.com/Article/details/ggfxfhvah.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gylolanmm.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gruiikryq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.sjlbkw.cn/Article/details/gnkncjrzi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.epnwcf.com/Article/details/gkygoqnog.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gdmmvspyi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fktsv.cn/Article/details/gspqrksgw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.yfazqb.com/Article/details/gvgtbatdk.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/glhqumhmr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.tarul.cn/Article/details/gnxktmpnl.sHtML

declare(strict_types=1);
来源：http://wap.epnwcf.com/Article/details/gcjgtsgsh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/ggagjibwq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gghopygbq.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/gqanwpari.sHtML

?string $name = null
来源：http://wap.epnwcf.com/Article/details/gflmwlemz.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gsbxxbzqv.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gfwkgwcgt.sHtML

[U48] PHP：纯枚举
来源：http://m.share.vehdjk.com/Article/details/gaohcpikr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.yfazqb.com/Article/details/gzqdwdjcc.sHtML

[U49] PHP：只读属性
来源：http://mobile.bbcook.cn/Article/details/gdazdxovg.sHtML

public readonly string $name
来源：http://3g.tarul.cn/Article/details/gmnfgmozc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/gicsatshy.sHtML

public function __construct(private int $id) {}
来源：http://mobile.tarul.cn/Article/details/gocuaadba.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/ggqmbocfb.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/gmunovxuc.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gmlutnycr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/ganljruhm.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/gsokzeeah.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.yfazqb.com/Article/details/gqnjoeddb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/gakgwxrlb.sHtML

$obj?->method()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfsfmiej.sHtML

[U55] PHP：match 表达式
来源：http://baike.bbcook.cn/Article/details/geaktntaa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gxyihedlc.sHtML

[U56] PHP：命名参数
来源：http://wap.sjlbkw.cn/Article/details/gnxoxbkqe.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gaglxwufk.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gpmlhedyq.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gzluwaply.sHtML

[U58] PHP：数组三件套
来源：http://wap.vehdjk.com/Article/details/gsabuwlfm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.bbcook.cn/Article/details/ggqtnyjtj.sHtML

[U59] PHP：自定义排序
来源：http://3g.fktsv.cn/Article/details/gszmkadhh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gutkmpufs.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gxnwkrwrv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.yfazqb.com/Article/details/ghqbhnhri.sHtML


<!-- 参考信息 -->