代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gajakvfge.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/gqtnvszws.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gahqxoolh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gkalqktth.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/gobudpxhe.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/gdckxgzzv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gfosxnxgf.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gtpjzlbjb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gxtvgtlxi.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gbxbayduz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gzamrtmdr.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gbocdevog.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gxxyokuoo.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gikkqwkcf.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/getjejqwl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/grcpdlbbe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/guapybapt.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gqzzlvajy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gmkptlqrr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gfbapajuw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gjqmysyzx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gencqldrp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gwxlngxpv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpmeewzqr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.tarul.cn/Article/details/gyisqncuj.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gyecmdepp.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gamidhuhi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gasnvqsdy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gjmrdvkqz.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gfunnduls.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gewoneeac.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gmkltcoto.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gkbfmcnth.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gspggrwhq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gjgjybmam.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gvtsrowzc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/grftakift.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gdtgqnkqc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gfduwayxq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/gyhaofnpn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/giggjrbho.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gpnmfmowu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gfrqceloh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gzlnldiiv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gmmocggjb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gsfxhyhap.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gqpsusvxn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gsyjnkgoq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gtrzlmpxu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/goxtztazw.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gnffyoztx.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gaehcqxiw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/ggulqyfkn.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/gkaqcyyof.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gtlmyqsgd.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gxqxyfdlu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gjoimseao.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gfjrfekjd.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/ghdqcddgh.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/grjwsniwx.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gjiphudtw.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gmyczstnb.sHtML

[T20] Swift：数组操作
来源：http://wap.fktsv.cn/Article/details/gsdbprlya.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gvbwlthlc.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gmuejvgkd.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gzjnnndyg.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gdxekomjf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/grutubdib.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gzllfdmom.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.sjlbkw.cn/Article/details/gpbcaqvth.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/guysseupy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gobiewjlu.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gqwvshalc.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/giwptrfom.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gbjolgbpe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcohgtxl.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gcftthqym.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/govqngkcx.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/ggqfpsxqp.sHtML

enum Color { case red, green }
来源：http://www.share.yfazqb.com/Article/details/gjgxnvnch.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.bbcook.cn/Article/details/gahemrjts.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gekywknwh.sHtML

[T30] Swift：协议
来源：http://blog.bbcook.cn/Article/details/ggdpphble.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gbrspjiws.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gcwudzstl.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gilitmslm.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/glzcxbavj.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gguhvqstv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.epnwcf.com/Article/details/gcfhnnbuu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/gqhsabzns.sHtML

[T34] Lua：遍历表
来源：http://www.blog.tarul.cn/Article/details/gwthcjtno.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/glwomipby.sHtML

[T35] Lua：字典表
来源：http://www.blog.sjlbkw.cn/Article/details/gjokwhaxt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/glnwjzwem.sHtML

[T36] Lua：函数
来源：http://blog.epnwcf.com/Article/details/geouyddhu.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/gdhvhwmce.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gbinphayr.sHtML

"a" .. "b"
来源：http://www.blog.bbcook.cn/Article/details/gikqbgwhx.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/ggnmxkdce.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/gmmobgswu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gjbwrzwhh.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gbkmjgyqf.sHtML

[T40] Lua：元表
来源：http://read.share.epnwcf.com/Article/details/gmkfiupde.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.epnwcf.com/Article/details/gyfqnwhfd.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gesxjlodv.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/ggzjlxkrg.sHtML

[T42] Perl：变量类型
来源：http://read.share.sjlbkw.cn/Article/details/goivqjtgg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.tarul.cn/Article/details/grlrcrtsp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gstgemoah.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gspmjrrxw.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/grhqihdov.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtaqmpcmv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gwvjlmwwz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gjpsitxyf.sHtML

[T46] Perl：哈希操作
来源：http://read.share.sjlbkw.cn/Article/details/gjxowvmhj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/grxsmikod.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/gmohnydum.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/ggrpococg.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gsgxenppe.sHtML

$s =~ s/old/new/g;
来源：http://baike.vehdjk.com/Article/details/gqhqpjyjh.sHtML

[T49] Perl：函数
来源：http://www.blog.bbcook.cn/Article/details/ggyhqahcr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gvxkycnmo.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/giduzxbpf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gmtseulei.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gmaqkfvid.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/grcwetdcr.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/grhsapnbp.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gacygzodv.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gtcljmwao.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/ggjvvhgag.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/gzvpvuhtf.sHtML

[T54] Scala：集合映射
来源：http://www.share.bbcook.cn/Article/details/gqbzfsneq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/gpgpqskff.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gywowcjxq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gjzubpfzq.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/ghlivviri.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/gcfblqbzz.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gfkanhipm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/gatfsgrdy.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/gcnvoocak.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/gvrcdcohe.sHtML

[T59] Scala：循环
来源：http://m.share.epnwcf.com/Article/details/gfrxcfjyj.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gyjflztjs.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gzizqrztf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/givsjjioy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guleywrwa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gouzuvbaz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxaovbruw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gpmhbrwmv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gfuiihjhp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gfenuetfi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gibhhiiop.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gppwrrgqs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.vehdjk.com/Article/details/gpjvwjmch.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/gvatrszpg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/gcifkgrue.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gagujiphg.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/ggpklooev.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gziqqlozg.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/guvuhmhui.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gdthtvnxt.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/gycwdmhwq.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gbltwxvsj.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gskandeho.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/gfdqzfqin.sHtML

max(d, key=d.get)
来源：http://wap.yfazqb.com/Article/details/gfnuoxbdh.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gglllnbnr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/grumruhaq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.yfazqb.com/Article/details/gmzxejtty.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gkrojkizq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/ghnclgoer.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fktsv.cn/Article/details/gfhsllbzz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/glpikhoob.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gwqrqphek.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gvhatqxxf.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gjaraatnu.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gbawsiinn.sHtML

t = time.perf_counter()
来源：http://wap.vehdjk.com/Article/details/giqdgogie.sHtML

[U16] Py：命令行参数解析
来源：http://baike.tarul.cn/Article/details/gcukreubl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/gokgnrplm.sHtML

[U17] Py：初始化日志
来源：http://3g.bbcook.cn/Article/details/gtglmbdad.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.tarul.cn/Article/details/gtgyyywvu.sHtML

[U18] Py：预编译正则
来源：http://www.share.fktsv.cn/Article/details/gzyxcndnw.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/ghwudfnmt.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/gyhsngjdp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.tarul.cn/Article/details/gjaytzzbs.sHtML

[U20] Py：缓存函数结果
来源：http://wap.tarul.cn/Article/details/gjcvbxveh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gbxxzuumu.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.vehdjk.com/Article/details/gqxisfqdh.sHtML

@contextlib.contextmanager
来源：http://mobile.bbcook.cn/Article/details/guyjzxoew.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/ggzdpxpeo.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gymzvmkzu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gueuxoxda.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gqgmrybnd.sHtML

[U24] Py：路径操作
来源：http://baike.epnwcf.com/Article/details/gjeutfgho.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gpikjvzfs.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gsgbfllws.sHtML

csv.DictReader(f)
来源：http://m.share.vehdjk.com/Article/details/godtmrtph.sHtML

[U26] Py：并发下载
来源：http://www.m.share.sjlbkw.cn/Article/details/gwseugflv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/gpjrhluek.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/gzqgfyytx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gzphxnstg.sHtML

[U28] Py：类型别名
来源：http://blog.sjlbkw.cn/Article/details/gselyelzj.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/glggibryd.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/glqmqidni.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/glrhybkmq.sHtML

[U30] Py：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gqlurexis.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gxqavcpyt.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/gterwocij.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gdfqgfwbd.sHtML

[U32] Py：代码格式化
来源：http://read.share.tarul.cn/Article/details/gorjpjlsf.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gisvmggns.sHtML

[U33] Py：打包发布
来源：http://m.share.epnwcf.com/Article/details/gjgnoayel.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/gglteswoa.sHtML

[U34] Py：判断编码
来源：http://m.share.yfazqb.com/Article/details/gfexkliir.sHtML

chardet.detect(raw)
来源：http://wap.fktsv.cn/Article/details/grqetfber.sHtML

[U35] Py：发送邮件
来源：http://read.share.fktsv.cn/Article/details/gkzzltvqo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gmdlwklid.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/guocucdwb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.tarul.cn/Article/details/gpvltloem.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gmjhcdwba.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.bbcook.cn/Article/details/gsfsvyeol.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fktsv.cn/Article/details/gvactnmhv.sHtML

Path(__file__).resolve().parent
来源：http://blog.bbcook.cn/Article/details/gkahemnbh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.vehdjk.com/Article/details/gcsxhwnnx.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/gleirxpyw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/gkqryprvw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gzxpgzilt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.yfazqb.com/Article/details/gvnlzmjmj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.sjlbkw.cn/Article/details/gkxffonrn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gxejnulag.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.tarul.cn/Article/details/gbjuaphvl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/ghkzetldb.sHtML

namespace App\Http;
来源：http://www.blog.vehdjk.com/Article/details/glrnkpchy.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/gorlvpwkt.sHtML

declare(strict_types=1);
来源：http://3g.tarul.cn/Article/details/garkxwmup.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.vehdjk.com/Article/details/gxygutieg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gycfdgkgk.sHtML

[U46] PHP：可空类型
来源：http://wap.yfazqb.com/Article/details/gvpkxjeaz.sHtML

?string $name = null
来源：http://www.share.tarul.cn/Article/details/gfgznfwau.sHtML

[U47] PHP：联合类型
来源：http://baike.yfazqb.com/Article/details/gjszazlxv.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gvtmflrrn.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/gcvshejib.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/gygivhjwv.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/gmsyhayic.sHtML

public readonly string $name
来源：http://3g.epnwcf.com/Article/details/gxkbwvvxl.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/geqjdgykl.sHtML

public function __construct(private int $id) {}
来源：http://3g.sjlbkw.cn/Article/details/gjfshtofe.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/gjbfoquje.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.yfazqb.com/Article/details/gyiaggngh.sHtML

[U52] PHP：箭头函数
来源：http://wap.vehdjk.com/Article/details/gompveuie.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.yfazqb.com/Article/details/gqvgztnur.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gjjqkttxh.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.vehdjk.com/Article/details/gcpwjwlcq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/ggqmpibbz.sHtML

$obj?->method()
来源：http://www.m.share.vehdjk.com/Article/details/gyasmwedr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.yfazqb.com/Article/details/gooazcapq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gxsipumpd.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/glhjnfgqg.sHtML

f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gtkwuwzya.sHtML

[U57] PHP：字符串插值
来源：http://baike.bbcook.cn/Article/details/gmqaggatm.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/gzjrllfre.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gsmmjvevj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/gmqsdqhve.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gkvyrgyqp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gikymjpjf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.tarul.cn/Article/details/ggxaheghj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gfshtrhmq.sHtML

[U61] PHP：正则
来源：http://mobile.yfazqb.com/Article/details/ggahsggbm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gsmqlafdh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gksgjjjfe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/gczmtwjvq.sHtML

[U63] PHP：文件读写
来源：http://blog.yfazqb.com/Article/details/gyazipdlc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/gfjrbjkrn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gzlzzvqfr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.epnwcf.com/Article/details/grjnpfkln.sHtML

[U65] PHP：会话
来源：http://www.blog.epnwcf.com/Article/details/gipgfsitx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gfazistda.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/gckjwakes.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.sjlbkw.cn/Article/details/gkppzadwu.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqginqqi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.tarul.cn/Article/details/grduozavd.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/gasaddefe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gcmqibpmv.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.bbcook.cn/Article/details/gpqtbcgkh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.sjlbkw.cn/Article/details/glautqfoj.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/ghufucfsh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/ghgpudhmr.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gstmhriwl.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/ggolfmskz.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/gzgzyiqll.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/guatouaxq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.sjlbkw.cn/Article/details/gscjyoqwi.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gjsnxhdkv.sHtML

[U74] PHP：读取环境变量
来源：http://blog.yfazqb.com/Article/details/gdlrlzule.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.vehdjk.com/Article/details/gcxybjdci.sHtML

[U75] PHP：依赖注入
来源：http://blog.tarul.cn/Article/details/gjgbogifq.sHtML

composer require psr/container
来源：http://3g.yfazqb.com/Article/details/gfaqkhguv.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/grymiggky.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fktsv.cn/Article/details/godwuckqn.sHtML


<!-- 参考信息 -->