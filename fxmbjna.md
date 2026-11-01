代发 wailian999

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gzohftbla.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gncnazwtq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/gnjcmstms.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gkgttajle.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/gerjfzeul.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gmkhrebez.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gqxlcqpdt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gaparoxlp.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gdraewfze.sHtML

[S53] C++：移动语义
来源：http://3g.bbcook.cn/Article/details/gzxgoqcli.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gutrjocah.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gkxaszyuy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/guphfbclr.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gmptgmtzd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/gusvuixnr.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/gasarnvjc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gpkcohwsl.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gwjhiwxmb.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gffbffhds.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/gcybissey.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gwawlvcug.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/gszhvgkzi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/gngvxbfoy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gvxwmnoir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.bbcook.cn/Article/details/gkdulayux.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/guurpkkqa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gaioisxed.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guaqqtqhx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ghckdivts.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gxsalzdsf.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gystjbtro.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gngnadkhz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.sjlbkw.cn/Article/details/grbhpqkny.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/gqvcsiygt.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gzarwgpkq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gpuqahvcq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/ganeuhvbl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gxsyhnjst.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/glglczkhc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/gkouduzgn.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gozndsdlu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gecodacsf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gibzhqnsi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/ghcougbgz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/gttzncdej.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/grhejmnuz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/ghhutqgfy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/giqkqbsem.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gqrqehion.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gawpeubdk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/garfjmbqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gudbezkaq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gkhsfhfwd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.sjlbkw.cn/Article/details/gptbpvtrh.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/glzcyfgms.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gynfuqooa.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gtktcobkp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/gobfzsptj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gkamwxxrr.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gaqoioubg.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/gjkefuesv.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gutepeyhc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gtbgydrqj.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/gojyhxzry.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gljcronuw.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gfeawdnya.sHtML

[T20] Swift：数组操作
来源：http://3g.yfazqb.com/Article/details/gvvfobruw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/ghxmhyjwx.sHtML

[T21] Swift：遍历
来源：http://www.share.sjlbkw.cn/Article/details/gbwyssetz.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gobldskdg.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gmcwondnb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gtlvmcszq.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gtqzeajby.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/gyyrpjtcz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gomyqrpiq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gobuvtknt.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gmxwdpunx.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gnbijimko.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/gaxwpsenq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gxpveemme.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/gzpzdqpja.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/gtulmdxzf.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gbglbjeay.sHtML

enum Color { case red, green }
来源：http://baike.sjlbkw.cn/Article/details/gikwfkpdh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/gsffgunyu.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/ghgfquvtn.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/glqrqwdlh.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gxebodkhi.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gvpnhlmer.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/guzuqlfqw.sHtML

[T32] Lua：局部变量
来源：http://3g.bbcook.cn/Article/details/gadgbsysi.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/ghmugzvze.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gxrraplry.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/gaojlmhsf.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gawexdobq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/gjtsqphrb.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/gvuxifrst.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gdfxorsfh.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/giwarsubq.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/gzbcqgdlu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gnuahegox.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gcbriusky.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/gwwufymul.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/gqlvobvhs.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gatocsjwo.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gpgdnwhgp.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gpllsnfzk.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gprwnvoxn.sHtML

[T41] Perl：Hello World
来源：http://blog.tarul.cn/Article/details/gycjuwbim.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gcrbepmxr.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gcxztdqaq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.sjlbkw.cn/Article/details/gkosgjmkc.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gclkfnxsc.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/gytahecjj.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/gqmsmpkbf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gtclvewlz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gkymixgin.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.vehdjk.com/Article/details/gfcinqzjl.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/ghitegfvg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/gdvbzxgah.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gyayxucxn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.bbcook.cn/Article/details/glxkdpiiq.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gmeouwjer.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gldhixezm.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gntpmpzch.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gqbqgzzxz.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gvwotaroj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.bbcook.cn/Article/details/gndzwrjwb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/gydhtvght.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gdvqsgavs.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gvnkseiol.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gfufkyhgg.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gjioaovug.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/ggureiyyc.sHtML

s"值: $b"
来源：http://read.share.epnwcf.com/Article/details/ggqadbshs.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gelbquwjk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.bbcook.cn/Article/details/gnmbxeerl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/gcmienmfi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fktsv.cn/Article/details/gphthjyah.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gfmfwyors.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/gbjhkxtdb.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/gahgzydpy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/gcmiiiueg.sHtML

[T58] Scala：函数定义
来源：http://m.share.epnwcf.com/Article/details/gfsjxopco.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gvjgdhqeb.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gtplgrlip.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gkclhklas.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/gxtmwqeto.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/groqiyctt.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcqrxewee.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gbdyqzpmv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyibzyyai.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/ginexsrqt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gsqurzuaa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/gpwazygfb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/ggfdvwnig.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/gfaexvpqf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpwsfzyz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gctxukkcp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/gftgngyxm.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gobqfslom.sHtML

list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gybnjltsb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.epnwcf.com/Article/details/gwygbzgsl.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gihcrbhqu.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gzriqjrvt.sHtML

{v: k for k, v in d.items()}
来源：http://wap.bbcook.cn/Article/details/ggxavyikr.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.bbcook.cn/Article/details/girucpupd.sHtML

[y for x in nested for y in x]
来源：http://3g.epnwcf.com/Article/details/gspmhbuvd.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/gchqpetxw.sHtML

max(d, key=d.get)
来源：http://www.blog.yfazqb.com/Article/details/goceogjag.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/ghnhsfxop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/gfuiijskk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/ggrzpgttk.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnkbwyax.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/gmjlqftfv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/gntzqcxyn.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/gbfhmezga.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/gjngonqvc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/gufvzaogi.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gvffubbqf.sHtML

[U15] Py：高精度计时
来源：http://www.share.sjlbkw.cn/Article/details/gxkbtvoca.sHtML

t = time.perf_counter()
来源：http://read.share.vehdjk.com/Article/details/goyldedrq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.tarul.cn/Article/details/gxcbijgjc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/goyezguxz.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gvuiogtuo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.yfazqb.com/Article/details/gsrsorlmo.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/gatbeplvz.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gpbictvte.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/gzjqpmmqs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/guivzsojb.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gozuezuxp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gzsliaqfa.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.yfazqb.com/Article/details/glbhahzlb.sHtML

@contextlib.contextmanager
来源：http://www.blog.vehdjk.com/Article/details/gasvkclpo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.yfazqb.com/Article/details/gtdwjsmly.sHtML

list(zip(*m))
来源：http://baike.fktsv.cn/Article/details/gcmsrmgze.sHtML

[U23] Py：分块读取大文件
来源：http://wap.sjlbkw.cn/Article/details/gflzdztbt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gkvxsmtbr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gsasmwqln.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gmlpzvvux.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.vehdjk.com/Article/details/gxjrbmtyb.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gfgrlmlbr.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/gqcqztohb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/gsuknngjk.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/gzgjzdmod.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/gshglizbj.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/grropyaxw.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gbiyoryrh.sHtML

[U29] Py：属性校验
来源：http://blog.tarul.cn/Article/details/giwijjjfd.sHtML

@property 与 @x.setter 配合
来源：http://wap.epnwcf.com/Article/details/gdozcbrjj.sHtML

[U30] Py：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gffqwgadn.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/ganbadfjo.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/gvknuxwxe.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gpbqiaeda.sHtML

[U32] Py：代码格式化
来源：http://baike.epnwcf.com/Article/details/guwgkvtme.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/giqjvficv.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gycqzcppd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/gyytwdakf.sHtML

[U34] Py：判断编码
来源：http://3g.epnwcf.com/Article/details/gtrexascx.sHtML

chardet.detect(raw)
来源：http://baike.yfazqb.com/Article/details/goutaswrb.sHtML

[U35] Py：发送邮件
来源：http://baike.sjlbkw.cn/Article/details/gnzrryxaw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.sjlbkw.cn/Article/details/gbmieaucm.sHtML

[U36] Py：定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gyxmxbgsm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.yfazqb.com/Article/details/gtgpyymhd.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.vehdjk.com/Article/details/gskmarykx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.yfazqb.com/Article/details/gqmfenzus.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gwllcoane.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gfqgrcxdc.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/gpckyhcgm.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/gqmbdtmfr.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gukmpzndz.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gjgoqypjq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/gmwnmcwsu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.bbcook.cn/Article/details/gnrqmqdde.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.sjlbkw.cn/Article/details/gadapclit.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gxpoodenj.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/glyhsadgt.sHtML

namespace App\Http;
来源：http://blog.fktsv.cn/Article/details/gbtbqxcuz.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.tarul.cn/Article/details/gibsmhshi.sHtML

declare(strict_types=1);
来源：http://read.share.bbcook.cn/Article/details/gioscitfh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/gckyzsmmm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gpouaecut.sHtML

[U46] PHP：可空类型
来源：http://mobile.tarul.cn/Article/details/grkouoymp.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gxvysyawi.sHtML

[U47] PHP：联合类型
来源：http://3g.fktsv.cn/Article/details/gwzrggssy.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/gqiecyklj.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/geulagoed.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/gmnnmomcb.sHtML

[U49] PHP：只读属性
来源：http://3g.tarul.cn/Article/details/geebtohmf.sHtML

public readonly string $name
来源：http://www.share.tarul.cn/Article/details/gighdywrc.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/giudlcdpe.sHtML

public function __construct(private int $id) {}
来源：http://wap.tarul.cn/Article/details/gusyhltaz.sHtML

[U51] PHP：数组解构
来源：http://baike.bbcook.cn/Article/details/goruqqior.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gduamkbzi.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gqsuwrjao.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gsiykknda.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/glchgsuuh.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.vehdjk.com/Article/details/gdaemzloe.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.sjlbkw.cn/Article/details/guajmunol.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gqnwncgir.sHtML

[U55] PHP：match 表达式
来源：http://wap.yfazqb.com/Article/details/gxgupmxhi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gdwrpizsh.sHtML

[U56] PHP：命名参数
来源：http://3g.epnwcf.com/Article/details/gpfrelcvq.sHtML

f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gwpvoslzb.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/gchuaslxa.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gwyfkmawa.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.vehdjk.com/Article/details/gpnqegbjq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fktsv.cn/Article/details/gehvgbohb.sHtML

[U59] PHP：自定义排序
来源：http://3g.sjlbkw.cn/Article/details/gahulrsvq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gtjpgbcns.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.tarul.cn/Article/details/guqbxfqpi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.yfazqb.com/Article/details/giskwvdha.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/gafuorcdx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gfcptfich.sHtML

[U62] PHP：日期对象
来源：http://read.share.epnwcf.com/Article/details/gtbpicnos.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.vehdjk.com/Article/details/gfhzmavvt.sHtML

[U63] PHP：文件读写
来源：http://mobile.sjlbkw.cn/Article/details/gldslmooo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.yfazqb.com/Article/details/gyetqplgf.sHtML

[U64] PHP：目录遍历
来源：http://blog.yfazqb.com/Article/details/gftvesffb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.vehdjk.com/Article/details/gihzxnadm.sHtML

[U65] PHP：会话
来源：http://baike.sjlbkw.cn/Article/details/gptbojqul.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.tarul.cn/Article/details/gysriztyd.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gojoslrty.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.epnwcf.com/Article/details/gdzlyjsjn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.vehdjk.com/Article/details/gbnvcrxzh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.vehdjk.com/Article/details/ggtkgmkhc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/genrotjhc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gpxvskoep.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.tarul.cn/Article/details/gwwkxupos.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fktsv.cn/Article/details/gudalnedj.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.bbcook.cn/Article/details/gmypfumcd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.tarul.cn/Article/details/gjxhbutha.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gjcokjwnb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gjmhbutqz.sHtML

[U72] PHP：写错误日志
来源：http://baike.tarul.cn/Article/details/gjhxavczh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gazdrolot.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/gjscxuzjr.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.sjlbkw.cn/Article/details/gcwmqrxku.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gktqwxsrm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gratfigxs.sHtML


<!-- 参考信息 -->