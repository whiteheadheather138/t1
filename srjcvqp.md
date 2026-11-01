代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gcodnshsg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/gntxklqbn.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gdyzsnhix.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gzqcyfrmz.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/glcvdmcto.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gjphnzvcf.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gcoplgkxf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/geaxzidhi.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gveguhcsi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/gdmwqwjgr.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gntfiqccr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gygsgkwpi.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/ggiarsfjl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/glozlrfrf.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gbupgyogt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gtwrzcwpf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gkdglfgqw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/guxxwqvyp.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gwlveaole.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gvkhrecel.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gusalywiz.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gzfleqbdw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gmzlsxluj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gijexlxoq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/govgcquph.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gcqaeoljl.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gulwpdiid.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gzqzyswik.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/gbvofxxia.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gbgtftofo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.bbcook.cn/Article/details/gjbdadthw.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gwylywdmb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gzelybywm.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/giplpusmj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gtvnmleur.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gaszwemql.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gobanouka.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gqpxetujl.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gsfsayuoz.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gggcwytio.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/gibvyolpu.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gsywtxwbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/gzayrzjxb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gwyjdxzwn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gneoukipg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxutjcmmv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gebltzeti.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsjcxriub.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gannilzbk.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gyutzzqfz.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gkbsuerpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gsbtrodgs.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gfumvufnc.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gcnqzyakh.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gtofmvmzx.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gwbtmgvjr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.bbcook.cn/Article/details/gsbsvjrok.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gsgfqtbhs.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/glcujjzmj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fktsv.cn/Article/details/ggsrvexpx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gixvltrrg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/ghqphmxrl.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gjnvckqpv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.bbcook.cn/Article/details/getkihjae.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gdqbcccud.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gggsodjlh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gshwfgnmv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gpjwgowfn.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/gfcjdqoyh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gsmxwmapv.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gurjusais.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/gdhivlyog.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/grkxklfek.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gtsukholj.sHtML

[T14] Kotlin：循环
来源：http://read.share.yfazqb.com/Article/details/gvaagxssy.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/gxwjkjzop.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/gvqzkxutv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gzhzjvqou.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gfzxoflak.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmihknvls.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/gddbfhjmm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gxkqwvyfp.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/ghdqpybrz.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gphflmahf.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gfhvexarq.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gdkplyzcl.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gfrrojbdn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/gcobhtnei.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gawmpblnm.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gmozjszxr.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gotnbyxws.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/gxhgcqnls.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/gkzzblraj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gecgydgsa.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/gjuevuhcl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gevuahdin.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/gsomhuatg.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gdchhkwwb.sHtML

[T26] Swift：类与重写
来源：http://mobile.tarul.cn/Article/details/gdvnczsdp.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/gjudpbpgc.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gkzaqytne.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/gvniaudty.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gjvadlujj.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/gquaitxgl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/glfrcucnr.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/ggvmemyde.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/gtipoalwl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gpanzhkwv.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/ggamiimqs.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/ggilvxtuh.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gmmypjndl.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/glwgeozty.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/gjmjolxgv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gantyoknh.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/gggyklsry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gucbcypwk.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/gzmnhqrbf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gxgryejjc.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/gmmqcruol.sHtML

function add(a, b) return a + b end
来源：http://m.share.fktsv.cn/Article/details/gheuwbvfm.sHtML

[T37] Lua：字符串拼接
来源：http://3g.vehdjk.com/Article/details/gzdjawqnu.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/gkanylbod.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gzslibqhw.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gmtlcniqr.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gzzmfhbsg.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gtbywkmka.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/goqwqijxb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gmyznvxsq.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gurwxndqe.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gxoxxetim.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/gpjaiarhv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/garpmkcdy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gsbxuukle.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/gbaubxkys.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/ggtbemwqo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.yfazqb.com/Article/details/gpqwiwqwa.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/gqaidwxzw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gunkgnfkl.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gofendkxj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gylbevvtt.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gbekversz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.sjlbkw.cn/Article/details/gqjramevf.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/ggejlwxfz.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gtrjbiczy.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/grsqzfkbr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gyebfxexj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gdngherwn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gcecfycbt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gztjagksu.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/grlujvvyd.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gxjbarzdl.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/grnomvurc.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gaxurivoh.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gmrfcdhpw.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/ggvhqkspx.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/girhnvppi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fktsv.cn/Article/details/gnajborhj.sHtML

[T55] Scala：集合过滤
来源：http://3g.epnwcf.com/Article/details/gdelkmjyf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.bbcook.cn/Article/details/gmyceijlr.sHtML

[T56] Scala：样例类
来源：http://mobile.fktsv.cn/Article/details/gxazbliuz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gnajfildt.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gxqyfjfsn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gvffoaclj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.sjlbkw.cn/Article/details/gcsxfreny.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/gzcrtgdgd.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/grouqjndv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gqfrhsueg.sHtML

[T60] Scala：折叠
来源：http://m.share.sjlbkw.cn/Article/details/gicuefosz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gunlyvfuq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqqxafrjy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gquntypbb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gykohmdjt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/gxyrmsgzk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gcxygvqhu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/gcivrztqu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gvbedkhpn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/gctxkecxg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/gbnoriric.sHtML

[U04] Py：变量调试打印
来源：http://www.share.sjlbkw.cn/Article/details/gwirlpwnx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/gmzyclajh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/gcsqodmcf.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/grdyltsld.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fktsv.cn/Article/details/gagqanhei.sHtML

{**a, **b}
来源：http://www.m.share.bbcook.cn/Article/details/geujhtgjw.sHtML

[U07] Py：反转字典键值
来源：http://blog.sjlbkw.cn/Article/details/gmvlbcarf.sHtML

{v: k for k, v in d.items()}
来源：http://baike.vehdjk.com/Article/details/gsjeuqshm.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/ggyeljwya.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/gkwsuaszu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gbtjjyajw.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gekigbxkh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/gfclgntkl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.epnwcf.com/Article/details/gubcqbghv.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/grbgslqxz.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/gdszbpqsm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fktsv.cn/Article/details/gurmpdvnw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gcxkirdvn.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gmhzmuugu.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/gvhxfmjng.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fktsv.cn/Article/details/gynlcuedq.sHtML

defaultdict(list)
来源：http://3g.tarul.cn/Article/details/grestfxol.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.sjlbkw.cn/Article/details/glecyxzri.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/gyyrgysbe.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/gknrnxitc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.bbcook.cn/Article/details/grqgjllhr.sHtML

[U17] Py：初始化日志
来源：http://blog.yfazqb.com/Article/details/gazngylvx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gojptdrxo.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gvqbpnozb.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gbohlmpoz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gsosljapu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/gclqyivfk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.bbcook.cn/Article/details/gtitumvss.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gcazaqkca.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gsgzudqof.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/gdqmdphdk.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/gpyfsxbux.sHtML

list(zip(*m))
来源：http://www.blog.tarul.cn/Article/details/gyyosbgif.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/gjkmzbgfw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/gwzrjrdfj.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/guyczftmu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/grpwveitq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gahhpdcfm.sHtML

csv.DictReader(f)
来源：http://3g.vehdjk.com/Article/details/ghvlnrviq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/gkhbkckqb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/ganercnkj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gjutyqyus.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/gtcmgitxk.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gfmizcmnz.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gkjulzudr.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gyxxxjvmp.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.yfazqb.com/Article/details/gtpeufphy.sHtML

[U30] Py：数据类
来源：http://www.blog.epnwcf.com/Article/details/gqvapepnn.sHtML

@dataclass(slots=True)
来源：http://www.m.share.epnwcf.com/Article/details/gumgnngpp.sHtML

[U31] Py：单测
来源：http://wap.tarul.cn/Article/details/gcuundrii.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gsvozveoh.sHtML

[U32] Py：代码格式化
来源：http://blog.yfazqb.com/Article/details/gzwmzxbjx.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.epnwcf.com/Article/details/gqkigqthc.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gwxfrmlkq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.sjlbkw.cn/Article/details/gvkfhdavy.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gcbkfbjse.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gcppbpqdc.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/ghuvtyswc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gbyrhoqye.sHtML

[U36] Py：定时任务
来源：http://www.share.vehdjk.com/Article/details/gdxlqajjf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/ggtuovtin.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/ganceawys.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/ggfmsnumv.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gjxwjaimw.sHtML

Path(__file__).resolve().parent
来源：http://wap.bbcook.cn/Article/details/gqgrbrhnq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.bbcook.cn/Article/details/gmjzqukpe.sHtML

sys.stdout.isatty()
来源：http://blog.vehdjk.com/Article/details/grkfvqkkf.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gnjkstjry.sHtML

print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gkrjhkiuw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fktsv.cn/Article/details/gzndxfqlb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/gqbodtpta.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/gsiefzdav.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/ginzherfz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gcglkizln.sHtML

namespace App\Http;
来源：http://www.share.vehdjk.com/Article/details/ghqrqrxka.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.epnwcf.com/Article/details/gwlbvuotl.sHtML

declare(strict_types=1);
来源：http://baike.fktsv.cn/Article/details/gpcjoblrz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fktsv.cn/Article/details/gavijcsbq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gppeycdte.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/gzpuvdban.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gyukpyijz.sHtML

[U47] PHP：联合类型
来源：http://mobile.vehdjk.com/Article/details/glgnvrjgv.sHtML

int|string $id
来源：http://baike.yfazqb.com/Article/details/gltehbfmr.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.tarul.cn/Article/details/gesnyggsi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.epnwcf.com/Article/details/gjepglopv.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/gxfrxkppe.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/gtiuoyese.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.yfazqb.com/Article/details/gredrnvir.sHtML

public function __construct(private int $id) {}
来源：http://mobile.sjlbkw.cn/Article/details/gwufwwirt.sHtML

[U51] PHP：数组解构
来源：http://mobile.vehdjk.com/Article/details/gttsshfiz.sHtML

[$a, $b] = $arr;
来源：http://read.share.bbcook.cn/Article/details/gdfixvjcm.sHtML

[U52] PHP：箭头函数
来源：http://mobile.yfazqb.com/Article/details/gahqftnuz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fktsv.cn/Article/details/glcjbzagv.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/gkbitzpdm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/gltxuioyd.sHtML

[U54] PHP：空安全调用
来源：http://baike.bbcook.cn/Article/details/gpuwogyiy.sHtML

$obj?->method()
来源：http://www.blog.fktsv.cn/Article/details/gwitvslfj.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/gpudgurgt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gjiwzzhha.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/gpsuybwab.sHtML

f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gupqtjojj.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/geljkzglx.sHtML

"值: {$a}"
来源：http://blog.sjlbkw.cn/Article/details/gcsbkbpnf.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gxotiiuag.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/gmxewedko.sHtML

[U59] PHP：自定义排序
来源：http://baike.bbcook.cn/Article/details/gnqzqucgz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gtmbooayl.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fktsv.cn/Article/details/gkubmuwgf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/glijbwnbb.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/gcyekzgoy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/gxzotqain.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gmphlengn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/guwpcoaxy.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gvyejjnrk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/geutzgygm.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/gywrqcaai.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/gapzqdcir.sHtML


<!-- 参考信息 -->