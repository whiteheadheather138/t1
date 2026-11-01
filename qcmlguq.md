代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gkeftbdsy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/ghcsnfqtu.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gvajtsxxy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/gijghiefw.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gcxszxomr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gaaorhtht.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gumbtcvkk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.sjlbkw.cn/Article/details/gavoumiqv.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gxilbovkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gsgjquqft.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/ghajoaizr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gvrmzsbwo.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gxppvqksq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gixvkepuc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/geqdhzqai.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gykmvjmfx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/gceyhasvb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gdbaiuuze.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gssqrrgiq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gncqdmqzt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gcppnoxwa.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/girnzhnrt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gxtjddqai.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gwzgtaouj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gfdhwwrve.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gemzqpjgx.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gsdyaorxn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/goxylrwwk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gclecysga.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gyhktordc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/grbptkpqf.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gmghxcatu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.yfazqb.com/Article/details/glbslqmfy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/gvfehmury.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.bbcook.cn/Article/details/gcsacdrgf.sHtML

[S56] C++：optional
来源：http://www.share.yfazqb.com/Article/details/glxyjbiwf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/gyoinkeef.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gyoablyqb.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gysijpcex.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gndvrobep.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gsbvpocwq.sHtML

[S59] C++：静态断言
来源：http://mobile.bbcook.cn/Article/details/gennpetun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.epnwcf.com/Article/details/ghthlcdnr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gbdcqlewp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gsfojsuou.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvpcqtwgp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/geueefuua.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfjfqpbrf.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/graaxwwxd.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gesadwshp.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gxyrfioow.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gwhvttald.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/guyqqyznv.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gnmprvshv.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/gmjudexwa.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gfcbvrpvr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gooogsqhz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gqihzgviq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/glcnkrxot.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fktsv.cn/Article/details/gvjeixnzk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.epnwcf.com/Article/details/gvzqfjqzx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gvfpmnsit.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/gtdapdgij.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/ghfcplzdb.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gsvbtpyyv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/gzsnkdpus.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gyulkaufb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.yfazqb.com/Article/details/gzcrxzjsi.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gczmudinh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gduslsjyt.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gotazvjjl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gtiqadbop.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/ghoswxank.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fktsv.cn/Article/details/gcpplvszz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpsejmsq.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gabqebjcu.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/ghxajfhzl.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/guuzoupll.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gbhtotyrg.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gmcgrnief.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gxknpndsa.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/grvbbtdet.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gpfaxrmay.sHtML

"值: \(b)"
来源：http://mobile.vehdjk.com/Article/details/gsijqunrg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/ggkwzltau.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/gfeewwqzy.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gdhshopcy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gcnvnrqui.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/gathofnhi.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/ghjbrihjk.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gvboqiest.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gprscrvxg.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/gregkyrjb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/ghdfcsgju.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gawwigimj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/glsloihzo.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/garnkresd.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gyqypksih.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/ghbekxsli.sHtML

class A: Base { override func f() {} }
来源：http://mobile.sjlbkw.cn/Article/details/gjlpmunqi.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gzgiwnefh.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/godojgswx.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gbkwfviwp.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/geszjitvq.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.sjlbkw.cn/Article/details/gqjjcepyk.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gbpjehqrh.sHtML

[T30] Swift：协议
来源：http://blog.yfazqb.com/Article/details/guoyulymc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.epnwcf.com/Article/details/gbyrtknob.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gynncwdlp.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gmpjqoxcz.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/gifvmccve.sHtML

local a = 1
来源：http://3g.sjlbkw.cn/Article/details/gtundgrma.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gewvhtljr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.bbcook.cn/Article/details/gcbxnhttq.sHtML

[T34] Lua：遍历表
来源：http://baike.bbcook.cn/Article/details/giqwhcvaq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/gnbtvujoh.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gamhmsnud.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.bbcook.cn/Article/details/gateabmxb.sHtML

[T36] Lua：函数
来源：http://blog.bbcook.cn/Article/details/gyckkqzry.sHtML

function add(a, b) return a + b end
来源：http://3g.yfazqb.com/Article/details/gpkxzcdkc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gomitouak.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gcydwpysz.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/glazwqqgi.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/gdwkyzuve.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/goseeganh.sHtML

string.find(s, "%d+")
来源：http://mobile.fktsv.cn/Article/details/gdxojkyhs.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/gvlvqsuri.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gfxdggick.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ghvkyhskk.sHtML

print "Hello\n";
来源：http://mobile.tarul.cn/Article/details/gcevdxevn.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/ghpzkouyl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/ggdcreizh.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gbtpefibv.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/gxfdglljf.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/ggfxgzgfo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gawccdesp.sHtML

[T45] Perl：数组遍历
来源：http://wap.fktsv.cn/Article/details/gpnfnotsd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/gsochinng.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gqwjyifnv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gjgvtwndh.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gkixykkek.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gcskxdvqq.sHtML

[T48] Perl：正则替换
来源：http://3g.bbcook.cn/Article/details/galazqyub.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fktsv.cn/Article/details/gbcbrdnyq.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/guzdnxmlq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gchgorvqy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gyxtesomv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/gyajhxwcp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.yfazqb.com/Article/details/gupqmnnpj.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gseweehum.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gdlohvhxa.sHtML

[T52] Scala：变量
来源：http://www.m.share.epnwcf.com/Article/details/grpufhqih.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gfmcmdxqy.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/graadbfoq.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gijseyorr.sHtML

[T54] Scala：集合映射
来源：http://wap.epnwcf.com/Article/details/gkkvqclmk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/guqqldvjm.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/gjsoplqex.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.yfazqb.com/Article/details/gvzmkoswh.sHtML

[T56] Scala：样例类
来源：http://wap.fktsv.cn/Article/details/glmxywmdj.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/guzicipul.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/giunxlkug.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gbwxyrlag.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/gntxzinpt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.epnwcf.com/Article/details/goanuosss.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gjbwqxojf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/gtivzzjad.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gcgasjytr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/gmmmruwlw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gafoxwzlw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gazvxiyfn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqhltwvgr.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gvrfhdtox.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/gzylyxivl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.bbcook.cn/Article/details/gsfaqrnna.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gohjflhfo.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/ghkiloqrg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gfymcllal.sHtML

[U04] Py：变量调试打印
来源：http://mobile.sjlbkw.cn/Article/details/glwvvkdry.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlocapuv.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.bbcook.cn/Article/details/gvtijrijj.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/guzsmdgvb.sHtML

[U06] Py：合并两个字典
来源：http://m.share.vehdjk.com/Article/details/gxefdwphy.sHtML

{**a, **b}
来源：http://www.share.vehdjk.com/Article/details/gwuwvqzha.sHtML

[U07] Py：反转字典键值
来源：http://www.share.epnwcf.com/Article/details/gmllkzchu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/ggjnshljj.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/gcemfuoow.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/ggeqtfmbw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/gdcxxgtsj.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/gdxzxduub.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/gvatbexbd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/gmuqznzet.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gyfvoyaoj.sHtML

(x * 2 for x in arr)
来源：http://blog.vehdjk.com/Article/details/gxfjaptvs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gnqntldyx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gslioazfp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/ghqaxdtsg.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gvytoukjn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gtlnddzoy.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gnbqvxhcw.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.tarul.cn/Article/details/gcljwgdpz.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/ggwqhomnw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gfikfxiim.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/gjjsrmqbv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.bbcook.cn/Article/details/gansjdpng.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.yfazqb.com/Article/details/gsowngbke.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gcprrngdo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gqrctbssa.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/gdgyxswjb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/geblnehlt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.yfazqb.com/Article/details/gwphvugxv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gircktkzg.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.sjlbkw.cn/Article/details/gulqnexrj.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gjlsiesup.sHtML

[U22] Py：矩阵转置
来源：http://wap.fktsv.cn/Article/details/gyijtahvm.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gvgyepfzk.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/grpwrdcgl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.yfazqb.com/Article/details/gltojvcea.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gvhsodkfx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/grhaziafb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gjzzuiiir.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gtxruumgi.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/ghvryviyq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.tarul.cn/Article/details/gvsqlloal.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gvictdbkq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.tarul.cn/Article/details/gapctbdsp.sHtML

[U28] Py：类型别名
来源：http://3g.fktsv.cn/Article/details/gvoghahwv.sHtML

UserId = int
来源：http://blog.tarul.cn/Article/details/gowckqhml.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gxjftrnzn.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/gungbttco.sHtML

[U30] Py：数据类
来源：http://www.blog.epnwcf.com/Article/details/gnyvtlrzh.sHtML

@dataclass(slots=True)
来源：http://baike.sjlbkw.cn/Article/details/ghgjtuims.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gbpvtfyfn.sHtML

python -m pytest -q
来源：http://3g.yfazqb.com/Article/details/gbgykkbcg.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/ggvvvcnsi.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.tarul.cn/Article/details/gqayaanib.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gzftvlpyq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gryvecwuc.sHtML

[U34] Py：判断编码
来源：http://www.blog.bbcook.cn/Article/details/grqnpximz.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/gwkrjjjsu.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/gzttyuczj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.epnwcf.com/Article/details/gqdogwvpv.sHtML

[U36] Py：定时任务
来源：http://www.share.vehdjk.com/Article/details/gzwdxglup.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.vehdjk.com/Article/details/guiipqexu.sHtML

[U37] Py：读写 Excel
来源：http://baike.yfazqb.com/Article/details/guhhbwziy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fktsv.cn/Article/details/gbohodujt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.bbcook.cn/Article/details/gvckhmfol.sHtML

Path(__file__).resolve().parent
来源：http://baike.vehdjk.com/Article/details/gsmcnjxoe.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/goxgnluzm.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/gzuhtxcfw.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fktsv.cn/Article/details/gngjyvttn.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gfibycnxz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/gxftyzmps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fktsv.cn/Article/details/goiuwqvrf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.tarul.cn/Article/details/gzuylwxau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.sjlbkw.cn/Article/details/georetgvm.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.vehdjk.com/Article/details/gibqgbgbn.sHtML

namespace App\Http;
来源：http://wap.bbcook.cn/Article/details/gmptodllr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/gazclqmpi.sHtML

declare(strict_types=1);
来源：http://blog.bbcook.cn/Article/details/govkokjub.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.vehdjk.com/Article/details/gbqhymvbn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gruiieybe.sHtML

[U46] PHP：可空类型
来源：http://wap.bbcook.cn/Article/details/gnysznurr.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/ghzocnemd.sHtML

[U47] PHP：联合类型
来源：http://m.share.fktsv.cn/Article/details/ghuaojhhz.sHtML

int|string $id
来源：http://mobile.fktsv.cn/Article/details/gluessszn.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gcmhuuznf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gjiigodun.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gbowdcgyd.sHtML

public readonly string $name
来源：http://wap.bbcook.cn/Article/details/gcqaxtlip.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/ggnrsahdq.sHtML

public function __construct(private int $id) {}
来源：http://read.share.yfazqb.com/Article/details/gvhkcuuot.sHtML

[U51] PHP：数组解构
来源：http://www.blog.yfazqb.com/Article/details/gwigzjtvg.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gemqvigdh.sHtML

[U52] PHP：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gcntonekk.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/gnnjbkpwo.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/gsdnsqjjq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gjcbufvrq.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gqlfqieaf.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gxrjrnvek.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fktsv.cn/Article/details/gwpbgpgji.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.bbcook.cn/Article/details/geoupcfyj.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/ggfawnxfp.sHtML

f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gnqlbbyxl.sHtML

[U57] PHP：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gxjksnauo.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/ggswjxpov.sHtML

[U58] PHP：数组三件套
来源：http://www.share.tarul.cn/Article/details/gveztbgwb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/ghiolcnuw.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/givlnduzi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gycshjchx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fktsv.cn/Article/details/gqtpnsfty.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gzkbcpzsp.sHtML

[U61] PHP：正则
来源：http://3g.epnwcf.com/Article/details/gpjubfzok.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gxepiwtfp.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gikqigxlr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gyilhsves.sHtML

[U63] PHP：文件读写
来源：http://mobile.epnwcf.com/Article/details/gevyojfvv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/gidfzxoon.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/giyotuikr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/gedzwryoy.sHtML


<!-- 参考信息 -->