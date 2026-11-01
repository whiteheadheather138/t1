代发 wailian999

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gokhoyvci.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/geifmtfnn.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/grzmveznv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gjqyywwpx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gvohsoggo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gwpfxzkuz.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.vehdjk.com/Article/details/galdjmgai.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/gxgdxtwch.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/guiyizniu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gigrfhddt.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gthheehca.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gzgjzemjj.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gqkfxqeqa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/gesaihylq.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gjemsybes.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/guugeyvgw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/guvselmyt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/ggmfetlhg.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gxbeeoghz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gcrrnpbyi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gbdzgytat.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gnbsqywbp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrwdkhui.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gpmstjpjn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/goawqlsph.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gjhxzvujs.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gnryplsgb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.tarul.cn/Article/details/gyojzctyc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gwoaalzdl.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/giakmfyqr.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gyyraazug.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gbnrvblel.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gnpqsrtwe.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gphpobvtk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.yfazqb.com/Article/details/giavhmptx.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/ggeyiohug.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/ghaixttvr.sHtML

[S57] C++：编译期常量
来源：http://wap.sjlbkw.cn/Article/details/ghmnscqeq.sHtML

constexpr int N = 10;
来源：http://m.share.bbcook.cn/Article/details/gmawglbry.sHtML

[S58] C++：命名空间
来源：http://3g.yfazqb.com/Article/details/gftlkfurt.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.epnwcf.com/Article/details/gfmpbwohr.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gmpcjfagg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gwhrppmzc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.yfazqb.com/Article/details/grpzoypus.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gwjdcqdre.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghgzdjime.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gazhyhfxv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmxwacdyx.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gdvnbrtok.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gylogmllz.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gzfnjyunl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.tarul.cn/Article/details/gmtisonqt.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/glsmwaadn.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gayugwytq.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/giulhtqgk.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gpfuiykrn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.sjlbkw.cn/Article/details/gciqhqstu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/gcskyedlg.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/glewoifez.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gfgclxldr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gkcfwzbeg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/ggogxjkxn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.epnwcf.com/Article/details/gtetlyvnn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gbcoyivtm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gbgrmnubf.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/gsbudmhku.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gqehgjikl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gnumojkiz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.tarul.cn/Article/details/gdfljrthu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/gwxzsosbp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gqfcgqudn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/ggtndszlm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.yfazqb.com/Article/details/guhgzxdog.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/ghzjsaaxd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fktsv.cn/Article/details/goiltntzk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/grggfpnni.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/gsrumbubf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gyjqdwtes.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gcvkcwxrd.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/grajhvrkr.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/galtxasab.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gptnvrmat.sHtML

[T18] Swift：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gfdjmldsv.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/gogquceym.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.yfazqb.com/Article/details/gxyaivrin.sHtML

if let n = opt { print(n) }
来源：http://baike.epnwcf.com/Article/details/gxequvidl.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gxkphueyk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/gwwsukkgj.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/ggiaiymdr.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/grfcvvqnu.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/gmyjczztv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gcwjnotlw.sHtML

[T23] Swift：函数
来源：http://wap.epnwcf.com/Article/details/gnidwlwpt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/goezwgjgu.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/ggzbldmxg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.epnwcf.com/Article/details/gjnlwofwy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/gxhvbkxqj.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gqnxilqjj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gpxhlsztc.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gpxeaxvqr.sHtML

[T27] Swift：错误处理
来源：http://wap.bbcook.cn/Article/details/gqdmpzfgg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gksbchoyk.sHtML

[T28] Swift：枚举
来源：http://read.share.tarul.cn/Article/details/gqeytwode.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gdynitqeq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/grxthspvs.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/gsjihzxgs.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gyjcenkoe.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gbpoevege.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/ggttriyvp.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/guncylorc.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gelysphfh.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gumjxmclu.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/glokvbdpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gauhuuupk.sHtML

[T34] Lua：遍历表
来源：http://www.share.bbcook.cn/Article/details/getvfhbmo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/gpxbcnatx.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/ggxnxspxk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gsymjkigx.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gdxkrujtp.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gvwzdgagf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/gwpkrbppl.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gvdbsqaxr.sHtML

[T38] Lua：条件
来源：http://www.m.share.epnwcf.com/Article/details/gztrlhwnz.sHtML

if x > 0 then print("正") end
来源：http://www.share.epnwcf.com/Article/details/gxhchughf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/grpqntqml.sHtML

string.find(s, "%d+")
来源：http://mobile.vehdjk.com/Article/details/gjpcbalbe.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gmgnxnhwj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gfgxmcbwl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gytucsycj.sHtML

print "Hello\n";
来源：http://blog.epnwcf.com/Article/details/gytrdaaju.sHtML

[T42] Perl：变量类型
来源：http://3g.yfazqb.com/Article/details/gfeqzwumw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.yfazqb.com/Article/details/gorpqdpzc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/ggorgebfe.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gorpsdglp.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gyjewigha.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.vehdjk.com/Article/details/gdyujfzwj.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gvvvgweqg.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gdludferw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.yfazqb.com/Article/details/giigkqjxl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gmwoqscce.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gdtvepzzx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gdztykjjq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbgzqask.sHtML

$s =~ s/old/new/g;
来源：http://www.share.tarul.cn/Article/details/gksuxoqwf.sHtML

[T49] Perl：函数
来源：http://3g.bbcook.cn/Article/details/gtheimjyq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gpyuiunxn.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gjkcilhsk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/gxuacmneh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gzougndro.sHtML

[T51] Scala：Hello World
来源：http://baike.fktsv.cn/Article/details/gghdfuyxa.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gmaqmayut.sHtML

[T52] Scala：变量
来源：http://3g.vehdjk.com/Article/details/gesuspksh.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/guxjsisif.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gavtyiiqh.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/gstktkrtx.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gxjkgqzdv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/goddrdwrq.sHtML

[T55] Scala：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gfkewwpaw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gparvafvk.sHtML

[T56] Scala：样例类
来源：http://www.blog.bbcook.cn/Article/details/gddivbfox.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gtaofexkh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gltmgihle.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gousivfcw.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gqkrhfjio.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gkmkfllza.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gugioliho.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.bbcook.cn/Article/details/gagsbgglt.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/gfifjhyha.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gtqjximby.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grxphgauf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/gymdgqeni.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnhpfqps.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fktsv.cn/Article/details/gfqxeltgq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gfqflzbsr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gnepnfmhl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fktsv.cn/Article/details/gfydvkzya.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.epnwcf.com/Article/details/grfwjcoww.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gorpxnvlq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gdrgkymsr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.sjlbkw.cn/Article/details/gxaamvvqp.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gpxyxkbej.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gljjuwvph.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gjuxirxed.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gsljyrboh.sHtML

[U07] Py：反转字典键值
来源：http://baike.yfazqb.com/Article/details/glwnhjqlk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gzakmtyyk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.yfazqb.com/Article/details/gmsyzsujm.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/gvdyywvjr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gcecgynxw.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/genbprggr.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gscnwsjpx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/geqzpglok.sHtML

[U11] Py：生成器表达式
来源：http://3g.sjlbkw.cn/Article/details/glzviugsn.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/gxlixcmgw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.sjlbkw.cn/Article/details/ghgitdiqx.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gqmvurqby.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/gzvfdtwiz.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/gumtdmsml.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gnksexpju.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/grcfbgzkg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/gqjbsajxn.sHtML

t = time.perf_counter()
来源：http://m.share.epnwcf.com/Article/details/gfvfivpxa.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gcqgrrigs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gptvljfgd.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gdvjqqknj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gnsnyqnui.sHtML

[U18] Py：预编译正则
来源：http://www.share.tarul.cn/Article/details/gvamqcbcr.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/gdhkxxfck.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/grkirlffu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.sjlbkw.cn/Article/details/gznzpwint.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/gqqllsvkh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.tarul.cn/Article/details/gztwvndzz.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gmibmddur.sHtML

@contextlib.contextmanager
来源：http://www.m.share.vehdjk.com/Article/details/gpwrshjoq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fktsv.cn/Article/details/gzdsppmyk.sHtML

list(zip(*m))
来源：http://blog.yfazqb.com/Article/details/guerbpkbs.sHtML

[U23] Py：分块读取大文件
来源：http://wap.sjlbkw.cn/Article/details/gpjgmhmyv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gpunsxgxd.sHtML

[U24] Py：路径操作
来源：http://blog.yfazqb.com/Article/details/gsunmuwsa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gugqnqhyo.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.epnwcf.com/Article/details/gnmtiryru.sHtML

csv.DictReader(f)
来源：http://wap.yfazqb.com/Article/details/goiacboza.sHtML

[U26] Py：并发下载
来源：http://www.blog.fktsv.cn/Article/details/gukvidmie.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/geehrjtul.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gthyqdyrs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.bbcook.cn/Article/details/gywavsnlj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/gblmtpxqd.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/gorruudfh.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/ganmeuyzz.sHtML

@property 与 @x.setter 配合
来源：http://3g.vehdjk.com/Article/details/gumhsrest.sHtML

[U30] Py：数据类
来源：http://baike.yfazqb.com/Article/details/gdlyzvitp.sHtML

@dataclass(slots=True)
来源：http://www.share.sjlbkw.cn/Article/details/gbdcvgmik.sHtML

[U31] Py：单测
来源：http://mobile.bbcook.cn/Article/details/gohjvhvxl.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/ggleadoah.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/guiteulvo.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.sjlbkw.cn/Article/details/gryrgnhvl.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/gxnmogste.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.vehdjk.com/Article/details/grvixujnu.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/gwsosxvbz.sHtML

chardet.detect(raw)
来源：http://read.share.fktsv.cn/Article/details/gbxczofyg.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gccsxgmph.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.bbcook.cn/Article/details/gxezvwmlh.sHtML

[U36] Py：定时任务
来源：http://m.share.epnwcf.com/Article/details/gvecfwnjo.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gscxswcvl.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/geiaypknv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gdivhuvuy.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.sjlbkw.cn/Article/details/gowmiujjr.sHtML

Path(__file__).resolve().parent
来源：http://m.share.vehdjk.com/Article/details/gyandlbcv.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.epnwcf.com/Article/details/gbwgzgosb.sHtML

sys.stdout.isatty()
来源：http://www.blog.bbcook.cn/Article/details/gtrcheyvy.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/gcblqymin.sHtML

print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gzqfxiisg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/gfnysedro.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gloomfabw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.yfazqb.com/Article/details/gjkeqfxwn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fktsv.cn/Article/details/gsxhjmhwv.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/gkgloatix.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gtntqkznx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.bbcook.cn/Article/details/gqdggvrob.sHtML

declare(strict_types=1);
来源：http://m.share.tarul.cn/Article/details/gflvesxic.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.sjlbkw.cn/Article/details/gymooatlx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/grozufopk.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gbbrsvppj.sHtML

?string $name = null
来源：http://www.blog.bbcook.cn/Article/details/gruytccqz.sHtML

[U47] PHP：联合类型
来源：http://m.share.epnwcf.com/Article/details/gmkosuugl.sHtML

int|string $id
来源：http://www.blog.vehdjk.com/Article/details/gezmucqcj.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/ggzsxsehn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gfjhvraft.sHtML

[U49] PHP：只读属性
来源：http://wap.yfazqb.com/Article/details/gmqserwft.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gacnpcjda.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.tarul.cn/Article/details/gydemxvwk.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.tarul.cn/Article/details/gjvkyhvfx.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gdcqbxeny.sHtML

[$a, $b] = $arr;
来源：http://3g.fktsv.cn/Article/details/glauamqfr.sHtML

[U52] PHP：箭头函数
来源：http://read.share.tarul.cn/Article/details/gbcllscks.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fktsv.cn/Article/details/gjzrkcjts.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.sjlbkw.cn/Article/details/glwpwkzwl.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/grgjxtqbo.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/gdqrlmwel.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/gitooqtzw.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/ghslqqjsn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/gwhfugsbo.sHtML

[U56] PHP：命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gyqlqznsw.sHtML

f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gwzntkpzi.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gfunoqjul.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/giqciovup.sHtML

[U58] PHP：数组三件套
来源：http://blog.bbcook.cn/Article/details/gmmoaaqvo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.bbcook.cn/Article/details/geadmytip.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/ggjxujdhu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gpjoagutg.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.bbcook.cn/Article/details/gprmqmspc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.vehdjk.com/Article/details/ggcfkonkg.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/gweecznvc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/geaztcqfu.sHtML

[U62] PHP：日期对象
来源：http://mobile.sjlbkw.cn/Article/details/giehzlbsb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gsehmhkwt.sHtML

[U63] PHP：文件读写
来源：http://www.share.bbcook.cn/Article/details/gqukibmht.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.bbcook.cn/Article/details/gahqnqfpj.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gpkjkhuam.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/gabtcjagm.sHtML


<!-- 参考信息 -->