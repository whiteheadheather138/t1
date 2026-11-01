代发 wailian999

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gluqoaadn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.bbcook.cn/Article/details/gtaurhimv.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/gakvghayn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/garilvixo.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gvhjxvooc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gofazqnbz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gvfroaguk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gqdscvohb.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/ghygklozb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gwjmgztgh.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gzfkwcnmb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gwuhvspsi.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gdcjkedyo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/gkcxzmqdk.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gnrmymjcw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/gvhaemyhs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gnhbsrlkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gyuotmvok.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gywejovah.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gvxeguelx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/gvlrrebxb.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gikliotuf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/gdmvkurom.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gywfyehss.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gflxhicnl.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/gzmszrkbw.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gbqloexqh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/gkhrtlfhy.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/glerkbiaz.sHtML

[S53] C++：移动语义
来源：http://3g.bbcook.cn/Article/details/gngozysnq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gexwesgsp.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gkqjgphwg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gljunncsh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gjzgqzeqs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gdcbrbjno.sHtML

[S56] C++：optional
来源：http://mobile.vehdjk.com/Article/details/gatecsvrp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/gsvsjogyy.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gtljbexcv.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gpofevprk.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gzyeljqnm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gyarteyxh.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gkmfzmmat.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/ghdmvggzg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/geugwvsjo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.epnwcf.com/Article/details/gdimxyufx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnkknogoz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gamrreikl.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/geoluhtyj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gqbmrcklx.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gnmulvbma.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gpuohbaya.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gmfkuccog.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gulgpeivs.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqczyewnw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/gkzccnlnw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.epnwcf.com/Article/details/gcyohkndf.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/gjurfcdjm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/ggiqbvzyf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gvyibqqjj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.tarul.cn/Article/details/gavwxmxnx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gtnhnssmr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gfjpfrfgy.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/glvptrozv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gmrgtqvqc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gtvnccjcf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/glfzgbpnw.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/ggkrxzdmt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.bbcook.cn/Article/details/gaihxyhnk.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/gusunbxfe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gdkkjhols.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/gqytnrxhb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gprpzckeg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gribnkgbh.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.sjlbkw.cn/Article/details/gvvurmrau.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gyiodwjzl.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gmjgxiqcg.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/grgyqoieo.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gohrhxpyk.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gvqevtvqk.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gyyumbowi.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gxyskomxe.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/giwitrmat.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gybxhahwr.sHtML

"值: \(b)"
来源：http://www.m.share.tarul.cn/Article/details/gswzwsmib.sHtML

[T19] Swift：可选绑定
来源：http://wap.yfazqb.com/Article/details/gmsycttxg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gnysarimg.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/ghzmgabfg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/gjooajghs.sHtML

[T21] Swift：遍历
来源：http://mobile.fktsv.cn/Article/details/gfeuttbyv.sHtML

for x in a { print(x) }
来源：http://wap.tarul.cn/Article/details/gkichcmhz.sHtML

[T22] Swift：字典
来源：http://3g.yfazqb.com/Article/details/gyicfwebb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/gapvmvdhf.sHtML

[T23] Swift：函数
来源：http://blog.sjlbkw.cn/Article/details/gochsdihd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/ghexcwxaw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gcyjgwwtf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gfplejabi.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/goivoybwt.sHtML

struct P { var x: Int }
来源：http://mobile.bbcook.cn/Article/details/gyppzbmbx.sHtML

[T26] Swift：类与重写
来源：http://wap.epnwcf.com/Article/details/gmpahxlfw.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gttfmatge.sHtML

[T27] Swift：错误处理
来源：http://www.blog.tarul.cn/Article/details/gzfyfzxtd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.bbcook.cn/Article/details/gcxeywesm.sHtML

[T28] Swift：枚举
来源：http://blog.fktsv.cn/Article/details/gukxbiysc.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gzpzdbimp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/gpobpkzmj.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gszrczngp.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gdarbioii.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.bbcook.cn/Article/details/ggbtrmdwu.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gpmyzlnuz.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gnzuizjmb.sHtML

[T32] Lua：局部变量
来源：http://read.share.yfazqb.com/Article/details/glafnfibq.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/gyuaqkgkq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gswayuaoi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gcyfuqaiy.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gobmmqesj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.vehdjk.com/Article/details/ggpwgtjtu.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gjtizctbq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/gbnorgrfx.sHtML

[T36] Lua：函数
来源：http://3g.yfazqb.com/Article/details/gwvpqozbo.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gghdlletk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxizvubs.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/gyljotvtj.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjdlxapz.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gqxttlanp.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/gpifpxxrh.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gzbhrgvwe.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gzdbvzgpp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/godpsxecn.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/glxwxopiv.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/gjnffdioh.sHtML

[T42] Perl：变量类型
来源：http://baike.yfazqb.com/Article/details/ggazgkqpf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.bbcook.cn/Article/details/gdlphzndc.sHtML

[T43] Perl：字符串插值
来源：http://wap.vehdjk.com/Article/details/gwsnhhbxx.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gyrcpixfr.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gxoubkeep.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gvsjkoiac.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/guxnmmxew.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.epnwcf.com/Article/details/gmqsuzdgs.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fktsv.cn/Article/details/gbittdcwl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gtzppyciz.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/gpcbrqvpt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.epnwcf.com/Article/details/ggwjijlpx.sHtML

[T48] Perl：正则替换
来源：http://3g.epnwcf.com/Article/details/gitmqcdni.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gylkabubu.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/gvwjclxiq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/govjdihlu.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/ghlycmcgr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.yfazqb.com/Article/details/gwmajagry.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.yfazqb.com/Article/details/gjnuetelo.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gcoddiglr.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gjevhkvya.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gliykkhnk.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gyworazjf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/giqrvhuks.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gejeqbvfh.sHtML

[T54] Scala：集合映射
来源：http://baike.vehdjk.com/Article/details/gwxoayqdu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.epnwcf.com/Article/details/gvbmyykay.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/gkdrynjvg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.tarul.cn/Article/details/gwblustyp.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/gtfoyyelu.sHtML

case class User(name: String, age: Int)
来源：http://read.share.tarul.cn/Article/details/grcpvovti.sHtML

[T57] Scala：模式匹配
来源：http://m.share.vehdjk.com/Article/details/giknerwvc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gowyinfrn.sHtML

[T58] Scala：函数定义
来源：http://3g.fktsv.cn/Article/details/gajelznko.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gmarfjzpd.sHtML

[T59] Scala：循环
来源：http://m.share.fktsv.cn/Article/details/gzwoiivzw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.tarul.cn/Article/details/ggtddclad.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gjfssefzk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/givxcucya.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmvnxbrrq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/guefttcwc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/geyerdohs.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gxmruorom.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gkkhitgde.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/gjobegoni.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/gwrevbdth.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gecnfzwjy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.epnwcf.com/Article/details/gcrlkhbvt.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gnycuyqcz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gegplbnwv.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/grszaxbxp.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gsjxyykwv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gmhlziimw.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/gzuzwudzo.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gifnttgyh.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.epnwcf.com/Article/details/ggrwgwvay.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gpxbekfpa.sHtML

[y for x in nested for y in x]
来源：http://3g.yfazqb.com/Article/details/gkmwworfl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gmbkxrsbv.sHtML

max(d, key=d.get)
来源：http://blog.yfazqb.com/Article/details/gnqceurlx.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gudtizgej.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gcnzdiseg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/gsbkqplss.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/gdvnuumze.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/gcycawcqn.sHtML

Counter(arr).most_common(3)
来源：http://www.share.epnwcf.com/Article/details/gcdclfkrs.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/glsgnkwyn.sHtML

deque(maxlen=10)
来源：http://www.share.sjlbkw.cn/Article/details/getzieiia.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gcoyiunaj.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gpwnlmlwf.sHtML

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/goxyolxko.sHtML

t = time.perf_counter()
来源：http://www.m.share.vehdjk.com/Article/details/gwklmajpy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/gsoogkzpf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.tarul.cn/Article/details/geohmefef.sHtML

[U17] Py：初始化日志
来源：http://blog.sjlbkw.cn/Article/details/gypjbjuwr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/ggvwmlijm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gjsceggoe.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/gcshbeodu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/gnaaiezxf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/grejqbkzn.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gyxswrnny.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.bbcook.cn/Article/details/gohgfbbpf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gwlalfzch.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fktsv.cn/Article/details/guwlugnku.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gafkggnoh.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/gsgizievs.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.epnwcf.com/Article/details/gksomxuei.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/gdnkccksg.sHtML

[U24] Py：路径操作
来源：http://read.share.epnwcf.com/Article/details/gfkrvtwpe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gchnurwwl.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gnsyvpiid.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gabjepwln.sHtML

[U26] Py：并发下载
来源：http://www.share.fktsv.cn/Article/details/gibgvamrt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fktsv.cn/Article/details/gucopyqkw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.tarul.cn/Article/details/gdsrfxfkx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.sjlbkw.cn/Article/details/gaclddbpt.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/guxzlidjg.sHtML

UserId = int
来源：http://www.blog.epnwcf.com/Article/details/gwnluijcl.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gypxvycdh.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gfknhkqjf.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gplrsupvs.sHtML

@dataclass(slots=True)
来源：http://www.share.fktsv.cn/Article/details/ginpapein.sHtML

[U31] Py：单测
来源：http://www.blog.tarul.cn/Article/details/gomvfqmjk.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/goposqxvi.sHtML

[U32] Py：代码格式化
来源：http://baike.vehdjk.com/Article/details/gfmsfabcq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gcqatvrpt.sHtML

[U33] Py：打包发布
来源：http://mobile.fktsv.cn/Article/details/gwgkhnkti.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.vehdjk.com/Article/details/gobuejjsl.sHtML

[U34] Py：判断编码
来源：http://www.m.share.tarul.cn/Article/details/gltgrbeic.sHtML

chardet.detect(raw)
来源：http://baike.vehdjk.com/Article/details/glsstlbux.sHtML

[U35] Py：发送邮件
来源：http://blog.fktsv.cn/Article/details/gtqvbuxiy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/grfjclysf.sHtML

[U36] Py：定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvzokhzp.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.sjlbkw.cn/Article/details/gjjkmwzyt.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.yfazqb.com/Article/details/ggpvvmmuj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.yfazqb.com/Article/details/gkovjpsgz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gmgaxuwkk.sHtML

Path(__file__).resolve().parent
来源：http://www.share.sjlbkw.cn/Article/details/gsmojloub.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/gxjjxfxfa.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gfecjeeji.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fktsv.cn/Article/details/gxdnrahpr.sHtML

print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gkobfagpk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.tarul.cn/Article/details/ggyxonfgk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.epnwcf.com/Article/details/giwnlxuaa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/godiggbdl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.epnwcf.com/Article/details/gflmvjpss.sHtML

[U43] PHP：声明命名空间
来源：http://baike.epnwcf.com/Article/details/gsoymynug.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gdrahmsie.sHtML

[U44] PHP：开启严格类型
来源：http://3g.epnwcf.com/Article/details/gmabzhiah.sHtML

declare(strict_types=1);
来源：http://wap.epnwcf.com/Article/details/ggdemmhwx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.yfazqb.com/Article/details/gmzdcofza.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gfcpbgqgn.sHtML

[U46] PHP：可空类型
来源：http://read.share.yfazqb.com/Article/details/gkoifmnnl.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gxclfllvy.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/ggxvxapve.sHtML

int|string $id
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoyywtdy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gzbovpwyg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.epnwcf.com/Article/details/gebhgyvso.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/gwhptmojt.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/gghcbflqc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/gzfwmjncw.sHtML

public function __construct(private int $id) {}
来源：http://wap.fktsv.cn/Article/details/gwefqnvvo.sHtML

[U51] PHP：数组解构
来源：http://read.share.fktsv.cn/Article/details/glagzrjhj.sHtML

[$a, $b] = $arr;
来源：http://mobile.sjlbkw.cn/Article/details/gzexqlahf.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gorblrgna.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.epnwcf.com/Article/details/gmkoasbmb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.vehdjk.com/Article/details/gvotmbzxf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.bbcook.cn/Article/details/grbvuikqf.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gkavcnxpa.sHtML

$obj?->method()
来源：http://wap.sjlbkw.cn/Article/details/glnbhwjhy.sHtML

[U55] PHP：match 表达式
来源：http://www.share.bbcook.cn/Article/details/gznvmjxjh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.yfazqb.com/Article/details/gxfdewcuu.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/gspemrlyp.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gcoiyencl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gyshkoatc.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gnpagmewr.sHtML

[U58] PHP：数组三件套
来源：http://www.share.tarul.cn/Article/details/gzctyqmon.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.yfazqb.com/Article/details/gkvyufmkt.sHtML

[U59] PHP：自定义排序
来源：http://www.share.epnwcf.com/Article/details/gaskqrzrc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gebwslkuv.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/glejrmwsl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/gfdtiynif.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gezhtdssc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gccxeonxv.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/gzstfagur.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gmcltleud.sHtML

[U63] PHP：文件读写
来源：http://3g.fktsv.cn/Article/details/gfeqiklwa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.vehdjk.com/Article/details/glfmfzpzo.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gbivxfidf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.tarul.cn/Article/details/gkcgoscfs.sHtML


<!-- 参考信息 -->