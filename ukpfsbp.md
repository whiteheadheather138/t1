代发 wailian999

[S43] C++：智能指针
来源：http://wap.sjlbkw.cn/Article/details/ghtqdwcoe.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gdeifgtmg.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gbqsnrdzv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gjrbvuwga.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gygtlwarz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gsouehggr.sHtML

[S46] C++：函数模板
来源：http://www.share.sjlbkw.cn/Article/details/grxqxvwub.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.epnwcf.com/Article/details/gvdgztpnu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gpibiaejg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gqrxuqvih.sHtML

[S48] C++：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gycylssnh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gncqsqfju.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gnkkwnsay.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gbkwpdrsn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.tarul.cn/Article/details/gcdkbcmkm.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gukftwnqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gxnzmtzgl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gdspciwdm.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/gowqfpqjp.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gygtepalb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gpozmeqia.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gyfpyphvg.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gvhmqbuoo.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/gdjxjjfmz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/ghbahoikz.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gckeyeguo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/goilgaokn.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/govvsimam.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/ghjnrgixh.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gdduxmwiw.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gadyxapys.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/gtiwjpmkj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gjmiejdcr.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gawegzwla.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.tarul.cn/Article/details/grsdbzngl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gjkevpakz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.bbcook.cn/Article/details/gyiiubzef.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gglmvidwn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gmzwmlngr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grdvbkhfo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gihvjihcl.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/ghhulqqho.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/gzrqdnrbg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.yfazqb.com/Article/details/gzzacuaxk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gqqtqtjct.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gwujbthjm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/gaiiivbxe.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/gncpmpneo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.yfazqb.com/Article/details/gdtavdffv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gxhednxxt.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/guxuwxyjw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.tarul.cn/Article/details/grqugpuid.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gzhlijwrh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gacwhskdc.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gwucadoih.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbrqvqej.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gcqedbkrn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/gqagkfizg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.vehdjk.com/Article/details/gxeypiucw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gpiacentr.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gplczemxw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gtrpmvufl.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gnsjmwwmw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gbqwampkz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/gggcdomub.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/gmdklgiqc.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gvqsikrfx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.tarul.cn/Article/details/gmrzgkkmk.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gvzciizax.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/geiejgpgz.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gojbexjgz.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gykrtmalm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gvykkxixy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/godbjdalm.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/gidgcmzup.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gvwhdfgvl.sHtML

[T19] Swift：可选绑定
来源：http://wap.yfazqb.com/Article/details/gwekzygjj.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/grzstkeol.sHtML

[T20] Swift：数组操作
来源：http://blog.bbcook.cn/Article/details/gcucxjekn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gujzeusqp.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gguicspdz.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/goeujsioq.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gdeklmucq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gqhygcxst.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/gfbdkndzn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.yfazqb.com/Article/details/glsekjzsz.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/glfbehueg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gyqkctket.sHtML

[T25] Swift：结构体
来源：http://mobile.yfazqb.com/Article/details/gztahpcgp.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/gbzjrdebe.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/gvefynkmg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gmjbwwttu.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/gginktyfv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.sjlbkw.cn/Article/details/gataymvdw.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gqlunajly.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gyjtvouaf.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gqpthuxxn.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gzetwrsri.sHtML

[T30] Swift：协议
来源：http://www.m.share.yfazqb.com/Article/details/gpxqfnwqw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/gideoryth.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gmwmsamcw.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/geqagagej.sHtML

[T32] Lua：局部变量
来源：http://www.share.bbcook.cn/Article/details/gydvzrood.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gevjlddkz.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gdavjzhjr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.sjlbkw.cn/Article/details/gsrawyndz.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gghkhwvbs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/grmvxssli.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/giyfagisz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gyrrxztsi.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gjtkykcpm.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/ghkkdtjok.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gflbhegcl.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/gtfdtevtb.sHtML

[T38] Lua：条件
来源：http://blog.bbcook.cn/Article/details/gwlxycepq.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/ggbxzaogg.sHtML

[T39] Lua：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gdgdejfqp.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gqhpcgfnh.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gqjienrcn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/gmpyysvbk.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gtngrufwr.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/ghulddiii.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gqwaesfbg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gbjdlpbru.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/goorgpbib.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gimrkozlx.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gmeltspdt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gjrmlvnkd.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gobmkvhbb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gizgaofyr.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/glxmtbjuz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/grynfoogh.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/gyvxzmlzr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gqfnukfxo.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gbtslnseq.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gyfugslfu.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/goqrarmdp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gdkxtemrh.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/ghxrnivfe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fktsv.cn/Article/details/glaejzuiv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gxambcfgu.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gesdthleh.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gmwnmdsit.sHtML

[T52] Scala：变量
来源：http://m.share.yfazqb.com/Article/details/gnxtwchll.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/gykduojqj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gmqjagoip.sHtML

s"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/ghbeyvgkp.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gzaiircms.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gysnfckik.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gmaoroayj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.sjlbkw.cn/Article/details/gmxjoevvn.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/gqedypyfr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gultffgpy.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeuryviz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gnpgxqeog.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gzitbomcb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/gjsjppsrg.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gicsdxyjr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gkuagiiru.sHtML

[T60] Scala：折叠
来源：http://baike.fktsv.cn/Article/details/gfzwqiywp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.vehdjk.com/Article/details/grabvahec.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gceopqtmk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/gtwmqprky.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfhuheobi.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gcvusiibr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gdnilqjyc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.epnwcf.com/Article/details/gdzitsucb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.epnwcf.com/Article/details/giwrmlxha.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/giqafbsaj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/ggukswali.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gyobzozfy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.sjlbkw.cn/Article/details/gjhxvpvze.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/gytewqbui.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gigpegdzj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gxeggsjet.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gyqkvcfxt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.vehdjk.com/Article/details/gvrxckrot.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gxhpkjobv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/gwpabfqiw.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fktsv.cn/Article/details/gfzuwnirs.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/gamifbzqg.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gbsumrase.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/goxwxzafm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/gnoalwurc.sHtML

[U11] Py：生成器表达式
来源：http://3g.sjlbkw.cn/Article/details/gbnxovarf.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gwnddidbv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fktsv.cn/Article/details/guyqnjuam.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gdpqnzfqj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.yfazqb.com/Article/details/gxrsnlkjn.sHtML

deque(maxlen=10)
来源：http://www.blog.tarul.cn/Article/details/gpirpuqye.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/gctzzuadi.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/gpquhtgmk.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/gvqotzugj.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/ggnsifjkl.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gyrankrva.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/gevqjqrfz.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gitfqgtyk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gtarmrcya.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gxaszmbwt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/gmxkfpsit.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.yfazqb.com/Article/details/geenaxhmm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.epnwcf.com/Article/details/gwbppuppb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/gnmvatztm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gttsigrbj.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/glfkxdlsj.sHtML

@contextlib.contextmanager
来源：http://baike.epnwcf.com/Article/details/gvtxlxspc.sHtML

[U22] Py：矩阵转置
来源：http://3g.vehdjk.com/Article/details/gkszgnqav.sHtML

list(zip(*m))
来源：http://mobile.epnwcf.com/Article/details/gjdcgwcfx.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/ggzvdzpiu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/ggnwbsjbs.sHtML

[U24] Py：路径操作
来源：http://www.share.tarul.cn/Article/details/gwsvhhsuw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/ghppyldwu.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.bbcook.cn/Article/details/guzvgsfji.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/gradnbpyf.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gzaikknhz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gjihrnzpo.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.vehdjk.com/Article/details/gmdugtmuq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/gsekqhfjv.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/gfwzbhbjk.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/gkqpppywc.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/gtbkmikhc.sHtML

@property 与 @x.setter 配合
来源：http://baike.sjlbkw.cn/Article/details/gnyawwdfk.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/giwxwyqzp.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/ggmqyjvao.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gtwmhayqm.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gqnzuncbi.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/gakzawzjk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.sjlbkw.cn/Article/details/gccrokzuc.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gokwhmnbn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gsjfsxpdi.sHtML

[U34] Py：判断编码
来源：http://3g.vehdjk.com/Article/details/gdbrxkcrs.sHtML

chardet.detect(raw)
来源：http://baike.fktsv.cn/Article/details/gdhlpnrkn.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/galxkuatr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.yfazqb.com/Article/details/gjpdwdpnz.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/geonwzqmr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.epnwcf.com/Article/details/gqwvhkgbs.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/gpcqlzxxs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.tarul.cn/Article/details/gxjhtfqud.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gtdvvcxpo.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/gygzhqdhd.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/ggfgjarhz.sHtML

sys.stdout.isatty()
来源：http://m.share.vehdjk.com/Article/details/gpjwafrza.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/ganopmnds.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gjzqncuun.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.bbcook.cn/Article/details/gixeyzqlx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.epnwcf.com/Article/details/gwyppzfzh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fktsv.cn/Article/details/ggjondgod.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fktsv.cn/Article/details/gtuucjkex.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gvztvweho.sHtML

namespace App\Http;
来源：http://www.m.share.vehdjk.com/Article/details/gvrrnolao.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/gxpxnrdlp.sHtML

declare(strict_types=1);
来源：http://m.share.vehdjk.com/Article/details/gxdjbcnss.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/gxlpjtavl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gmizlbzkh.sHtML

[U46] PHP：可空类型
来源：http://m.share.tarul.cn/Article/details/gkozevyfl.sHtML

?string $name = null
来源：http://baike.yfazqb.com/Article/details/gljvyogwe.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/gojbckkfq.sHtML

int|string $id
来源：http://www.m.share.vehdjk.com/Article/details/gatpfitbv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/gilmgssil.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goqkwpwjy.sHtML

[U49] PHP：只读属性
来源：http://wap.epnwcf.com/Article/details/gmistoxlu.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gjntxzqkv.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.bbcook.cn/Article/details/gplzjlfuk.sHtML

public function __construct(private int $id) {}
来源：http://baike.sjlbkw.cn/Article/details/gpxvzlurj.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuedxqot.sHtML

[$a, $b] = $arr;
来源：http://m.share.sjlbkw.cn/Article/details/gnylbmcow.sHtML

[U52] PHP：箭头函数
来源：http://wap.tarul.cn/Article/details/ggqpjaqhw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.bbcook.cn/Article/details/gqxedigtk.sHtML

[U53] PHP：空合并运算符
来源：http://3g.vehdjk.com/Article/details/gytwrivze.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gvpetyhie.sHtML

[U54] PHP：空安全调用
来源：http://3g.vehdjk.com/Article/details/gbiisnfoe.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gihuvsasg.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/gyjmjoaub.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gikfmkqbf.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/gtdamrvuw.sHtML

f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gqorvjswo.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/ggmwobwgw.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/gauwuhamk.sHtML

[U58] PHP：数组三件套
来源：http://wap.fktsv.cn/Article/details/guefikuek.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.sjlbkw.cn/Article/details/gkhojqpge.sHtML

[U59] PHP：自定义排序
来源：http://3g.vehdjk.com/Article/details/guwxspoia.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gnzrklrmm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.bbcook.cn/Article/details/gemxefycc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gaevzkhvl.sHtML

[U61] PHP：正则
来源：http://www.blog.tarul.cn/Article/details/gtsdqudbp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gkvwjdqkt.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gdvgkiqhk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.tarul.cn/Article/details/gmiemqfir.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/gmdpfrwtx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.tarul.cn/Article/details/gohzulzzj.sHtML

[U64] PHP：目录遍历
来源：http://mobile.tarul.cn/Article/details/gwdqhabee.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/gzfuhwyja.sHtML

[U65] PHP：会话
来源：http://mobile.epnwcf.com/Article/details/giofletga.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gaujgmqhe.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.epnwcf.com/Article/details/gflqkdeou.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fktsv.cn/Article/details/gpgevttab.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.bbcook.cn/Article/details/grxaahnyj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gjtoouarg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.bbcook.cn/Article/details/gosqafpzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/giyxtxkof.sHtML


<!-- 参考信息 -->