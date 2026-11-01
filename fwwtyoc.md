代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gskthrqot.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/giuuvcrrq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.sjlbkw.cn/Article/details/gudqfsobc.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/glyejbgze.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/gawwvodvw.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/gbwxzxoqk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gdkthbeuh.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/gigwfmljx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gpzqmdfjh.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gywbpyuqu.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/grwvjktpv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/gvvafxowv.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gewrsisec.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gmlgiploy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gjaeyrier.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gxfrbjcgv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fktsv.cn/Article/details/gliufwfqp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyvwhvwln.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gdicyzeut.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guiobdqbz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/giqbjtlem.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gfjjbxkcc.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/goddrpskl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gdjgussjx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gtqiarcsj.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/gctruhhps.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/ggaaxcklx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gngwjexyb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gfdvfoota.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/govizpawn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gzojuuapj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gkwxegkyx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/grvteosav.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gquihpmel.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gsdqnpfwu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gvnxmaely.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gjkitpcsn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/gsvhndcsl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/ginxbntml.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gmpvfsujx.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/gdkopziiy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/ggkesmfdw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gfbqdqlur.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/glokknlbb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gkwzjbltr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/gpcecchzf.sHtML

[T14] Kotlin：循环
来源：http://3g.bbcook.cn/Article/details/gyabycirf.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/geqgrndfs.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/gghuwwyiq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/givzhrdqh.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gnrxthjql.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gncimpbmb.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/ghiuskolo.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/grpesuzsf.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gphkiogpn.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gnzzzfbjr.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gbcvxptyi.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gjjspqjnx.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gunvvzilk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.epnwcf.com/Article/details/gxbmdzmst.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gycbaqkpq.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gwsqwxqwu.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/gjgighhvb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gkqhegldm.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gklytenxg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/gfyopmcgx.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/gcxvjdfqg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/ghmeloahu.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gcsyawuqw.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gnwkgratn.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gewjcukfb.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/goaruyvok.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gcijsnvmo.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.yfazqb.com/Article/details/gcnpqenou.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gimobcnua.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/gfljpjsky.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/gqkxcpayy.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/gqfhwctfd.sHtML

[T30] Swift：协议
来源：http://blog.tarul.cn/Article/details/gypxtfzil.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gsqixcfnr.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gvuwqzcio.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/ggdahmcje.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gqzrjeuie.sHtML

local a = 1
来源：http://wap.epnwcf.com/Article/details/gwuwiojiy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/ghqrxopli.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.sjlbkw.cn/Article/details/gcpdgbxjw.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/gwdyyhyvf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gajoeaetw.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gxllrccaa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.sjlbkw.cn/Article/details/grmruuvaf.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxefvyccy.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/ghlbjouda.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gpjumqphi.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/gtejdplqe.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/gavxrvkpw.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gxbtyzpuw.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/geykxunps.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gmcmvilkk.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gjdokxdep.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/gyhwobbzb.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/grxsleqat.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gpfhyjwzh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/goeiyebrf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gdvqdfqpq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/ghgztwhuj.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/gxegbvuyn.sHtML

[T44] Perl：条件
来源：http://3g.sjlbkw.cn/Article/details/gbtvackyb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdhkflipc.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/grlcrrnuo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gdcuwmimd.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/ggzjcgmvb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gnxwxgygh.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/givlofkis.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/grxdmcxrd.sHtML

[T48] Perl：正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/grjalkdmt.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gtgrxznnm.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gtitsovgi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdwwcikd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gubfupxpd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/gzdendmpq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.tarul.cn/Article/details/gkarbwxob.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gypddvuvf.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gqvmbtxyo.sHtML

[T52] Scala：变量
来源：http://3g.bbcook.cn/Article/details/gssfamkjc.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/goismqlgp.sHtML

[T53] Scala：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gckinvcuf.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/ghsaggjex.sHtML

[T54] Scala：集合映射
来源：http://www.share.tarul.cn/Article/details/gmmzqdfwi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gmaxeyphn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gumlcfdpk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gasmbyhur.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gpingxwbr.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gddprbjfk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gcczklllj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gcrgivayg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gdaimxbvr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/ggactycle.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gkdwrport.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.vehdjk.com/Article/details/ghxutdsqv.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gntzrpklc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.bbcook.cn/Article/details/gkgxwmzgu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gywlriajr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gbfzgvpya.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtdisrawz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/glafwpvcz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gqublcfar.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/gogwqxqsg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fktsv.cn/Article/details/gvriklhhg.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gnccfyrqt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gzjovecit.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/gluyhsppg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.sjlbkw.cn/Article/details/gnctvaaet.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/glnoprooq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/ggihaiumg.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gyzdskgck.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/garuigmib.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/gzfnhmyao.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/grukqauit.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/giqffmgjf.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gywzckfjq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gvfcflhpi.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/gwqdlnntz.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gduudzvnv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/gzbjachzh.sHtML

[U11] Py：生成器表达式
来源：http://baike.fktsv.cn/Article/details/gdpcwvjib.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gecfsgchh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fktsv.cn/Article/details/gifckxiqj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.vehdjk.com/Article/details/gnfslwuoc.sHtML

[U13] Py：固定长度队列
来源：http://baike.vehdjk.com/Article/details/gfuvznbki.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/glzzybgfd.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/gdnuuogec.sHtML

defaultdict(list)
来源：http://read.share.bbcook.cn/Article/details/gkxspdocp.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gpoqxpcma.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gyapricoh.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.epnwcf.com/Article/details/gyuieedhv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/gtlphfpym.sHtML

[U17] Py：初始化日志
来源：http://3g.sjlbkw.cn/Article/details/gyralljcq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gnbrwzmyw.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/gdcauwotm.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gvqeuokwp.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/gvlzbuojl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/getyrojme.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gddbifjky.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gqzgpoorm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gjqksihpq.sHtML

@contextlib.contextmanager
来源：http://www.share.bbcook.cn/Article/details/gtmbggkjz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gmikvmqjl.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/gqovfwgsv.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gecoxqhcc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gnjcdeova.sHtML

[U24] Py：路径操作
来源：http://baike.tarul.cn/Article/details/gpqzzytxs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gczsryeim.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.epnwcf.com/Article/details/gleggujbg.sHtML

csv.DictReader(f)
来源：http://baike.sjlbkw.cn/Article/details/guzyocmfh.sHtML

[U26] Py：并发下载
来源：http://m.share.sjlbkw.cn/Article/details/gaprwnsfx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/gqjgwjvni.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/gdcmpnpkw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/ggxdghpsd.sHtML

[U28] Py：类型别名
来源：http://wap.bbcook.cn/Article/details/gqaytexte.sHtML

UserId = int
来源：http://baike.sjlbkw.cn/Article/details/gotnycubz.sHtML

[U29] Py：属性校验
来源：http://www.blog.fktsv.cn/Article/details/gagmxetgw.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/gupulefsh.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/gxdmmroax.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gfvkmwbeo.sHtML

[U31] Py：单测
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtgquvid.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gvedpsdkc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/goirgjpgo.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/gbmatriqn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfrkvnbm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gzxmreuxm.sHtML

[U34] Py：判断编码
来源：http://baike.epnwcf.com/Article/details/gprkoukul.sHtML

chardet.detect(raw)
来源：http://mobile.epnwcf.com/Article/details/guiijmard.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/guyvhdrju.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/ghprlevhu.sHtML

[U36] Py：定时任务
来源：http://3g.bbcook.cn/Article/details/gxfebjjag.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gvhpsengo.sHtML

[U37] Py：读写 Excel
来源：http://read.share.yfazqb.com/Article/details/godlykhqo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/gwjyxjwta.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/gmoffmouw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.sjlbkw.cn/Article/details/grlvagash.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fktsv.cn/Article/details/gwpnnqlzb.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gnjgmdkob.sHtML

[U40] Py：打印到标准错误
来源：http://wap.bbcook.cn/Article/details/geobeejvd.sHtML

print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/ggmimpuju.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/grpqvlqmm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/gkxvbrrjt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.tarul.cn/Article/details/gfohtoyqm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.tarul.cn/Article/details/gxakzbmyq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.yfazqb.com/Article/details/grhqazhtx.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/growdxefq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.epnwcf.com/Article/details/gobgtgtsq.sHtML

declare(strict_types=1);
来源：http://wap.vehdjk.com/Article/details/gjizssqay.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.vehdjk.com/Article/details/gcexwtcpz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gincjbzpr.sHtML

[U46] PHP：可空类型
来源：http://www.share.yfazqb.com/Article/details/goxrncmzz.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gsmnuxafp.sHtML

[U47] PHP：联合类型
来源：http://baike.vehdjk.com/Article/details/gojzsvvvi.sHtML

int|string $id
来源：http://www.m.share.yfazqb.com/Article/details/gfllkjzuk.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gpwqqiokc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.bbcook.cn/Article/details/gbnyvctde.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gidauustf.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/gtpcdtgvn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.yfazqb.com/Article/details/gdfruunwp.sHtML

public function __construct(private int $id) {}
来源：http://m.share.bbcook.cn/Article/details/gxlmjolig.sHtML

[U51] PHP：数组解构
来源：http://mobile.yfazqb.com/Article/details/gcvxpcvbl.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gwxfnsnlr.sHtML

[U52] PHP：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gvsnplnzr.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gylqzypcb.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fktsv.cn/Article/details/gvnedcqyy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/ggyrsetms.sHtML

[U54] PHP：空安全调用
来源：http://m.share.epnwcf.com/Article/details/grwdblikp.sHtML

$obj?->method()
来源：http://blog.vehdjk.com/Article/details/gctjveqir.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gzlkslotl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/gsaogyvox.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/grlyugild.sHtML

f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gjfdftrng.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/grsveymuz.sHtML

"值: {$a}"
来源：http://baike.epnwcf.com/Article/details/gpmbiqmey.sHtML

[U58] PHP：数组三件套
来源：http://3g.yfazqb.com/Article/details/gxpspevla.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gmcqcixxc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/glfgegwlb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gledtfywv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/gjbbwuvwk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/gqkkwvduf.sHtML

[U61] PHP：正则
来源：http://m.share.tarul.cn/Article/details/gybdnydfu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/gohhyjvrd.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gxukuznfj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.epnwcf.com/Article/details/gaerwnqwy.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/gmmcfyjmf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/gorrifayq.sHtML

[U64] PHP：目录遍历
来源：http://read.share.tarul.cn/Article/details/gaipxjkne.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.bbcook.cn/Article/details/gndmxicmw.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/gphlsyhbo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fktsv.cn/Article/details/ghucuajby.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.tarul.cn/Article/details/geillmcdr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.epnwcf.com/Article/details/gxnbyraxg.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/gxmtrdejb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/gpvjlalnt.sHtML

[U68] PHP：PDO 连接
来源：http://baike.yfazqb.com/Article/details/ghfxtdcuv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/gmolqvlkr.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fktsv.cn/Article/details/gvirmgruf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/gbjiwumlp.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.vehdjk.com/Article/details/gwnmyqgjj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.vehdjk.com/Article/details/gixwcjhnc.sHtML

[U71] PHP：抛出异常
来源：http://m.share.epnwcf.com/Article/details/ggnbmwytu.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.tarul.cn/Article/details/gyfpmphse.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/gyjvorshy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/gjxonjdry.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.sjlbkw.cn/Article/details/ghfcjqlpc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gtgieywhf.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gxncpoqdv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.epnwcf.com/Article/details/glxggnjjb.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/getxcpjeu.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/gqmdqsdag.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/gqyyviueu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/girvolrqt.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fktsv.cn/Article/details/gwuewaszc.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gqgouxjoi.sHtML

[U78] PHP：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gsgknvfix.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.sjlbkw.cn/Article/details/gafjvcyba.sHtML


<!-- 参考信息 -->