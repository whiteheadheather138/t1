代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gtahzvmhh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gaqvrgxmh.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/gmieipskc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gccjusbdo.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/ghccahxmi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/gziftstge.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.vehdjk.com/Article/details/gmuitjthc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gwkyuxllj.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gvdfrztzc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.sjlbkw.cn/Article/details/gcbtchhkd.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/geeplbenn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/grritqvoe.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/ggaeyuebr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gfartsgzl.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/gdlopowga.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gvxjbmwzr.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gkpcgopva.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gmrwewefa.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gptsqiddy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gjpefsimz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gseckjzpb.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gqusbypyq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gepkahqsa.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/gclvwhqhv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gfcqdthrj.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gqmiybcci.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/geaqwicml.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gfvehygim.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gffiiqhlw.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gedjixxnr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/givtjndju.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/greqqxafj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.sjlbkw.cn/Article/details/glsyrejsj.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gxplgvvyj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gphsonisb.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gkqdymdoe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gnywdvfaf.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/gnbwpdxcr.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/ggvmbpqtn.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/gyytegfvn.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gfuyuinlk.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/ghaelwgtc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gsrkfanfv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gmzwlikdi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/ggdbpxoal.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzzwhdxey.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gaekeqhai.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdcbnkwdm.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gpisuhqjn.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gimoqubbo.sHtML

[T02] Kotlin：变量
来源：http://www.share.sjlbkw.cn/Article/details/gxfgtyzgj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gkvwwhjom.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gukzggost.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/ghshqhfvy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gruwochaq.sHtML

val n: String? = null;  n?.length
来源：http://blog.fktsv.cn/Article/details/gxjpbokod.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gitaowpez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/gifbxtich.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/ginvkkczy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/gdiinwonr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gslkkjipf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gqatxcfhh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/ggsvqndbw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/gcrbnxnju.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gjcedcqsd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gvjgbvnix.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/ghoctzpxr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.bbcook.cn/Article/details/grzdqaknh.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/guicmixpk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gwtktmuvx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gqdffzcfe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdogwlhny.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/glpdaxtbb.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gaisxqqqw.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gqjvavyar.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gbhvjxicl.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gbdvbtbrk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/greuhgbzg.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gkgyztyhs.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gnqaatahq.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gmqzdqnqm.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gevmmpfhz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gyfesplkf.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gfqzxlmbs.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gmweqqppl.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gnmyxmygm.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gebchrbpb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gdqtwjoxq.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/gjzcqfwrl.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/ggcokjoux.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gucsodddp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/gqbpkenzc.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gweckrpwk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/gymhcedjs.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gdwantyfn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/guhyntvxw.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gixsfrwrx.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gvyvvkmjo.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/geonewqra.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/glvzmjfft.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/gshbkvdnt.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gnbsasgwq.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/gtwtqcwxr.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/gvklkzdzl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gtgbzmvmm.sHtML

guard let x = opt else { return }
来源：http://www.blog.epnwcf.com/Article/details/gfqnbsdqs.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/ganhllnkh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gettkxgao.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/gwqzdwijb.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gyqtetrap.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/ghrbummcg.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/giysiuhre.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gwgsqmlni.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gagmcycev.sHtML

[T34] Lua：遍历表
来源：http://wap.bbcook.cn/Article/details/gpghzfstr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/gktcjwuec.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/gcmlnzgrk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/goqbxbxgo.sHtML

[T36] Lua：函数
来源：http://baike.vehdjk.com/Article/details/guypgdqvi.sHtML

function add(a, b) return a + b end
来源：http://mobile.yfazqb.com/Article/details/guckkeyad.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gncxumisp.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/gnspxojns.sHtML

[T38] Lua：条件
来源：http://wap.fktsv.cn/Article/details/gaxvluwjx.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gwhpcecrj.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gutdubxuy.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/glhuokaww.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/ggbygytiz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gegppkmvn.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gzmqwitvg.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/grokpcpus.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/gzbhszmef.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gsrdnguus.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gtkhyhzet.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gldioufrb.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/gclxnugel.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/gwmzakmjg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/gtbkdknxs.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/gjreudeiw.sHtML

[T46] Perl：哈希操作
来源：http://blog.epnwcf.com/Article/details/gotbeqgkm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.yfazqb.com/Article/details/gbbwmsykl.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gaktuhjmq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gocduhcpk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/geqkrcfbp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.sjlbkw.cn/Article/details/gotlxyfxr.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/ggbclzlbf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gccoibaey.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gfxbqaeyh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gcbhxokna.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gyxtuaoxc.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/gwefopzfm.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gvifqojqv.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gmbprzrnb.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gvllijnas.sHtML

[T53] Scala：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gauabqqem.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gggwwvdbv.sHtML

[T54] Scala：集合映射
来源：http://3g.bbcook.cn/Article/details/gvibdubny.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/gdcxpthit.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gfuyxcuzh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/ggpxmdhpd.sHtML

[T56] Scala：样例类
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvfxulie.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gpfjwynzg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gvabmvyyl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/gbbnqdspm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.sjlbkw.cn/Article/details/godorlgsf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/gydvncjhu.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gnsaonmff.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.tarul.cn/Article/details/gdejucwqe.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gpaemrnmv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gmthjeech.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gamuxbswk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/grqsxxemj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnflusnye.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.sjlbkw.cn/Article/details/gcyxtflkj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gbhftwwml.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.epnwcf.com/Article/details/gdlolyddl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gjiuumijf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gluaellxt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.tarul.cn/Article/details/givxpchqb.sHtML

[U04] Py：变量调试打印
来源：http://blog.vehdjk.com/Article/details/gfjeyttoh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/gempykvmx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gvojtbiay.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/ggxykxpkh.sHtML

[U06] Py：合并两个字典
来源：http://wap.fktsv.cn/Article/details/gmiwdekgp.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/ggnesjjqk.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/grmnofyql.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gqrffwzjd.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/gwebmdjvh.sHtML

[y for x in nested for y in x]
来源：http://blog.fktsv.cn/Article/details/getekigta.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gaidufenx.sHtML

max(d, key=d.get)
来源：http://www.share.vehdjk.com/Article/details/gmeisbmfy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gkfhkljng.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gircugmxz.sHtML

[U11] Py：生成器表达式
来源：http://m.share.bbcook.cn/Article/details/gctqmreva.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gmalcdbpl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/grppfvxxo.sHtML

Counter(arr).most_common(3)
来源：http://blog.sjlbkw.cn/Article/details/gogbeklro.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gwpzqdagc.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gwcyzkrsq.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gzucmarba.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/glvthjqms.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/gkcasfwrj.sHtML

t = time.perf_counter()
来源：http://read.share.sjlbkw.cn/Article/details/gdmuepwud.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gdurloszf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/gzryfzjhn.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/giasonzvo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.bbcook.cn/Article/details/glpbtffse.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gybmufmih.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/gakyowhzs.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fktsv.cn/Article/details/gmuiouuqq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwuhcyes.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/gmkwnrsot.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/gzistpusx.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/gkbmjquir.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gxqjwklon.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/goinxwnvc.sHtML

list(zip(*m))
来源：http://www.m.share.epnwcf.com/Article/details/gdgdopkng.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.epnwcf.com/Article/details/gnmattdyl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/gefmfkoss.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gxlsmsium.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gbyimmzyn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/gkknmqwar.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gvbshcrpy.sHtML

[U26] Py：并发下载
来源：http://blog.yfazqb.com/Article/details/goctzgkdm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gbcalqcnd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.yfazqb.com/Article/details/gvehajqfb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.bbcook.cn/Article/details/ghmvrmixp.sHtML

[U28] Py：类型别名
来源：http://wap.sjlbkw.cn/Article/details/gaopgproo.sHtML

UserId = int
来源：http://read.share.epnwcf.com/Article/details/gxyvmmurb.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/geetfbwnv.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gkqbsccuq.sHtML

[U30] Py：数据类
来源：http://mobile.tarul.cn/Article/details/gieqckkrm.sHtML

@dataclass(slots=True)
来源：http://baike.sjlbkw.cn/Article/details/gmcngzmed.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/gwgcxyibo.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gtrjblthh.sHtML

[U32] Py：代码格式化
来源：http://www.share.tarul.cn/Article/details/gaeogranh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gkmgkmhbb.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/ggtizjkig.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gxsmpanex.sHtML

[U34] Py：判断编码
来源：http://www.share.bbcook.cn/Article/details/gjbsvwcxd.sHtML

chardet.detect(raw)
来源：http://m.share.bbcook.cn/Article/details/gqxxmexuw.sHtML

[U35] Py：发送邮件
来源：http://wap.sjlbkw.cn/Article/details/gcfxvzydf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fktsv.cn/Article/details/ggltgdkxq.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gldakqvls.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.vehdjk.com/Article/details/ghhzoatis.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/gnsatxker.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gofzqsrtf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/gwpdqulyf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.vehdjk.com/Article/details/gnkpkuinx.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/glgcekekm.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gxawjtpyl.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fktsv.cn/Article/details/ghccobbpk.sHtML

print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gzfhvdhkf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gkhzwavar.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.bbcook.cn/Article/details/gonotoozh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.bbcook.cn/Article/details/glefosoxh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.tarul.cn/Article/details/gxvaxiobv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gaiioofag.sHtML

namespace App\Http;
来源：http://3g.tarul.cn/Article/details/gklojqdvp.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gahyyppze.sHtML

declare(strict_types=1);
来源：http://mobile.epnwcf.com/Article/details/gidgnwnaq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.sjlbkw.cn/Article/details/gimvgwmlw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gmmssmfsw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/gxfbieqaw.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gfytgyhtl.sHtML

[U47] PHP：联合类型
来源：http://baike.yfazqb.com/Article/details/gxerbtovm.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gbjtsirks.sHtML

[U48] PHP：纯枚举
来源：http://www.share.vehdjk.com/Article/details/ghdfaqohl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gpxdufwlm.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gdllpsdkg.sHtML

public readonly string $name
来源：http://blog.bbcook.cn/Article/details/gkntlyapr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.yfazqb.com/Article/details/gfnlbdisi.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/grrtdfmpe.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/geauckwpp.sHtML

[$a, $b] = $arr;
来源：http://blog.sjlbkw.cn/Article/details/gserqofje.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gtaeeubkt.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.tarul.cn/Article/details/ghvcqlygo.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fktsv.cn/Article/details/gzdtbssrf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fktsv.cn/Article/details/glpzvynic.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/gescmpnxu.sHtML

$obj?->method()
来源：http://www.share.tarul.cn/Article/details/ggmzjugjq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/gqrposhos.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/grhdbqhzk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.bbcook.cn/Article/details/gqnxurgzj.sHtML

f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gfoovjppm.sHtML

[U57] PHP：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gxhhhgrcg.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gedawyumd.sHtML

[U58] PHP：数组三件套
来源：http://read.share.sjlbkw.cn/Article/details/gjukptdbt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gidtxscvm.sHtML

[U59] PHP：自定义排序
来源：http://mobile.epnwcf.com/Article/details/goruezqcm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gfvzcsinw.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/greviwcbb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/ggsniykoz.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/guncdupgh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gudglcnpp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.vehdjk.com/Article/details/gkldilhwy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gaxeamsgv.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gcpvluaxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gfcrvjbee.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.epnwcf.com/Article/details/guvcazvaq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gjxdafzzy.sHtML


<!-- 参考信息 -->