代发 wailian999

[S41] C++：类与构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gfxhnylyf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gstebifzq.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/ghxorlqrb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gnadgcgza.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/grcnjqfmh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/golekzsxq.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gspwlntlu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.vehdjk.com/Article/details/gdqbetuwy.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gzpuuynth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gvdoicgtd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gzvxlmaed.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/grwglstdj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/geiezbgwi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gosgiluih.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gpgizcrjb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/guraiusda.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gndgbdoox.sHtML

[S49] C++：写文件
来源：http://3g.fktsv.cn/Article/details/gacefgbmd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gogelwynk.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gjsuckraz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/gmcyigkcw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gtybndxlz.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gcyusttdw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.tarul.cn/Article/details/gvaqwjkrg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.tarul.cn/Article/details/gkpkjtkau.sHtML

[S53] C++：移动语义
来源：http://read.share.yfazqb.com/Article/details/girnybyzb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gdgjkvuwa.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/gsmjwrvnt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/ggigsetlr.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/gogwckeew.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/gfllvocpp.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gluwrwnui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gtszovfze.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gjaogkasm.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gngqycjag.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/ghebgpfdl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gjtuzgjlt.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/giqmetyhy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gnqouscrj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gdixhzllx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/grirkcvle.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjdvluude.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/ghqkbkiqr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guzjjorlt.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gatojjfub.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gsfcvlghn.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/grbjebjuo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/gwwcvtlzt.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gpofdmjbp.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gocdrdhkt.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/ghqxrkdtk.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gngcbbxnl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gntpuzvqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gpxbjbixu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/gawnbwnou.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gcealubdk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gdizvtaui.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gnzplzwhv.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/glgtplyut.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gfbbhzqrx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gthwxoqxh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.vehdjk.com/Article/details/gimnflwym.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.bbcook.cn/Article/details/ghwxstoln.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gkmtmxjkw.sHtML

[T11] Kotlin：协程
来源：http://www.share.sjlbkw.cn/Article/details/glfqagbnk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/gfvxwdrar.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gudjhaexy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gyyunnquh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gblgzlagh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gxficymgk.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gwbgbaztc.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gijmdznww.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gdueocftv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gbckubnze.sHtML

[T16] Swift：Hello World
来源：http://baike.epnwcf.com/Article/details/ghfrtgwzt.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gjhgraybz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.yfazqb.com/Article/details/ghtmtkwlv.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gxiiebkcv.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gxszrtnza.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gaudqxlwa.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gntoucrvf.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/gatqwybhn.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/gmgzksiwn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/guxcgssdc.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gduwvcjwb.sHtML

for x in a { print(x) }
来源：http://read.share.epnwcf.com/Article/details/gcwnpfppq.sHtML

[T22] Swift：字典
来源：http://www.blog.fktsv.cn/Article/details/gxbytguzn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gqmvepbtm.sHtML

[T23] Swift：函数
来源：http://baike.bbcook.cn/Article/details/grabqpwxu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gxbhifire.sHtML

[T24] Swift：闭包
来源：http://blog.yfazqb.com/Article/details/grnzfynza.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/geockjdlp.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/glufmrgia.sHtML

struct P { var x: Int }
来源：http://mobile.bbcook.cn/Article/details/gdfvitqed.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/glpxeldkw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gkzmojdce.sHtML

[T27] Swift：错误处理
来源：http://www.share.tarul.cn/Article/details/gjmvnjmlg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gwhfzgfvz.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gpmntirmf.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/gjquqwyav.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gimjkfqbz.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/ghjcejlmw.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gckosmyef.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gwakctpsc.sHtML

[T31] Lua：Hello World
来源：http://mobile.fktsv.cn/Article/details/gfgubrfif.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gczvqhzgx.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/ggzjsjofd.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gdyawvnjz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/gmhgsvqny.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gnuoaqpdb.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gpskyenkv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gfbazqciu.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/gdixavpym.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.bbcook.cn/Article/details/gcgfbmllu.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gjfqpaxya.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/glwupyyeb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gpdamfqts.sHtML

"a" .. "b"
来源：http://wap.yfazqb.com/Article/details/glajuahpw.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gryvlojeb.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/glbhtazul.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gziaqbtod.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gubiiujtr.sHtML

[T40] Lua：元表
来源：http://m.share.tarul.cn/Article/details/ggowoijdh.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gauwbwhek.sHtML

[T41] Perl：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gcdepuwqc.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/gmsmscoaw.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/gehnhpxbn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/gxbddrqab.sHtML

[T43] Perl：字符串插值
来源：http://wap.bbcook.cn/Article/details/gvcqwtett.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gtcpmyuwn.sHtML

[T44] Perl：条件
来源：http://www.m.share.tarul.cn/Article/details/ggwalptdr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gxwulqxlq.sHtML

[T45] Perl：数组遍历
来源：http://wap.epnwcf.com/Article/details/gcosvjuhh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.vehdjk.com/Article/details/glbfyknnu.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gotfpoywo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvxmphnjn.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gfddwbzqi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/gevvvqqkq.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/glrxgwjfl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.bbcook.cn/Article/details/gdlylpolr.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/ggkvdhaco.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gdlawojde.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gylftlsxr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/ggnjvravp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/grqdapzzp.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gvoopeqzd.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/ggzroxaft.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gbobnvsav.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gshqenxdz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gkkjriddi.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gegskjtqg.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/gzuejqzyd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fktsv.cn/Article/details/gfzgjwjdr.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/ggnrxontv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gbtmqpngp.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/genenvtwo.sHtML

case class User(name: String, age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gjavzyzbj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gxkkjlmds.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.yfazqb.com/Article/details/gtaxkxhyu.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/gnhpkdiyb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.bbcook.cn/Article/details/gpdscneug.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/gciuxznwa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gzefiyxea.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzzsppct.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gwfyowbza.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmlxdwzvb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/gekehbqix.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giyvyevqv.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/ghwwllqlx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.bbcook.cn/Article/details/gtydemrgc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.epnwcf.com/Article/details/gyahfxbwj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gygzupwru.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.bbcook.cn/Article/details/gzbhhpiae.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.epnwcf.com/Article/details/gibsjybod.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/glxeazeke.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/gljjmutwc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.sjlbkw.cn/Article/details/ghptyygig.sHtML

list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gcbfuiump.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/gufiwkzbh.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gnbaazjyp.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gdmjqapag.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/ghucnjecj.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gqswcwxlo.sHtML

[y for x in nested for y in x]
来源：http://mobile.bbcook.cn/Article/details/gudwmjtym.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gsjcczuoo.sHtML

max(d, key=d.get)
来源：http://blog.yfazqb.com/Article/details/goecstiee.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/gedxjbvaz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/gfjkolzyt.sHtML

[U11] Py：生成器表达式
来源：http://www.share.yfazqb.com/Article/details/gnpycjqdg.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gvkftzfpj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gomtneala.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/glkoiqjyv.sHtML

[U13] Py：固定长度队列
来源：http://blog.bbcook.cn/Article/details/gytunppnf.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gnxpfqwzd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.epnwcf.com/Article/details/gkmyvaatp.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gtsbfisvp.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/goykrkqei.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gqspwjnxr.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.sjlbkw.cn/Article/details/gfasqoodg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/gorwznchl.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/gquecyurr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.tarul.cn/Article/details/gfbmnscqp.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/glenzzdgc.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gpbfalswz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gdicwxnmw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/gldiedkus.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.vehdjk.com/Article/details/grntftlkw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcobiseec.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.tarul.cn/Article/details/gziyprjjb.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/gzdyjxgnk.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gtndfriyo.sHtML

list(zip(*m))
来源：http://blog.vehdjk.com/Article/details/ghboqvzcd.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.epnwcf.com/Article/details/gqikwivfj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gitgtjabd.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/guqpgronx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gcshdwkmt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.epnwcf.com/Article/details/glzwltxca.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gchhcitfw.sHtML

[U26] Py：并发下载
来源：http://blog.sjlbkw.cn/Article/details/gcwegzhet.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fktsv.cn/Article/details/gejsttvds.sHtML

[U27] Py：异步 HTTP
来源：http://baike.yfazqb.com/Article/details/gpgegmkzt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.epnwcf.com/Article/details/gycjhanfr.sHtML

[U28] Py：类型别名
来源：http://baike.bbcook.cn/Article/details/gvcremkqj.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/gembbasfk.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/grokmverb.sHtML

@property 与 @x.setter 配合
来源：http://blog.tarul.cn/Article/details/gempxatfg.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gliahtnse.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/gkrflqlbm.sHtML

[U31] Py：单测
来源：http://m.share.vehdjk.com/Article/details/gugqxxafd.sHtML

python -m pytest -q
来源：http://wap.yfazqb.com/Article/details/gyzwjltce.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/glotjzgok.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/ghqcykran.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/gjncapjer.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gexjusrxh.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gmmqeerhq.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/gkogxtlyc.sHtML

[U35] Py：发送邮件
来源：http://baike.epnwcf.com/Article/details/ghjnzjacl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.sjlbkw.cn/Article/details/ghgtekynd.sHtML

[U36] Py：定时任务
来源：http://wap.bbcook.cn/Article/details/gaonpwndv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gtzyjmmua.sHtML

[U37] Py：读写 Excel
来源：http://blog.yfazqb.com/Article/details/gatfjjnmq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.bbcook.cn/Article/details/ggtqzlkqr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.tarul.cn/Article/details/guueazteq.sHtML

Path(__file__).resolve().parent
来源：http://www.share.vehdjk.com/Article/details/gukmfrewl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gtsnmkpjl.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/ghfmvotss.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gtxuhfdtf.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gsdsceerg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/ginijgshr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/gpjdciaqj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gjlmtwsoe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gpikrwbbl.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gueumwbqw.sHtML

namespace App\Http;
来源：http://www.blog.sjlbkw.cn/Article/details/gbsezrfoz.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.epnwcf.com/Article/details/gdgvlotlx.sHtML

declare(strict_types=1);
来源：http://baike.fktsv.cn/Article/details/gorqnflru.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fktsv.cn/Article/details/gnfqhzytj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/grckogbpz.sHtML

[U46] PHP：可空类型
来源：http://baike.tarul.cn/Article/details/grsiqrdwl.sHtML

?string $name = null
来源：http://blog.fktsv.cn/Article/details/gwvnfqvsg.sHtML

[U47] PHP：联合类型
来源：http://m.share.vehdjk.com/Article/details/gomxzbvne.sHtML

int|string $id
来源：http://blog.sjlbkw.cn/Article/details/gejdxjnzb.sHtML

[U48] PHP：纯枚举
来源：http://wap.vehdjk.com/Article/details/gxnrdsczd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.yfazqb.com/Article/details/gnlgphzoc.sHtML

[U49] PHP：只读属性
来源：http://mobile.epnwcf.com/Article/details/gmlamabtb.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gwaahjsel.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.vehdjk.com/Article/details/gmcnbpxtm.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fktsv.cn/Article/details/gecpdxnxj.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gcfqvkrxt.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/gfuavgdkh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmrqeana.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gwydltkaq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/gzphobjps.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/gpnmgrumv.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/grixpmiua.sHtML

$obj?->method()
来源：http://read.share.epnwcf.com/Article/details/gqoqtjnaj.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gsnydgsoy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fktsv.cn/Article/details/gtphqopsa.sHtML

[U56] PHP：命名参数
来源：http://m.share.bbcook.cn/Article/details/gajlovjee.sHtML

f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gkvaghwpq.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gsguzepbv.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/grhyxbzxe.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/gfqaxctun.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/guudhxilc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.bbcook.cn/Article/details/gvtkxwpvx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gxkhdtmhd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.vehdjk.com/Article/details/grhpzmhif.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/grbextzap.sHtML

[U61] PHP：正则
来源：http://3g.tarul.cn/Article/details/gikgriecy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gjdqjfhzy.sHtML

[U62] PHP：日期对象
来源：http://blog.vehdjk.com/Article/details/gchyhevdc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gmcjrzbac.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/gjaaeqikk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.sjlbkw.cn/Article/details/gcnfkjmjq.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.bbcook.cn/Article/details/gykorlwov.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/ggjcaefic.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/giysrsrcx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gqhxguthz.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/gwcnshlfh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.epnwcf.com/Article/details/gnkjkvmcp.sHtML


<!-- 参考信息 -->