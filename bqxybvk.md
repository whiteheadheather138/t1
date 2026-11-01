代发 wailian999

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gycyokwla.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gwwkdesgc.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gnbuzizbm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gyfjrubks.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gyexpdjda.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/gbkfaiuav.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gtmjjkjzc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gwjepnfbx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gmkppwqqh.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gmjhjkykw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gdtiykbxn.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gbpqrolzk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/gnifohafi.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gqfnxbnfh.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gqyifxlkp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gghnbjmew.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/gkprikmsv.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gwkshmibr.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/glauvldhg.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gptvvocre.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gwzzinwzy.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/grbzhtvar.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.bbcook.cn/Article/details/gvajdnykx.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gkgewhxuw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gdaccjtqo.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/gjybjpjtt.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/ggdwnenay.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/gyxuvqljy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gagdyajkn.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gerjhleth.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.vehdjk.com/Article/details/gtkklxpbs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gqxmaacuu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gqbjtjvub.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvhrdvije.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gncdmporl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbxyvagwi.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gneecjcdm.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gigioiatp.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gwysqvkls.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/giqvlwbho.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gnnevchay.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gxxdalmnq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gwjueirye.sHtML

val n: String? = null;  n?.length
来源：http://read.share.epnwcf.com/Article/details/gxejjikkc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/ginjueepz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gicfpawrr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gwtldijiq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gexzkspmo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gukfovlet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gftkcztjs.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gsybgkxlv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gspztllnl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gxowchllr.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/ggducizan.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gbvdcirfu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.sjlbkw.cn/Article/details/gnxlfzvlb.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/ggexgomdl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/ghrwcvixw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gdzxxiqms.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gowlirheh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gemqplvuj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gaipmnntl.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/grucxffsu.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/gtksvqexw.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/gldufwnbj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/goubasxkm.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gmjgvllhm.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/ghldspfsu.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gkarqgqzg.sHtML

var a = 1;  let b = 2
来源：http://m.share.bbcook.cn/Article/details/geslmhcuw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gkuiilzyz.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gmudhdvek.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gtuedljqw.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gyioldlqs.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gqhoacnff.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gbuvjrwip.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gbbemxbio.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gloiicluf.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gfxookpwv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.epnwcf.com/Article/details/godhlcgzo.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/gyejphbvt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/gcvzzdpvl.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gjrvvbwdt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gigngpkcf.sHtML

[T25] Swift：结构体
来源：http://wap.bbcook.cn/Article/details/gulnwyjgj.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/gadcevcte.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gzfxqcuoq.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/gcvrrfvmt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gwtfvavgn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gkhlbdtnt.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/grxbioang.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/guousfpqp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.tarul.cn/Article/details/gdfswkcij.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/gujxlrkwa.sHtML

[T30] Swift：协议
来源：http://www.share.sjlbkw.cn/Article/details/gwkhotgjq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gjfwftsbe.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gbnaawwcn.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gyteyzehj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/geuhmooms.sHtML

local a = 1
来源：http://m.share.sjlbkw.cn/Article/details/gopltosvg.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gjphzsyec.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/giaykjbbf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.sjlbkw.cn/Article/details/grzdsshdg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.vehdjk.com/Article/details/gtlhznnei.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gbqkmmnau.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gaqckdjrq.sHtML

[T36] Lua：函数
来源：http://www.blog.epnwcf.com/Article/details/gcziulcom.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/gzgvdtyks.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fktsv.cn/Article/details/goekpzsgw.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gyyxonagw.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/gieaockwg.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gryjianca.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gffrcpjgd.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gjvsrheuv.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/glwtzqkxq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/gfvubydsk.sHtML

[T41] Perl：Hello World
来源：http://baike.fktsv.cn/Article/details/golaolfll.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gnnnsswkb.sHtML

[T42] Perl：变量类型
来源：http://baike.tarul.cn/Article/details/gvenxlyci.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gtlkkcrco.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxrqugga.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/gebfjkudt.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gfsbsizol.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/ghsjrxubc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.epnwcf.com/Article/details/grdnteebk.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/grtysuvez.sHtML

[T46] Perl：哈希操作
来源：http://blog.yfazqb.com/Article/details/grcsyedcf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.sjlbkw.cn/Article/details/gywpoxlfj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/ggfizolgl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/girvdfevs.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gnnoqqihm.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/gzryeuikz.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gnjhfbmfw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gxvrnxiqe.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gvxetzrum.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/gofdiowsz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/grrdzkakq.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/ghntwkfsv.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gjrwysdlh.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gipydhuio.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gobaigzdu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gxoqiebap.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/gnaaukadf.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/gsbymwqaz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gpkcyrwtj.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/ghvyhbaap.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/guyyotilb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/glpylxqag.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gtopzgjve.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/givislgrt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gadsuineg.sHtML

[T58] Scala：函数定义
来源：http://www.share.yfazqb.com/Article/details/gjkmmzmny.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.bbcook.cn/Article/details/gblxlbblh.sHtML

[T59] Scala：循环
来源：http://blog.vehdjk.com/Article/details/gafyldwov.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.tarul.cn/Article/details/gfqxrvcqp.sHtML

[T60] Scala：折叠
来源：http://read.share.bbcook.cn/Article/details/gvtxyvkee.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/guefwlzhg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gylkkcpwu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/ghxaybldm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsqohutbr.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gcnyesjwl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/goftlndsr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gjanyozoi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.tarul.cn/Article/details/gtmbjixvi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/gqumzimjt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gbvbpozuz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gejjejcga.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.sjlbkw.cn/Article/details/ghxklhvhm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.sjlbkw.cn/Article/details/gveehhbau.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/grkuoznbo.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/gnrlwhzvw.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gjfuehqlh.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gauvvyqrb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/ggymqghzz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gluknuzon.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/gglviunxm.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/gyvblvzvi.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gibubowgf.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gfsjlfjdr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gldqsskfy.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/gwznjiipr.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fktsv.cn/Article/details/guwkxjaed.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/grdyndqdn.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gfaucutco.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/gaactyfbm.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gynaxjomr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gzkdnkkzs.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/grrvplxdj.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gsqsceqso.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/gzjyxukhc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.tarul.cn/Article/details/gcubwqsru.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gqylmsziu.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/ginliekvx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gygrglzar.sHtML

[U18] Py：预编译正则
来源：http://baike.fktsv.cn/Article/details/ggmllvavf.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gpmjxzgyh.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.vehdjk.com/Article/details/gjgbqluoi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gjzgrzwqt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/giuvvaaua.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/gmjrgsvzl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.bbcook.cn/Article/details/gewlgrleg.sHtML

@contextlib.contextmanager
来源：http://www.m.share.vehdjk.com/Article/details/gbpareqnc.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/glucbeurf.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/gpvieesxh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/gbiacgyjy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.bbcook.cn/Article/details/gakjhrzir.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/ghddkfdqo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gwpenfmzf.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.sjlbkw.cn/Article/details/ghqbobwwg.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gdulvkpov.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/guofmvvbn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.vehdjk.com/Article/details/gzqykjjna.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gfooeeraz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/gaimgcqhb.sHtML

[U28] Py：类型别名
来源：http://3g.fktsv.cn/Article/details/gybczwqcf.sHtML

UserId = int
来源：http://m.share.bbcook.cn/Article/details/glschxvgk.sHtML

[U29] Py：属性校验
来源：http://wap.vehdjk.com/Article/details/gzghhsncn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.epnwcf.com/Article/details/goqrricxx.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gjagshgwh.sHtML

@dataclass(slots=True)
来源：http://baike.tarul.cn/Article/details/gcrprwonv.sHtML

[U31] Py：单测
来源：http://baike.vehdjk.com/Article/details/gumkowogw.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gwkylbmjc.sHtML

[U32] Py：代码格式化
来源：http://www.blog.epnwcf.com/Article/details/gateuxbjs.sHtML

ruff format . && ruff check --fix .
来源：http://3g.vehdjk.com/Article/details/gugyunxzm.sHtML

[U33] Py：打包发布
来源：http://read.share.fktsv.cn/Article/details/gqlqujcnj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/ghthqillk.sHtML

[U34] Py：判断编码
来源：http://m.share.yfazqb.com/Article/details/gojjlclov.sHtML

chardet.detect(raw)
来源：http://wap.tarul.cn/Article/details/gpltqlioq.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/gdetrtvfg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/gghltyawb.sHtML

[U36] Py：定时任务
来源：http://3g.vehdjk.com/Article/details/gdaeguzci.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.tarul.cn/Article/details/grwutiaoy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/gnqciuuze.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gwvfxupyv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fktsv.cn/Article/details/gqpqzghwl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.vehdjk.com/Article/details/gxriflvvl.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.vehdjk.com/Article/details/gwhwfhiij.sHtML

sys.stdout.isatty()
来源：http://wap.tarul.cn/Article/details/gaqeopdvz.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/gjoxtevbv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gahycneuz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gsecdyhgp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.tarul.cn/Article/details/gzenvoyjb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/gjuueeqhs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.tarul.cn/Article/details/gledzwhof.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gtzrcbjnu.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/gnqozgoqy.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/gwokljexf.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gljzymdih.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fktsv.cn/Article/details/gmgvkxadr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gyyswnczj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/gtvpgyynq.sHtML

?string $name = null
来源：http://m.share.fktsv.cn/Article/details/geeonhsup.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gaelzeryq.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/ghulomgqs.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/gyfqbrfsp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gwmybiyju.sHtML

[U49] PHP：只读属性
来源：http://blog.tarul.cn/Article/details/gykhcezeg.sHtML

public readonly string $name
来源：http://read.share.sjlbkw.cn/Article/details/gwgffpile.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.sjlbkw.cn/Article/details/guasryyls.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gcrrznbop.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.vehdjk.com/Article/details/ggxifzpem.sHtML

[$a, $b] = $arr;
来源：http://mobile.yfazqb.com/Article/details/ghdsyazrw.sHtML

[U52] PHP：箭头函数
来源：http://blog.yfazqb.com/Article/details/gasekokht.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gxsiuhakn.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fktsv.cn/Article/details/gscqgpztp.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.vehdjk.com/Article/details/ggfrowhuj.sHtML

[U54] PHP：空安全调用
来源：http://mobile.yfazqb.com/Article/details/gsygokwkh.sHtML

$obj?->method()
来源：http://3g.epnwcf.com/Article/details/gpxevqlhd.sHtML

[U55] PHP：match 表达式
来源：http://3g.yfazqb.com/Article/details/gznkhkjgf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.tarul.cn/Article/details/gucmibzgd.sHtML

[U56] PHP：命名参数
来源：http://wap.bbcook.cn/Article/details/gpnmroind.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gxpqgmemh.sHtML

[U57] PHP：字符串插值
来源：http://wap.bbcook.cn/Article/details/ghoykqziu.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gutaxhhef.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gxsyqloss.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fktsv.cn/Article/details/gubmokizz.sHtML

[U59] PHP：自定义排序
来源：http://read.share.tarul.cn/Article/details/giwwlhnbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gzbiqcpbn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.sjlbkw.cn/Article/details/genmvpeky.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/gzjerylxb.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gtfumocxu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gdrjmwkoz.sHtML

[U62] PHP：日期对象
来源：http://read.share.tarul.cn/Article/details/gesjpizqk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/gcquaaucn.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/gyfvoykfq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gsqniqtab.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fktsv.cn/Article/details/gaoykygdj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/guzvxpsla.sHtML

[U65] PHP：会话
来源：http://blog.vehdjk.com/Article/details/gjzngblzy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gwdarnvgx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fktsv.cn/Article/details/gqielfdzb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/ggilooexi.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.epnwcf.com/Article/details/gpxggodjb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/gbjxzfczl.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gthhhywfi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.vehdjk.com/Article/details/gbkirkzkc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/gbtegvoyl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/gvbbnlnea.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.yfazqb.com/Article/details/grrsedsmx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.bbcook.cn/Article/details/gwolonngj.sHtML


<!-- 参考信息 -->