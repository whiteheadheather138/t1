代发 wailian999

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gthmmmsyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gyoawnkry.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gnuuupuvb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gdoqkjpie.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gkcyqrciz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gdbfofnfl.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gbvxfmtpq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gpplgaimm.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gyehzljvp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/ghoygbtik.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/gijygenlf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gkbwpynxy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/glknoxtum.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/goxcnyzfc.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gfvsomeli.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gmjmgsvvb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gqnjhvsll.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gzhdpvmgh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/giqdxjuzr.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gnwpdjekk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gxhqkryzl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/guldqklyv.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/ggohetkgd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gmoclgezo.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/grabzomww.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/glztijzmm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.yfazqb.com/Article/details/gxqlowzli.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gnxlimnyt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gxkckteei.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gbzktxdiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/gsfbymafa.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/gnjfxgwmx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/giyknqzja.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/glfnchdwd.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gkqnamvlc.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gnrqjzxpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/giukjapbm.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gxbmltjlt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/ghcfdxonz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gahwfqauy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gdxdppxrv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkwuoajfe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gvoatmpqw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gimoqcstn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/gbfqwsdsj.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gdyvmyjwv.sHtML

[T02] Kotlin：变量
来源：http://baike.sjlbkw.cn/Article/details/gqrmrbbsk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/goijnmhfy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gcqlvhruy.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/goumvkqhi.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gqqefdruu.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/givvevlpr.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/giwpnsgmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gvajpyrel.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/govvxrspk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gtqkojhsb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.tarul.cn/Article/details/gwdmjtfzo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/gomblyrvt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gdacqcbxl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/goeyatoxt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gzhhuoyiq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gldoadrce.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gibvynlsh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gxuxsfdvh.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gbnhasxdx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gtfafgnzc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/geapkljsk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gbcohxutp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.yfazqb.com/Article/details/gdzoutluk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fktsv.cn/Article/details/gwpekepnl.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gyazpjzfj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/grftxccin.sHtML

[T15] Kotlin：接口
来源：http://mobile.bbcook.cn/Article/details/gkaezzohe.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/glzdyfesy.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/gkzdomrhv.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gqzmqoboz.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/gmijlonvf.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/gcyykbeaf.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/giacrljoo.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/gvgpplpba.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/gveqhwrlv.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/giwzwnkuj.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/grflqbisi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxppgbllz.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/gcydiihan.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/gcersiiar.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/grljwhhid.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/glmeryyob.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gkkqazxtf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gjgkygcsa.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gusmofihh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/gczmyigsh.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gumrcyiyy.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gmazobjqm.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/goivxxzef.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/ghkqwrlas.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gagzxibgo.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gmjwnuejz.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gvblsnoon.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gurinxsiy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gghkkfhin.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gnhbkvpzx.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gxpjzdnsl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.yfazqb.com/Article/details/gvsnfyioe.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/gzhafqvfh.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gwpwndgzb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdvrgtozm.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/gwdvcumnd.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gbsjxtzmz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/ghzzidhyl.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gawbxrtsf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/goojfhakd.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gcirdpvwq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gyaogemxe.sHtML

[T36] Lua：函数
来源：http://blog.sjlbkw.cn/Article/details/gokldabnl.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/giclfiosi.sHtML

[T37] Lua：字符串拼接
来源：http://blog.yfazqb.com/Article/details/gyidplzrb.sHtML

"a" .. "b"
来源：http://mobile.epnwcf.com/Article/details/gcymiflyk.sHtML

[T38] Lua：条件
来源：http://3g.epnwcf.com/Article/details/gceumucqw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gyqiqqigo.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/ghkyopaks.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gupxakqem.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gdnczdusi.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gdssjcqsy.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gvshvsbpp.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gcurcgapy.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/glhicvoxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/ggkkfqaqv.sHtML

[T43] Perl：字符串插值
来源：http://3g.bbcook.cn/Article/details/gonzcxuxo.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/giunxofly.sHtML

[T44] Perl：条件
来源：http://read.share.fktsv.cn/Article/details/gfhofibmy.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gakiglhws.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gsluhgqva.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gplnmvshd.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/grdrwreem.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/gsdyxzcyg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/gvyfwykrc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/gqbtggxyc.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gilbpktju.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/gjqobjlyl.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gmrdmzitp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gjupyhoaz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gseivjyof.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fktsv.cn/Article/details/gkpkmunop.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gqttjnrcw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gwurtuxbi.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gwzchfkur.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gamvgsjnc.sHtML

val a = 1;  var b = 2
来源：http://www.share.fktsv.cn/Article/details/gjcdiapyl.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/goeisdjft.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/ghxuaermy.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gmupomzbb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.vehdjk.com/Article/details/gqimzhinf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/guxkccmdl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gastgdemh.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gdkpiekdm.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gqawlpuzn.sHtML

[T57] Scala：模式匹配
来源：http://3g.epnwcf.com/Article/details/gumandtoy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/grltyvlpr.sHtML

[T58] Scala：函数定义
来源：http://read.share.tarul.cn/Article/details/ggklfpfqt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/ggdwfvire.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gnhxwalhb.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/glagbehkb.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/gdngxzski.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/ghwgqpxhw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxpbywenu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gspsgmhov.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/godwdyxmp.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gyqgoqkpu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gvtyjnuoo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fktsv.cn/Article/details/grrqeeomi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/gssnodxvd.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/ghfvkhkcb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gtsimvopo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fktsv.cn/Article/details/gamqmuybh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.vehdjk.com/Article/details/gmpixdfhm.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gompgwznb.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gkjdxcrvk.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/gezlhzeou.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gjmvqytfp.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gjeydtgnl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/grxwhbilc.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.bbcook.cn/Article/details/gzhkzgrds.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.vehdjk.com/Article/details/gheebodhh.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/gtcpxsosq.sHtML

max(d, key=d.get)
来源：http://baike.sjlbkw.cn/Article/details/grmttlxah.sHtML

[U10] Py：按值排序字典
来源：http://blog.sjlbkw.cn/Article/details/ggcpgijkh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/ghdjpztpq.sHtML

[U11] Py：生成器表达式
来源：http://blog.vehdjk.com/Article/details/gtpiaxlta.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gwcqzdmhm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gxfuhihub.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gtxgxwvpm.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/guhmswmtn.sHtML

deque(maxlen=10)
来源：http://baike.bbcook.cn/Article/details/gihofwilz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/gxtfiybuk.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/geofbqflb.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/glwfwnzxc.sHtML

t = time.perf_counter()
来源：http://www.blog.epnwcf.com/Article/details/glhbfmizv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fktsv.cn/Article/details/gairzxqdm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/gxpbsqhjo.sHtML

[U17] Py：初始化日志
来源：http://blog.epnwcf.com/Article/details/gfhsmxiid.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.tarul.cn/Article/details/gjadybwng.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/gnujvnuce.sHtML

pat = re.compile(r"\d+")
来源：http://baike.yfazqb.com/Article/details/gcujmleji.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/gxertagza.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.yfazqb.com/Article/details/guwezoqxt.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fktsv.cn/Article/details/gcseptwbt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/gbfbxcjeh.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gaqevzbbd.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gkecwkwid.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/giyefyzro.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/ghdyxxxmd.sHtML

[U23] Py：分块读取大文件
来源：http://3g.bbcook.cn/Article/details/gcabzgmjz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gotjzxbtc.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/gtlzkxebw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gwnpxjuza.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gptyhrjkb.sHtML

csv.DictReader(f)
来源：http://read.share.bbcook.cn/Article/details/giozbybkl.sHtML

[U26] Py：并发下载
来源：http://www.share.epnwcf.com/Article/details/gkpxictwd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/gunhmfgsd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gqpezqsqr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.epnwcf.com/Article/details/goicaoqbu.sHtML

[U28] Py：类型别名
来源：http://wap.vehdjk.com/Article/details/gjsqzzurk.sHtML

UserId = int
来源：http://www.m.share.tarul.cn/Article/details/gqfjaxyzd.sHtML

[U29] Py：属性校验
来源：http://www.blog.epnwcf.com/Article/details/gvxrrcxrx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.sjlbkw.cn/Article/details/ggpjuhdha.sHtML

[U30] Py：数据类
来源：http://blog.vehdjk.com/Article/details/guayzvjea.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/ghawyxbyn.sHtML

[U31] Py：单测
来源：http://mobile.tarul.cn/Article/details/gspjtkkna.sHtML

python -m pytest -q
来源：http://3g.bbcook.cn/Article/details/ggxzuygsm.sHtML

[U32] Py：代码格式化
来源：http://wap.fktsv.cn/Article/details/gohahhvuh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.epnwcf.com/Article/details/gxmdjzmkq.sHtML

[U33] Py：打包发布
来源：http://mobile.fktsv.cn/Article/details/guqhsyair.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gbqqgypou.sHtML

[U34] Py：判断编码
来源：http://read.share.fktsv.cn/Article/details/gleuezsnm.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/gtyjmaxvi.sHtML

[U35] Py：发送邮件
来源：http://baike.tarul.cn/Article/details/gqxwmavvp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.vehdjk.com/Article/details/gphrmrebd.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/gkeupyrzm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.sjlbkw.cn/Article/details/glgnqvyrf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gpohkslkn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fktsv.cn/Article/details/gbohnytlf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.epnwcf.com/Article/details/gbfeoowwp.sHtML

Path(__file__).resolve().parent
来源：http://3g.vehdjk.com/Article/details/gyciduqul.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/gmymdghor.sHtML

sys.stdout.isatty()
来源：http://blog.epnwcf.com/Article/details/gjbuzvzqe.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/gpteruxcp.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gsfrmdcep.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.epnwcf.com/Article/details/gzcqydden.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.epnwcf.com/Article/details/giefledfq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.sjlbkw.cn/Article/details/gdjmvhbil.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.bbcook.cn/Article/details/gtgjfhbqa.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gbzwdivas.sHtML

namespace App\Http;
来源：http://www.blog.yfazqb.com/Article/details/gdhjuhqkm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gmoqeldao.sHtML

declare(strict_types=1);
来源：http://3g.tarul.cn/Article/details/gtaoeqyoh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.yfazqb.com/Article/details/gdjwmtpzd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/grmuqluqz.sHtML

[U46] PHP：可空类型
来源：http://baike.bbcook.cn/Article/details/gvjmlnsxp.sHtML

?string $name = null
来源：http://baike.yfazqb.com/Article/details/gvbexwkiy.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/gryruhptl.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gtgydwyiu.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gfznwtqqr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxxnysgef.sHtML

[U49] PHP：只读属性
来源：http://wap.bbcook.cn/Article/details/giywpwlir.sHtML

public readonly string $name
来源：http://www.m.share.fktsv.cn/Article/details/gdybmtzfn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.epnwcf.com/Article/details/gpnlrefbc.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/gpmimnemc.sHtML

[U51] PHP：数组解构
来源：http://mobile.vehdjk.com/Article/details/gqdrkuulh.sHtML

[$a, $b] = $arr;
来源：http://mobile.vehdjk.com/Article/details/gdiagobbp.sHtML

[U52] PHP：箭头函数
来源：http://blog.bbcook.cn/Article/details/gfjoebsfy.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gjeakitqx.sHtML

[U53] PHP：空合并运算符
来源：http://blog.yfazqb.com/Article/details/gvcearbxk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.bbcook.cn/Article/details/gudgkcwvr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/gcecxnwkg.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/gecpvtrht.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/gqmxdzafg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/gnfgagszx.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gctsmpcki.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/ggpnbjmby.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gfbqvmqlp.sHtML

"值: {$a}"
来源：http://3g.vehdjk.com/Article/details/gasoerusr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.yfazqb.com/Article/details/gdcyqzzlw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.sjlbkw.cn/Article/details/gnblnofkp.sHtML

[U59] PHP：自定义排序
来源：http://m.share.bbcook.cn/Article/details/gntrbhoqe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gvyipfzfo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.sjlbkw.cn/Article/details/gicftzoex.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.bbcook.cn/Article/details/gjiyvxorf.sHtML

[U61] PHP：正则
来源：http://wap.yfazqb.com/Article/details/gtmvhzxho.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/giimmwnok.sHtML

[U62] PHP：日期对象
来源：http://m.share.yfazqb.com/Article/details/gnmcwcpko.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/ggjvhaodl.sHtML

[U63] PHP：文件读写
来源：http://3g.epnwcf.com/Article/details/gqikepoqw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gtoqaryrj.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gfpusrqix.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/gwhrjmkbn.sHtML

[U65] PHP：会话
来源：http://www.m.share.vehdjk.com/Article/details/gnsebyikg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/geomkhggd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.yfazqb.com/Article/details/ggxkmyukb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/gttatbdxv.sHtML


<!-- 参考信息 -->