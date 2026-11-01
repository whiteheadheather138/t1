代发 wailian999

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/ghucaqvzc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gdotppmln.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/ghwtxhwks.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gravepkfa.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gtqmmkael.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.tarul.cn/Article/details/giglllgrw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gdjjjgkue.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.epnwcf.com/Article/details/gxkapfwyh.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gtxgyiwax.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gimztigbo.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gqligmoft.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/gnzhkfzsv.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gvmbrzntl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gljsntjug.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gtgauacnf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gljmpcxga.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gciiwyvpt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fktsv.cn/Article/details/gfyucybvu.sHtML

[S48] C++：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gqsdrazrw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gwexzcneb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gcccllhwh.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gpcvykert.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gdwltxyrl.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gcfpqwjpi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gwluzvexr.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gxmpbraip.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/gdybdvkvr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gqjrtuhxl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gvkpyuutp.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gwibcllbq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/ggumplrcp.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gnmipmkpz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gvjzuwyjf.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gstcktfjb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gcdbzbkmz.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gdfsvmcyd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gqfqedwad.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/goovwbpxs.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gfnznayvu.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gphzwrxqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/gyvzkbykh.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gqcbemafx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.epnwcf.com/Article/details/gmcoivgmr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/grsykkjke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.epnwcf.com/Article/details/gupypsihi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gobcwmbwv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gbducfnxh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmxuqmxil.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gddetrceu.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gmbylsuku.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gtjdeoaax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.tarul.cn/Article/details/gbgerithm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gjgjnckwf.sHtML

"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gwiqtjomy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.tarul.cn/Article/details/gzklfmsnk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gasygjamx.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.epnwcf.com/Article/details/gipciujnz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/geukhtepo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gqzuqwiet.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gjmlpttkc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gmvcwaqvv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gdyddawcz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/grnmphdfs.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gdukenfwa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/geqwfuvyk.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gmvebijyx.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gwkubprwg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gysqbuxlu.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gfmvfoljc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gnzymnhkm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/ghyhqubij.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gtpxeubkq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gxvajxivc.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gzrcnyixe.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gulzsmpbw.sHtML

for (i in 1..10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gfxmcirqr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gpbymiofz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/gpaqdqpeu.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gulkmjohm.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gvvxqrzoz.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gewgwftpv.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/goekzmomc.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gbveoelws.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gvzzfrojj.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gedpkvkif.sHtML

if let n = opt { print(n) }
来源：http://www.share.sjlbkw.cn/Article/details/gxpnjhlgc.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gjlhusvuo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gyfozqznk.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gamvxkzmh.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gjovoocdw.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfrmcofx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gewxpltwj.sHtML

[T23] Swift：函数
来源：http://mobile.yfazqb.com/Article/details/gbbnpqweo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/ghxqkreck.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gavputbso.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghukzhkrw.sHtML

[T25] Swift：结构体
来源：http://m.share.fktsv.cn/Article/details/gfvpmtnzb.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gununvvmd.sHtML

[T26] Swift：类与重写
来源：http://blog.fktsv.cn/Article/details/gpqjtsjku.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gjxrpqodn.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gkgipybjh.sHtML

do { try f() } catch { print(error) }
来源：http://wap.epnwcf.com/Article/details/gyxzekqea.sHtML

[T28] Swift：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gttntmxxi.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/gmhbvxqer.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.vehdjk.com/Article/details/gboclykif.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gscbwhsuq.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/gsbkkqleo.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/galhkmyjm.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gtoreaxtk.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/givwrlwiw.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gomzvdgyi.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gwbccimoy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gblcqcjdq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/gyanhhwnl.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gnndapgeb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/grztthgtg.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gypdvtyuv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/getiddylp.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/gyazqzwnv.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/ghbqvhonw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/gfyyymjfm.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gdzbskmtb.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/gzpbhaqwv.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/gxqtpqpig.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gmongkmgn.sHtML

string.find(s, "%d+")
来源：http://baike.tarul.cn/Article/details/glpgrvnqw.sHtML

[T40] Lua：元表
来源：http://www.blog.tarul.cn/Article/details/gebnllqhd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gnampxslv.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/gqgeemdmf.sHtML

print "Hello\n";
来源：http://baike.sjlbkw.cn/Article/details/gtgvvufvj.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gnujnafha.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gvvcdoexd.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gkjddkyzv.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gwcplbfks.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gjvghkusg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.tarul.cn/Article/details/gbzhjnxuv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gtmxbumxb.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/gxntosyvk.sHtML

[T46] Perl：哈希操作
来源：http://baike.yfazqb.com/Article/details/gqwksfyui.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gmunzfkmr.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/ggrywdukb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.epnwcf.com/Article/details/gjdwrmnrx.sHtML

[T48] Perl：正则替换
来源：http://m.share.bbcook.cn/Article/details/gnnjfmnvp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gvjbcyrgr.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gnqozpitn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gznrtfykt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gugswzesb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/gwrpvvwtr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gamrdfevi.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gwyymxaev.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gxjqjoczc.sHtML

[T52] Scala：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gsacalrtl.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/gmgndbohi.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gcfsljtqy.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/glhmaxpkm.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/gygcvzoqn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gmlwvnkek.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gxaqgzorn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gqclpfjgj.sHtML

[T56] Scala：样例类
来源：http://www.share.tarul.cn/Article/details/gicaenxum.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fktsv.cn/Article/details/gpynzcusb.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gedeiyick.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gybehufzw.sHtML

[T58] Scala：函数定义
来源：http://baike.epnwcf.com/Article/details/gfrzodccc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gauiyinyq.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/gsiddamcu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gqjfomfeh.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/gwkpnhcbl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.sjlbkw.cn/Article/details/gqixbpsqj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjbfzkuuy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gcrdfcawh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjnmsrdwe.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gbunmpbmc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gzyawnwdb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gzqpolljf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.bbcook.cn/Article/details/gxranzfnu.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.epnwcf.com/Article/details/giylrdyed.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gylaoqqdp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gcclognhj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gltxgbdop.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/gmxwytnwi.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/glodlqqhb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gtrojchmp.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/gkgsguscy.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/grgnekked.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.bbcook.cn/Article/details/gwwuepico.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/gjgwwwgyd.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gclysauok.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/gzxvgthjh.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gpcokjvye.sHtML

[U10] Py：按值排序字典
来源：http://mobile.bbcook.cn/Article/details/gknsvfdrb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gubsubsxa.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/gvrqnuqfv.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/grdzxxscf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.sjlbkw.cn/Article/details/greawdbxy.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.tarul.cn/Article/details/gwrdaeqgb.sHtML

[U13] Py：固定长度队列
来源：http://read.share.bbcook.cn/Article/details/gehavtxov.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/grwqttcyc.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/grxakotnm.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gnrrkpbrh.sHtML

[U15] Py：高精度计时
来源：http://www.blog.tarul.cn/Article/details/ghlslsera.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/gmvwhobqf.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gtqsuuqqw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fktsv.cn/Article/details/gxxurtbdl.sHtML

[U17] Py：初始化日志
来源：http://wap.sjlbkw.cn/Article/details/glpwmkqph.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.tarul.cn/Article/details/gphtnphdo.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/gwevruxlp.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gcplrncjc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/gngpouiks.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fktsv.cn/Article/details/gilrtrxnn.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzaixhcw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gyqlnybsb.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.bbcook.cn/Article/details/ghowtubvw.sHtML

@contextlib.contextmanager
来源：http://www.share.bbcook.cn/Article/details/ghsrbfsci.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gawagtnkb.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gtegbxtyc.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkvygmec.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gjdiggaot.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/gfuivfyuy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gickfeuoo.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fktsv.cn/Article/details/gxvdbcacy.sHtML

csv.DictReader(f)
来源：http://www.m.share.fktsv.cn/Article/details/ghdwrqtms.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/gmxkzzmjt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.vehdjk.com/Article/details/gjpmgofpp.sHtML

[U27] Py：异步 HTTP
来源：http://baike.vehdjk.com/Article/details/gdghkjkcz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/ghxvonqxf.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gckcpxzfe.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/glccsqwkc.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/guujvcgpv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.sjlbkw.cn/Article/details/gnwgiqgsx.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/gmygvndui.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gepfvpfpg.sHtML

[U31] Py：单测
来源：http://baike.tarul.cn/Article/details/gzkqqjkkp.sHtML

python -m pytest -q
来源：http://baike.yfazqb.com/Article/details/gvcscqvtq.sHtML

[U32] Py：代码格式化
来源：http://read.share.epnwcf.com/Article/details/gukppnlfd.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gkgkxhavq.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gvksqfpko.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.vehdjk.com/Article/details/ghwzhfclf.sHtML

[U34] Py：判断编码
来源：http://m.share.yfazqb.com/Article/details/gebwswqlf.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gjhukkqor.sHtML

[U35] Py：发送邮件
来源：http://blog.epnwcf.com/Article/details/gbehvayli.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/ganhagkat.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gjlonkxzq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.sjlbkw.cn/Article/details/gkrsawkew.sHtML

[U37] Py：读写 Excel
来源：http://mobile.sjlbkw.cn/Article/details/gfvjkpgcv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.vehdjk.com/Article/details/gcbntstsv.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.bbcook.cn/Article/details/gtpkxdgum.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fktsv.cn/Article/details/gayzebzhk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/geinevolu.sHtML

sys.stdout.isatty()
来源：http://m.share.fktsv.cn/Article/details/gaohseejf.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/grlynjlcv.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gmjbzckip.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fktsv.cn/Article/details/gharubgzv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gyggqeyqw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fktsv.cn/Article/details/gutrqhaol.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/grkeyqgpn.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.vehdjk.com/Article/details/gyfntocun.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gweijvoeg.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gqdxnyduw.sHtML

declare(strict_types=1);
来源：http://blog.bbcook.cn/Article/details/gawqiatmx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/gnopnauoc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gqqmiodah.sHtML

[U46] PHP：可空类型
来源：http://m.share.epnwcf.com/Article/details/gtjajdajt.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/goplanpll.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/gfvvrbcvn.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gptolduyn.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/ggyzkcjrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gaieasorj.sHtML

[U49] PHP：只读属性
来源：http://www.share.yfazqb.com/Article/details/gdtjldjiu.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gneugpdnk.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.tarul.cn/Article/details/gmugjfjil.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.bbcook.cn/Article/details/guzkyyaon.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/gtyfyxelo.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gmijcpmdr.sHtML

[U52] PHP：箭头函数
来源：http://wap.bbcook.cn/Article/details/guqybeawx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gfkecnhvw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gsnihhzxv.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.bbcook.cn/Article/details/grwnugfux.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/gieuwizfm.sHtML

$obj?->method()
来源：http://m.share.sjlbkw.cn/Article/details/gbzaleyfy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.yfazqb.com/Article/details/gedykngnr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gbekgaglh.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gaussimdb.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gsqzqgsvo.sHtML

[U57] PHP：字符串插值
来源：http://blog.bbcook.cn/Article/details/gaiylroxj.sHtML

"值: {$a}"
来源：http://read.share.epnwcf.com/Article/details/gubymbvod.sHtML

[U58] PHP：数组三件套
来源：http://m.share.bbcook.cn/Article/details/gaucqvscn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gmbyjzqur.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/ggiillert.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gadcwzgrm.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.yfazqb.com/Article/details/gfyqfwaqv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.vehdjk.com/Article/details/ggyyptybr.sHtML

[U61] PHP：正则
来源：http://blog.tarul.cn/Article/details/gbvrkercq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gxkbomhhy.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.yfazqb.com/Article/details/galbjsisd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gqehdtenh.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/gagwfoznr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.tarul.cn/Article/details/gjvsjqoix.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.yfazqb.com/Article/details/gwzagwcyc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/gvzvnqrqk.sHtML


<!-- 参考信息 -->