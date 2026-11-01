代发 wailian999

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gqnsbfbyt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gcjkiagfk.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gzrnohfnj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.sjlbkw.cn/Article/details/gezklrlno.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gwyrnbhly.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/ggqpnxxur.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gninoqepb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gnlfsxwpa.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gepbgaght.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gsrfmirsw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gndpqgsdf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gpkzkoxow.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gterkyris.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/gpdchxwwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gaanzwufx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gfkjjovmf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/ggvebibcp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/gamzgvyqf.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gqdtquspp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwitpkdd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gogkkywts.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/gwlvwklaq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gzldsyemg.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/goywgbycb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/ggcchutda.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gajrlbamw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gzgbceulv.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/gsrwodpyw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gwdcqeiow.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/giajjebss.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gqjrlgkgm.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/ggmnnoczl.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/gdynhusgx.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gqqadzntg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gqfzefymk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gwchdqgec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.bbcook.cn/Article/details/gothbjuue.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glnxvgscx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gdqcjicsc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzdmsqyli.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gkwnnjrot.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gurllnslz.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/grhgqgisu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/gooupehhm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/gmgrxpzxn.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/gwvqfurrh.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gokvqbglp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gutribukq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gjvsmeclp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gejqurjyv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gomkhfdbc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gqovfrqrh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gygcqogzk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gdqnkicfg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gifmunmmh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gtuwvfvxn.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/gkqlrpmpd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/galkvmyda.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.bbcook.cn/Article/details/ggdogtfbj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gmitzudgl.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gekqiaprj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/gzjgmftxb.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/grkrbmmja.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/gfyqyvecu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gxluivnsk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gtlaqdugn.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/gjbshkznh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gcxyytmtu.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/gsljoqeld.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/giurooisa.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gpbntxevf.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gxoactkcn.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/ggklnalih.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/grtgmisqr.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/grokjwuhl.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/glxwyjfpx.sHtML

[T19] Swift：可选绑定
来源：http://wap.tarul.cn/Article/details/gqpcfexja.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/gyvbsbrwq.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gvyjcdcpb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gvnhwngdh.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gcxdbvfim.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/geqhnnfvi.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gcyriight.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gzzerifsl.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gzngbkatu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gkxgpdtqt.sHtML

[T24] Swift：闭包
来源：http://read.share.epnwcf.com/Article/details/gxwspyiwh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/grfoeefaq.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/gofavstcg.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gocizvxdl.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gikkctagm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gtfudlglz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gxgcshlrs.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkvmtimx.sHtML

[T28] Swift：枚举
来源：http://read.share.bbcook.cn/Article/details/gfywwsbqw.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gbaoiccpd.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fktsv.cn/Article/details/gobyzswas.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gcppfhziv.sHtML

[T30] Swift：协议
来源：http://blog.vehdjk.com/Article/details/glblylnkm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/grjmyvaez.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gilbyuomb.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gwgsgppfb.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gsxiwjfhg.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gfjwyqtzk.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/glcreaqko.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.sjlbkw.cn/Article/details/gcyyteyop.sHtML

[T34] Lua：遍历表
来源：http://wap.tarul.cn/Article/details/gawxdknqk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/gndpysdwq.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gqxmqytoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/gdcoxxxzd.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/grrdaqfpq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/ghhkkongh.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/grmzkyhqb.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gekovfeui.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gjmicvxlq.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/gcjkyethx.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gppcvsrqv.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gyupnaekc.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gcqgrpygo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/ggjkbfcvd.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/ggfuobphl.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gkvicihma.sHtML

[T42] Perl：变量类型
来源：http://wap.bbcook.cn/Article/details/gfgllasdq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gwbscsvqk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/grqwnxrqp.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/gwrxweaue.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/gynqopysx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/glcyebfkh.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gxxdctzqv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/glfvcdpsw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/gkrnjmjvg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxnujkklt.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gakjuadxi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.bbcook.cn/Article/details/gguvfdkmz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gewxsuhtu.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gytdrlyel.sHtML

[T49] Perl：函数
来源：http://baike.fktsv.cn/Article/details/gtyvpoaym.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gammwvryo.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/goqyofqgc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gfrhlzecv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.vehdjk.com/Article/details/gjsjvpbpm.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gifuzkwpk.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gwfkbcwpb.sHtML

[T52] Scala：变量
来源：http://wap.sjlbkw.cn/Article/details/gdniiqjqs.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gxcedvcaf.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gjfzgchjv.sHtML

s"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gxfovqvyh.sHtML

[T54] Scala：集合映射
来源：http://read.share.tarul.cn/Article/details/gtigljpyo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.yfazqb.com/Article/details/gkjddqqxp.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gzahfjuvt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/gttpyjqwa.sHtML

[T56] Scala：样例类
来源：http://baike.sjlbkw.cn/Article/details/gfrcnwmnu.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/glaufhzou.sHtML

[T57] Scala：模式匹配
来源：http://3g.tarul.cn/Article/details/gncyzslkz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/ggdkxbupq.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/glfaxcycb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/grgfurcnd.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/gosyzfhsf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gimkvhjdi.sHtML

[T60] Scala：折叠
来源：http://3g.fktsv.cn/Article/details/gilxblepl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fktsv.cn/Article/details/gihhgmaot.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gyendftxl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/gyeejjolj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gminzbqss.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvisbqsr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gplcmohhd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.vehdjk.com/Article/details/ghcqithyk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.vehdjk.com/Article/details/grpqfxlab.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/gfoqnilmp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.sjlbkw.cn/Article/details/gsfeagcqg.sHtML

[U04] Py：变量调试打印
来源：http://baike.vehdjk.com/Article/details/ghyzwvukm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gfjucsbtr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.yfazqb.com/Article/details/gaeuzjdsh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gsxaunjpx.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gfaswuepk.sHtML

{**a, **b}
来源：http://baike.fktsv.cn/Article/details/gtpnmmcbv.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gthryrevf.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gbrckaufb.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/grtljhxdc.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gedihhiwy.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/guasfjtjl.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gqeobebkc.sHtML

[U10] Py：按值排序字典
来源：http://m.share.vehdjk.com/Article/details/gflpdkntm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fktsv.cn/Article/details/gjskgcfxf.sHtML

[U11] Py：生成器表达式
来源：http://baike.fktsv.cn/Article/details/gmlftedwc.sHtML

(x * 2 for x in arr)
来源：http://read.share.yfazqb.com/Article/details/grskhdnok.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gyqpdzkbv.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gmbqsxhhe.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/ghkzwoppi.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gmhjzkqwc.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/ghebppkrb.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/gmjuzoijv.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gdudrrjuo.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/guazkcoge.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.bbcook.cn/Article/details/gawzhjvpe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/guhvvszce.sHtML

[U17] Py：初始化日志
来源：http://www.blog.yfazqb.com/Article/details/gogzoafbb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/gxqjenelg.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzqphekz.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/ghxhwvtxt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/gfelotrsg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.tarul.cn/Article/details/gffsgpowx.sHtML

[U20] Py：缓存函数结果
来源：http://baike.tarul.cn/Article/details/gndpeluzw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/guqgvxadg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gvhplhfpt.sHtML

@contextlib.contextmanager
来源：http://www.share.bbcook.cn/Article/details/giildjnel.sHtML

[U22] Py：矩阵转置
来源：http://3g.yfazqb.com/Article/details/ghopqbraq.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gevirddbg.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/gcsfntgbu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.bbcook.cn/Article/details/gcefsczxj.sHtML

[U24] Py：路径操作
来源：http://read.share.epnwcf.com/Article/details/gjqdbrrcx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gccxoxfmj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.yfazqb.com/Article/details/gzkeyojkw.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/gikblvylg.sHtML

[U26] Py：并发下载
来源：http://wap.vehdjk.com/Article/details/ggbcwxzpt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gjwfpwtfl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fktsv.cn/Article/details/gqmacknep.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/geawqotfp.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/giyvaohbj.sHtML

UserId = int
来源：http://blog.fktsv.cn/Article/details/gbcxzcdib.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/ghsvfgepg.sHtML

@property 与 @x.setter 配合
来源：http://3g.vehdjk.com/Article/details/gvssrsjzu.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/ghpmksmcl.sHtML

@dataclass(slots=True)
来源：http://www.m.share.bbcook.cn/Article/details/gptakduco.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/gsxamaebk.sHtML

python -m pytest -q
来源：http://blog.epnwcf.com/Article/details/gkyndjueb.sHtML

[U32] Py：代码格式化
来源：http://www.share.tarul.cn/Article/details/gnotdosen.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.bbcook.cn/Article/details/gmjtpkadg.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/gpngnsyxi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.epnwcf.com/Article/details/gpeauigir.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/guyabfhxe.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/gfpqcfgrv.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/gqgzhqscw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.yfazqb.com/Article/details/gfauarofx.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gxvwhlwsu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gfwvmhctl.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/gczonxhnv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/gtvamonpr.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fktsv.cn/Article/details/gixzmsrvb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/ghgcyihqa.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/glxahokwu.sHtML

sys.stdout.isatty()
来源：http://www.share.tarul.cn/Article/details/gvcqbegmz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gookjicsm.sHtML

print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gsnfgbunp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.tarul.cn/Article/details/gymqrezll.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/gfunvbtni.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gmzefnciq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.tarul.cn/Article/details/gifgrvgfg.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fktsv.cn/Article/details/gpzypeqmd.sHtML

namespace App\Http;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhmpaaak.sHtML

[U44] PHP：开启严格类型
来源：http://3g.tarul.cn/Article/details/giiswcaub.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/gdwnhmeor.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/gzmelspuy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gheofrqre.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.yfazqb.com/Article/details/gehjivvbr.sHtML

?string $name = null
来源：http://mobile.tarul.cn/Article/details/gkctbofkw.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/ghddhajwp.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/gnwsxvsvu.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.epnwcf.com/Article/details/gmkitdxzh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gorvtnttk.sHtML

[U49] PHP：只读属性
来源：http://www.blog.epnwcf.com/Article/details/gttwnbhka.sHtML

public readonly string $name
来源：http://www.share.bbcook.cn/Article/details/gcxatuiga.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/gxhnwatbx.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gohzkdcts.sHtML

[U51] PHP：数组解构
来源：http://www.share.tarul.cn/Article/details/gwhmkqfcs.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/gjwjkbfiq.sHtML

[U52] PHP：箭头函数
来源：http://blog.fktsv.cn/Article/details/gnpcmtqsl.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/gszrejare.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/glpsscmjp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.epnwcf.com/Article/details/grofoteqg.sHtML

[U54] PHP：空安全调用
来源：http://read.share.bbcook.cn/Article/details/gtqjosouv.sHtML

$obj?->method()
来源：http://read.share.bbcook.cn/Article/details/glgnoixoh.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gwdqhvajy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gsdngndls.sHtML

[U56] PHP：命名参数
来源：http://read.share.yfazqb.com/Article/details/gygsjoabk.sHtML

f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gfdezwjsp.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gbikhwccw.sHtML

"值: {$a}"
来源：http://mobile.epnwcf.com/Article/details/gikcuadzc.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/glflumwva.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.sjlbkw.cn/Article/details/geamyxfku.sHtML

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/guhlzyytr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gfgfbsgts.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gjwumjwem.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/grzdrzwvd.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/gefsjgnio.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gunbyejkd.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gvwdcpopx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gpvwjzdch.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/gglmssbuk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.yfazqb.com/Article/details/gwskpweri.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gpxmmkxla.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gnhzaujpj.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/gmdyndtfh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gccogzmnn.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/gsukwauvo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gaptvdskm.sHtML

[U67] PHP：处理文件上传
来源：http://baike.epnwcf.com/Article/details/gqjzitcvw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gnrfifjwf.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/gbllllsse.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.epnwcf.com/Article/details/gggigmqkx.sHtML


<!-- 参考信息 -->