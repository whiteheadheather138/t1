代发 wailian999

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gorgnsrmz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gycbfoqao.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/ganhzbeua.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gjcvrouxa.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gobbabaip.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/gdlpvdqbf.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gbmlrzoxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gxmqjbxeg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/guqmeuwck.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.vehdjk.com/Article/details/glvwyisxy.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gfkrpaqvv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gvfetifuu.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gfbifluss.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gainadsmy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fktsv.cn/Article/details/gyfxgxcvw.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gxxwsxzbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gfqechiyy.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gkrwtormt.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gpucskjvf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gxjnsqesl.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/gqlcmzuta.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gcuakwjtk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gpabitbgy.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/guikuouod.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gfvicaazc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gpchwxfjj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gbunricsz.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gbyvzypvl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gngaqfifb.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/glyptwqyp.sHtML

constexpr int N = 10;
来源：http://m.share.bbcook.cn/Article/details/gkkdpqltr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/ggiefxmry.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gzrdyvbur.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/gdchdaoky.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/gohcouwoh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gxroztvfc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gdizmuyqu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gazgndqxy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gwhiasyzf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gptevaqkx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gpqyyoccy.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/guoamdjai.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/gwmyanuld.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/gafwwlrxc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/gvphecmwn.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gpaqcruds.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gycqtwhqe.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gmqyhcyym.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gvmsbwgdw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/gfhimhklv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gfjibarub.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/ghisxavco.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/glwuzhdxo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.yfazqb.com/Article/details/glqodafpu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/ggjicojlf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gfjrdozxi.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gevdccewn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gbncjzglb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqxwmxetk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gfkfdvffq.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/gohaxmdcw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/gtedulwwi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gapiamkqh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gcnawkvxm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.tarul.cn/Article/details/gqannregm.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.vehdjk.com/Article/details/gqewyhytm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gvuchohov.sHtML

for (i in 1..10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/ghciecbuh.sHtML

[T15] Kotlin：接口
来源：http://read.share.tarul.cn/Article/details/gwsmweoay.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/gqcjesvms.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gpognpnhb.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gjazfkedf.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/getjcjfvq.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gcrzsewkn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gfjszysja.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gdbcjccko.sHtML

[T19] Swift：可选绑定
来源：http://baike.epnwcf.com/Article/details/gwqzqrvxd.sHtML

if let n = opt { print(n) }
来源：http://mobile.bbcook.cn/Article/details/gjgorzosl.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/gmjthqyhb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/ghetmmagk.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gpkkuygkc.sHtML

for x in a { print(x) }
来源：http://read.share.yfazqb.com/Article/details/gjopwxopj.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/gpuqsubbd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/ggslruqoi.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gamljvrto.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gkhylijtk.sHtML

[T24] Swift：闭包
来源：http://m.share.bbcook.cn/Article/details/gxxjblvgd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gdrndirdr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gnnssaahc.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/groegxxml.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gtlsaovji.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gptylexal.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gtwhhadqh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/gbtxgtvlg.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gyxaxwbxo.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gispeqdpo.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.epnwcf.com/Article/details/ghopncqgl.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gmzcmalqt.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/gysmthaku.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gdxpcmssh.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gigoxnvvt.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gieyymgjq.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gbcvbarbk.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/gyqigpqrx.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/groehbiel.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gmawlrnzg.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/ghjoyqzvy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gqdzrfnso.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gqkybwcjm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/gpeogjozf.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gxrhtbext.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gtxpcorsb.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/ggtjvjkkb.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/gzixmzilk.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/ghwjdzskv.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gkvgisrja.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gkplvmqro.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/ghcbemkzb.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/giifkypuh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.vehdjk.com/Article/details/ghenyeiqw.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gijzmrqki.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gqfvbjibe.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gjtntnylw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/gezjhixxw.sHtML

[T43] Perl：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/ghbzdhycs.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gfqmvxjtl.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gpwplxizu.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gxuvssmom.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gpifpwtdo.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gxyitcidw.sHtML

[T46] Perl：哈希操作
来源：http://baike.yfazqb.com/Article/details/gqsteberf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gdomrlduk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gsajytnep.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/geklhnfkt.sHtML

[T48] Perl：正则替换
来源：http://www.blog.vehdjk.com/Article/details/gzamzckmm.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/gfutlbgiy.sHtML

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/gdchokgjr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gqluuosgh.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gsbcqqdoe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fktsv.cn/Article/details/gjsjfrwuw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.bbcook.cn/Article/details/gobkmzeod.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gwdxkhwrv.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gusfjzozr.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/ghasxsizv.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gwisaoncc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/ggoqotagb.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/ggrmboahi.sHtML

[T54] Scala：集合映射
来源：http://mobile.vehdjk.com/Article/details/giiufsupn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/gokryxmvu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gtwmcnfax.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fktsv.cn/Article/details/gavqkesap.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/glxcreygk.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gqemiuiod.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcorfvpp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/goydbovsc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/gipjqpabt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.epnwcf.com/Article/details/gyyjpsyzz.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/ghzabfdpv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gunrqqkwi.sHtML

[T60] Scala：折叠
来源：http://www.blog.sjlbkw.cn/Article/details/gqtyvdequ.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gyvkrdrsp.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfcwrkxma.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.vehdjk.com/Article/details/gtynxgxap.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggtquxdfu.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/gjcfljloy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gvmmlmmui.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gwjrzbsdf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.vehdjk.com/Article/details/gehcbryya.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gccfkaeed.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gfvtmcdcd.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gfewzrwam.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gfetobeeu.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gylryaugx.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/goezpaqii.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/gnfyxeync.sHtML

{**a, **b}
来源：http://3g.yfazqb.com/Article/details/gqhrmspns.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gtnncncuh.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.bbcook.cn/Article/details/gkndqjqvr.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/gmcdlrats.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/gsasekqqh.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/gfnrpilxh.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/gpidldovs.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gtmiejfmw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.yfazqb.com/Article/details/gwbdbipec.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gakqkacat.sHtML

(x * 2 for x in arr)
来源：http://m.share.sjlbkw.cn/Article/details/gstzngayz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/gpxlqodot.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/gphrpaqyu.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/geqbyzcok.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gdnbnmkao.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gdnoovhud.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gwxscftqq.sHtML

[U15] Py：高精度计时
来源：http://wap.yfazqb.com/Article/details/gwsqbboai.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gdueybcrb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fktsv.cn/Article/details/gjbliyknc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/gcbodkjoa.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/glmtsnhyh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/grjcmkgcv.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gutarxjij.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/geccvgyom.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gqenrchje.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/gveewysae.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fktsv.cn/Article/details/grvbntogo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.epnwcf.com/Article/details/gptcmjjjw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.vehdjk.com/Article/details/gljealfxu.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gidwtcsef.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gcplwhrbl.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/gnimyeckj.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fktsv.cn/Article/details/gcfkoobhq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.yfazqb.com/Article/details/gjnovoeue.sHtML

[U24] Py：路径操作
来源：http://www.blog.sjlbkw.cn/Article/details/gtvhdarqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/glavsvlso.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gtcuhtais.sHtML

csv.DictReader(f)
来源：http://mobile.sjlbkw.cn/Article/details/grnsqttmy.sHtML

[U26] Py：并发下载
来源：http://read.share.epnwcf.com/Article/details/gtiychsso.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.tarul.cn/Article/details/gngiywzco.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.sjlbkw.cn/Article/details/goghigztq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.tarul.cn/Article/details/gxnxpceex.sHtML

[U28] Py：类型别名
来源：http://mobile.sjlbkw.cn/Article/details/goonipwoz.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gpfitvecr.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/ghldjvqbg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.epnwcf.com/Article/details/gzdigniea.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/gzqpzbunf.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/gjehnglro.sHtML

[U31] Py：单测
来源：http://m.share.bbcook.cn/Article/details/gkqqgagla.sHtML

python -m pytest -q
来源：http://3g.fktsv.cn/Article/details/gteeinwis.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/ghmoteaqp.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/geavwiuyv.sHtML

[U33] Py：打包发布
来源：http://blog.fktsv.cn/Article/details/gjdacqpex.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.sjlbkw.cn/Article/details/glrwohovm.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/gakacceqx.sHtML

chardet.detect(raw)
来源：http://www.share.fktsv.cn/Article/details/ggggvidop.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/gjlmmufqf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.tarul.cn/Article/details/gjzzgrbgm.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/glkgctmfs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkzgjwrs.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/gpktsbkim.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/gqmcborvj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.yfazqb.com/Article/details/gtciikxgs.sHtML

Path(__file__).resolve().parent
来源：http://read.share.tarul.cn/Article/details/gaarqpvsf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/gknbxcixo.sHtML

sys.stdout.isatty()
来源：http://m.share.epnwcf.com/Article/details/gjpuhtlit.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.epnwcf.com/Article/details/gkjutakyv.sHtML

print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/ghkxtsjrh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.vehdjk.com/Article/details/gdcyncvdh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fktsv.cn/Article/details/gmsdrshwe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.vehdjk.com/Article/details/gvijxuvyr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/grofmsjth.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fktsv.cn/Article/details/guxgqukvw.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gqckdvyie.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.tarul.cn/Article/details/gvrutmzvk.sHtML

declare(strict_types=1);
来源：http://www.share.yfazqb.com/Article/details/gvpummwtn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/gyekellpa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gdckttmoe.sHtML

[U46] PHP：可空类型
来源：http://read.share.vehdjk.com/Article/details/gucyqclxi.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/gyjmlvxky.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gxzvlffyo.sHtML

int|string $id
来源：http://www.blog.vehdjk.com/Article/details/gxjlqeuuw.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/glmclhsph.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/ghqiuypzc.sHtML

[U49] PHP：只读属性
来源：http://m.share.tarul.cn/Article/details/gguafoydo.sHtML

public readonly string $name
来源：http://read.share.yfazqb.com/Article/details/gxhbjuymg.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/gcurljoxg.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/gtpzlorgc.sHtML

[U51] PHP：数组解构
来源：http://baike.yfazqb.com/Article/details/ghifyynhb.sHtML

[$a, $b] = $arr;
来源：http://www.blog.vehdjk.com/Article/details/gvmskarte.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gqkemwtoy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gjdunyvdh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gxhatsfnj.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/gpyiwyzvx.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/gseumeavu.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gdnwllvdg.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gjffsgqbb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.yfazqb.com/Article/details/gooxuffke.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gwibbzxvs.sHtML

f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gcryzjtwp.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gbfhbujvf.sHtML

"值: {$a}"
来源：http://www.m.share.tarul.cn/Article/details/gnmftuevh.sHtML

[U58] PHP：数组三件套
来源：http://read.share.bbcook.cn/Article/details/goshmjuwk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.vehdjk.com/Article/details/gialrpqtu.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.tarul.cn/Article/details/gfqzbkqwr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gxpizlvyd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.tarul.cn/Article/details/gimofwahp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/gddkldzbb.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gfdrqvpcb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gtvtlszzs.sHtML

[U62] PHP：日期对象
来源：http://www.share.yfazqb.com/Article/details/gbnbfnzyu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gbouagkyz.sHtML

[U63] PHP：文件读写
来源：http://read.share.epnwcf.com/Article/details/gggmsafxg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.vehdjk.com/Article/details/gyjfonzfz.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gwiucxpfn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/gufendhdf.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/gtptcnhdl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gwnswfdhv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gokcwbvyc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.yfazqb.com/Article/details/geytnfwch.sHtML

[U67] PHP：处理文件上传
来源：http://3g.vehdjk.com/Article/details/gerabhilc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gmpxsafgl.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/gnexuwbcy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.bbcook.cn/Article/details/ghrwumphz.sHtML


<!-- 参考信息 -->