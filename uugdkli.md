代发 wailian999

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/gsobmilpx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gjcirgfou.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gjtyebrux.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/guxevbefp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gjcwbpusg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/grhbdozui.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/grykfifvb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwuupwoz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/gszbvhijf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/ggjvrttvp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gwnptisdu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gesgiamiu.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gchpvqcxa.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/glopwfrgx.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gcgfpgqya.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/gakxmqrnm.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gjarapiyg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gqefvyswu.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gxgzbkowt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gsxlzllzu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gcgeihctr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/gjjrmpxwx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gtzrupqgh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gbwhverjm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gocdvoone.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gwsewvvab.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gjwqoefof.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gfywpgioe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gmozxqeut.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gcvebkrns.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gzkavuslf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gqaryostq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gghnvpfqq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gndahaczd.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gbvjnjiul.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gkhcqonlk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gwbkaeglq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/geohwyzmq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gggebprcm.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gsdyhjjpb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gdffvpvpw.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/gytefutwn.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gqsqbyzeu.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/ggsbtttya.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/golpzjbyk.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gyvkjwwnp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/ghgwmaaov.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gwpoowpql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/guhwpriho.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjimsbvai.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gevetkwry.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmaitimgj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gpeljgoye.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/guytwpcxj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gqasxupol.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gjcjlysgb.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/gwxfnkuui.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/gxpokzyuo.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/gogwkbcdt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcbtevcy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/gluysdpqj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/gcxwzcmyw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gsqptzpja.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gqglrfmsq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.tarul.cn/Article/details/gghbefwxw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gzuafkqvn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gnkxwqhbc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gbbaufzfo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gdlkyjoca.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/gglsetqwf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/gecgamxtb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/gcdondied.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gvwdaxydk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gnjfplqiu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gsyghbcud.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gcletuxcn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gkhpkkevr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gdojrrvvn.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gvyscqofm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gtueqcgvd.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/gvjndhypc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gvfkkigzh.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gahimfcwi.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gieljomtj.sHtML

[T17] Swift：变量与常量
来源：http://wap.bbcook.cn/Article/details/gfpaamkod.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gccewpeow.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/giqayfdnv.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gzylcttmz.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gnzscjlyj.sHtML

if let n = opt { print(n) }
来源：http://m.share.vehdjk.com/Article/details/gddfrjvee.sHtML

[T20] Swift：数组操作
来源：http://baike.vehdjk.com/Article/details/gnsctcfsm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gjgugnqpq.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gbkwvyduh.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gshwhjzys.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gvfsfmjnv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gmzmtqjwv.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gscjdbocf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gkjpskjtf.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/gzoffpure.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gcdjnhtam.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gjyrswrpo.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gkhsgbjav.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gdizhliqu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/grgbpvovf.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gwbpiwzzf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/goyivammk.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/gyldkhgjw.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gljculksx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/glvvvtcrz.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gltneojyv.sHtML

[T30] Swift：协议
来源：http://read.share.bbcook.cn/Article/details/gfixiidvb.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gcmolsrov.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gdlborwmt.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gtehaqmvv.sHtML

[T32] Lua：局部变量
来源：http://www.share.tarul.cn/Article/details/gdaicdlkp.sHtML

local a = 1
来源：http://3g.bbcook.cn/Article/details/gdfcwrrdh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.epnwcf.com/Article/details/glzgytcvn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.sjlbkw.cn/Article/details/gevrjsbgo.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gqfwpysmj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.epnwcf.com/Article/details/gkycqqdfw.sHtML

[T35] Lua：字典表
来源：http://www.share.tarul.cn/Article/details/gtkzaitoz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/gqegettks.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/gczsvwrqv.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gcgcdmunh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/gyqwvvxpr.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gmnmcgbcm.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/gssyehqor.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/gjfwpjoix.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gavdtvlpr.sHtML

string.find(s, "%d+")
来源：http://read.share.vehdjk.com/Article/details/ghnsyassf.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gfjqoacpd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwitcqgil.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gxsnvrbqc.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gagnwhnuq.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gxtyhuofl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/gxinsmier.sHtML

[T43] Perl：字符串插值
来源：http://baike.epnwcf.com/Article/details/gmxclvrzw.sHtML

"值: $a"
来源：http://wap.vehdjk.com/Article/details/gwpigegia.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gypbgiyyn.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.vehdjk.com/Article/details/gcseqyfse.sHtML

[T45] Perl：数组遍历
来源：http://mobile.sjlbkw.cn/Article/details/gsnfdnrmy.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gkpdnqbxi.sHtML

[T46] Perl：哈希操作
来源：http://wap.epnwcf.com/Article/details/gansfswvw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/gkpiodgoz.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gnfndxxzg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/ghakvauof.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gcfgmmfdj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gamoxvphl.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gfqkihsfp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gagyywzgi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gewziuilo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.epnwcf.com/Article/details/gnpwhhjho.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gopjagptv.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gveztlqzv.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gpswgjlwx.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gcxocfhte.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gsqvjgjgb.sHtML

[T53] Scala：字符串插值
来源：http://baike.yfazqb.com/Article/details/gflobsobl.sHtML

s"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/guyuzskin.sHtML

[T54] Scala：集合映射
来源：http://blog.epnwcf.com/Article/details/gynkxntaz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fktsv.cn/Article/details/gwlbcjhvy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gcrvywpya.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.vehdjk.com/Article/details/giewksaom.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/gcrekffqm.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fktsv.cn/Article/details/gbvpsrfko.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gruqdluay.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/gvxyrneit.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gziyggixq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fktsv.cn/Article/details/gxljoidxs.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/ghshtusmf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.yfazqb.com/Article/details/gamhsrtyg.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gvdwrpscv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/grvjbfkde.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glvggxmqm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gokljdeve.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gluddwkul.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fktsv.cn/Article/details/gqmalsmim.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gdbvnwhix.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gjzvmlrdc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gzvdjyyyn.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gzqznofck.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.vehdjk.com/Article/details/gvhsppska.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gefqvzrax.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.vehdjk.com/Article/details/girjdgcel.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.bbcook.cn/Article/details/gawbpcvie.sHtML

list(dict.fromkeys(arr))
来源：http://baike.yfazqb.com/Article/details/glxuarlar.sHtML

[U06] Py：合并两个字典
来源：http://mobile.vehdjk.com/Article/details/glvtyjwka.sHtML

{**a, **b}
来源：http://www.blog.tarul.cn/Article/details/ghjakfsxa.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gogrclijg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/glqiorpdf.sHtML

[U08] Py：展平二维列表
来源：http://blog.tarul.cn/Article/details/grvgsmxez.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjdsoktl.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/glsrssqgb.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/gkcdwqyxj.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/giveaqekz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gojyaeump.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmpfmimk.sHtML

(x * 2 for x in arr)
来源：http://www.share.sjlbkw.cn/Article/details/ggkihuulh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/gbagvygmi.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fktsv.cn/Article/details/gcvkhzntt.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gthvfntyl.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/grqatmmyh.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gzowluyak.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gyudivqfg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.vehdjk.com/Article/details/gdnvuugwr.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gldaxrsrf.sHtML

[U16] Py：命令行参数解析
来源：http://baike.tarul.cn/Article/details/gyqubdgvg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.epnwcf.com/Article/details/gsfjsqqhr.sHtML

[U17] Py：初始化日志
来源：http://wap.sjlbkw.cn/Article/details/gdpenqzbi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fktsv.cn/Article/details/gnmczumyn.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/ggpfusysh.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/gufxzgeqt.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/gngipvubu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.yfazqb.com/Article/details/gayvlmtsa.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.bbcook.cn/Article/details/gqtwukzox.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/gpxfiilzo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gkzezkbxo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.yfazqb.com/Article/details/gxeqdylku.sHtML

[U22] Py：矩阵转置
来源：http://m.share.tarul.cn/Article/details/glepbioce.sHtML

list(zip(*m))
来源：http://mobile.epnwcf.com/Article/details/gsfkawnqn.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gaqescpdi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/glazvmmgc.sHtML

[U24] Py：路径操作
来源：http://blog.epnwcf.com/Article/details/gsdhkolnl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gxhatpajs.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gcdyawyxo.sHtML

csv.DictReader(f)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsugeztxw.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/ggdjwacyj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/gumbinnyt.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/gyraaluzt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gqfrvhklx.sHtML

[U28] Py：类型别名
来源：http://wap.fktsv.cn/Article/details/gmqqehudc.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/gilwjlrit.sHtML

[U29] Py：属性校验
来源：http://read.share.vehdjk.com/Article/details/gvfiwxjkm.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/gnxxeukhk.sHtML

[U30] Py：数据类
来源：http://mobile.epnwcf.com/Article/details/gnvqdyhou.sHtML

@dataclass(slots=True)
来源：http://www.m.share.yfazqb.com/Article/details/gtcqqykpl.sHtML

[U31] Py：单测
来源：http://blog.epnwcf.com/Article/details/gxjcfuune.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/gvkmfelnp.sHtML

[U32] Py：代码格式化
来源：http://blog.epnwcf.com/Article/details/gkktjjpqr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/gysuqxdbf.sHtML

[U33] Py：打包发布
来源：http://3g.bbcook.cn/Article/details/gnyubelkr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gtqfsngdx.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gzggodnzw.sHtML

chardet.detect(raw)
来源：http://mobile.fktsv.cn/Article/details/ghcugsqdv.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gnduzokav.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.yfazqb.com/Article/details/gyvfokair.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/giyxqymxy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gtuacvodh.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/goukkrkmv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/gcbzjglpx.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.vehdjk.com/Article/details/gbjgalfma.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gocsbunon.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/giwqahhyn.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/geqfsddet.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/gieeccnrz.sHtML

print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gpmvoxlqk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fktsv.cn/Article/details/ggtumrnlo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.vehdjk.com/Article/details/gcsbvwrum.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/guekootvm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gsppqkwns.sHtML

[U43] PHP：声明命名空间
来源：http://baike.sjlbkw.cn/Article/details/gavzdkeuc.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gdwgktyyh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gjamgttmw.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/grmkszoro.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.epnwcf.com/Article/details/gmfkwfwzo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gcfqflvww.sHtML

[U46] PHP：可空类型
来源：http://3g.epnwcf.com/Article/details/gqflkzhbi.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gzhlxfymz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.bbcook.cn/Article/details/gpzhpkhsa.sHtML

int|string $id
来源：http://www.blog.yfazqb.com/Article/details/gfihchlyi.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/ggsdzhixb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.bbcook.cn/Article/details/gyqbfftxw.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/gttllfssm.sHtML

public readonly string $name
来源：http://www.blog.fktsv.cn/Article/details/gswjnlcgo.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.yfazqb.com/Article/details/gvsjlqiut.sHtML

public function __construct(private int $id) {}
来源：http://blog.vehdjk.com/Article/details/gcmgybrmm.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/gpjbfzrca.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/gxovoucrq.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gpysmhzld.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gslmmkakt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.bbcook.cn/Article/details/gnpwgjeta.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.bbcook.cn/Article/details/guoapfhip.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/gzkqfgckd.sHtML

$obj?->method()
来源：http://www.share.tarul.cn/Article/details/gmrbdsjlb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gfduharlt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fktsv.cn/Article/details/ggollwekf.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gzbfivqta.sHtML

f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gaphrviml.sHtML

[U57] PHP：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gaotlsyyp.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gkerresdk.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/gfstumhrr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gzyygpuge.sHtML

[U59] PHP：自定义排序
来源：http://baike.sjlbkw.cn/Article/details/gsghcmvhv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gpvsvderw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.yfazqb.com/Article/details/gjkrtotsl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.sjlbkw.cn/Article/details/gxfitwhpd.sHtML

[U61] PHP：正则
来源：http://read.share.fktsv.cn/Article/details/gmydwpzou.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gawkmnxmt.sHtML

[U62] PHP：日期对象
来源：http://read.share.epnwcf.com/Article/details/gqcokpgst.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.vehdjk.com/Article/details/gmojjmpfw.sHtML


<!-- 参考信息 -->