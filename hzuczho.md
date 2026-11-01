代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gkufdmmff.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/ggbxifnle.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gqnivggtu.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/gglcwqmpb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gzcoemyee.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/godliadym.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/gfiojtxgc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gdtojcjfi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fktsv.cn/Article/details/glbtvfwvb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gunxirsfb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gvnwfjzjr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghvxvuhxu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gienoavzj.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gvsxrpkvi.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gyxehgroi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gsktnfati.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gnjuepaiu.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gppftditt.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gqhgygvzo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gyhqwqoad.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gakinxkzw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/gqdkxxdvu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/gyeewxupg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gewwtwamb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gaqxkfiti.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/ggguqgbsa.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gbpfxogjg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gbvjmeriq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.yfazqb.com/Article/details/gwurrunkv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.bbcook.cn/Article/details/garjiouxw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/goeqveqif.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gubozritx.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/ggraxevgj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gdhdccnee.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gvdwkiolh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gytcxpvjp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.tarul.cn/Article/details/gdxznyegb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gxcmlsnku.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gxjmlhzml.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwfcsfmi.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/golwnntnb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gtrrsjglh.sHtML

[T16] Swift：Hello World
来源：http://3g.bbcook.cn/Article/details/gjdtstwkm.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gzqjiaofb.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gzujorfuz.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/gajeqmldx.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/glxhsztax.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gyddxtowe.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gqzygbrbq.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/grcflaxyc.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gdsjrzjpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gkmyycfur.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gsofvpukr.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/ggqtiuljj.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gbexqirqe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gwcflxtss.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gtbfixewl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gummdkgea.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gkkyzcvgn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gvvnaioxr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/gyqpmhxdz.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/gqiffnwlh.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gwtijmuwk.sHtML

class A: Base { override func f() {} }
来源：http://blog.sjlbkw.cn/Article/details/geecughts.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/gvgafvkhh.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/gbxvokyyh.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gnyyjnmdg.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/gqbotqzla.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/grtbcqtzr.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/giltcgwqv.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/ggpbmleky.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/gjzsvzyaz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkyvhpvj.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/grrgzykim.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gvnqzdmeu.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gulytowex.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gebzleuzr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/giubwmjxn.sHtML

[T34] Lua：遍历表
来源：http://baike.yfazqb.com/Article/details/gkcvifzlj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gtjvvojfi.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/ghrxkdcps.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gqplbbvxh.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gxhwlyomf.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gjttuiqjs.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gdbltipef.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/gqxsatkrj.sHtML

[T38] Lua：条件
来源：http://www.m.share.vehdjk.com/Article/details/gpkhslyzc.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/gpefilcit.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/gmlozbmiv.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/goruoktrf.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/guhvnlran.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gtegafbyd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gioqxkhom.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/gvhvgrntc.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/ghjwsyrnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gvltjtudv.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gwspehnpm.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gjgrttwga.sHtML

[T44] Perl：条件
来源：http://www.m.share.vehdjk.com/Article/details/gqibmdigi.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gdaiedqvw.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gjtyzpiqi.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/glcmzzkkp.sHtML

[T46] Perl：哈希操作
来源：http://blog.sjlbkw.cn/Article/details/gorxobgra.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gqcrmnlqg.sHtML

[T47] Perl：正则捕获
来源：http://3g.epnwcf.com/Article/details/gnwwmykmn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gbiqpxqsk.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/gpkwhqfrd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gqknbvwyt.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gmbupwejc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/grlwthmeb.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gtwmvqriq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/ggztpporc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.bbcook.cn/Article/details/gbkuxzxws.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/gzxfxfrsp.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/glitgxwrv.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/gcvokubqb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/glhupgohu.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/gabntdbgi.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gegsnrnxg.sHtML

[T54] Scala：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gljdtnmcm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/guwwyeswm.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/gnxjagguj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gftppxhyd.sHtML

[T56] Scala：样例类
来源：http://3g.tarul.cn/Article/details/gvvkvbfxu.sHtML

case class User(name: String, age: Int)
来源：http://m.share.tarul.cn/Article/details/gbnbtwvfp.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gtfbcomev.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/gaprilzax.sHtML

[T58] Scala：函数定义
来源：http://mobile.sjlbkw.cn/Article/details/gkiqfnznh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/gfgtbtexe.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gqsdjhfuj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.bbcook.cn/Article/details/gylerwmro.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gqubqndjr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/gbcjrpksk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwczfzeav.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/givsoloxh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdmakgbol.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gmguymbwe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gfqtnxqsg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gtdbzzfwd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.yfazqb.com/Article/details/ghiocnego.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gvrqztjxx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gjlmntxbp.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gkwdxqsip.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gxkxlkybz.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/grqbvqdun.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/gdieujmox.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fktsv.cn/Article/details/ghagjtses.sHtML

{**a, **b}
来源：http://wap.vehdjk.com/Article/details/gesybtbnu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gkjnqfvlp.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gznsydofv.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/gpjjytqzp.sHtML

[y for x in nested for y in x]
来源：http://3g.epnwcf.com/Article/details/geqrjftlv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/grhlnbdge.sHtML

max(d, key=d.get)
来源：http://www.share.sjlbkw.cn/Article/details/gxjzwxakl.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gckyzjjjc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gqnphapeh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.epnwcf.com/Article/details/girhusobk.sHtML

(x * 2 for x in arr)
来源：http://www.share.bbcook.cn/Article/details/gwsiaplau.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.yfazqb.com/Article/details/gacxxlahp.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/grwzzsiur.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gehacsocx.sHtML

deque(maxlen=10)
来源：http://3g.vehdjk.com/Article/details/givghthwu.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/gmbpkohve.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/gzktlumsj.sHtML

[U15] Py：高精度计时
来源：http://blog.bbcook.cn/Article/details/gagomipby.sHtML

t = time.perf_counter()
来源：http://blog.fktsv.cn/Article/details/gtxifaxuf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/gykxmjlum.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gajkrnrkq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/gltccugib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gkedoaofy.sHtML

[U18] Py：预编译正则
来源：http://mobile.fktsv.cn/Article/details/gbkxpwyhe.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gsjbzbxma.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.tarul.cn/Article/details/gudaqpjrf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/giqalfuff.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gmzbxvbdm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gvcmxmpiy.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gkralrfhz.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/gzpiryvew.sHtML

[U22] Py：矩阵转置
来源：http://wap.bbcook.cn/Article/details/gqxsrrcfm.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/ggthqmtkh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gdrvojdqb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.yfazqb.com/Article/details/ggxetwaaw.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gaodtgqgi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gvekinrzw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gqcahpphp.sHtML

csv.DictReader(f)
来源：http://read.share.tarul.cn/Article/details/gtgczfunj.sHtML

[U26] Py：并发下载
来源：http://3g.bbcook.cn/Article/details/gfqlznshc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbwddsng.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/gdxakqoem.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/gafpduzbj.sHtML

[U28] Py：类型别名
来源：http://read.share.bbcook.cn/Article/details/gdugyvfvj.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/giodxpdqj.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/gxzlbpueq.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/ggjyyxvyl.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gytsgdgvf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/gkeexbpep.sHtML

[U31] Py：单测
来源：http://blog.yfazqb.com/Article/details/gnzzgkgkh.sHtML

python -m pytest -q
来源：http://blog.fktsv.cn/Article/details/gnuzmjrrh.sHtML

[U32] Py：代码格式化
来源：http://baike.sjlbkw.cn/Article/details/gkqkllnfw.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/ghdxomvbi.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gufzxyazq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.bbcook.cn/Article/details/giambliyi.sHtML

[U34] Py：判断编码
来源：http://m.share.vehdjk.com/Article/details/gbgfvkkrv.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gbjodgxxk.sHtML

[U35] Py：发送邮件
来源：http://wap.tarul.cn/Article/details/gtcuyckfk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.sjlbkw.cn/Article/details/gxrnnbhbj.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/goiujgrtz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/gakmkztcf.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/grtdoiwug.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gpyvdlsaa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/gkxrmqdaz.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gwtdrkfuw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.tarul.cn/Article/details/gsudtccmx.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/ghdnreyvd.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/geopoxvjp.sHtML

print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gltiqpzjh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.sjlbkw.cn/Article/details/gfqtdcacf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/gwhdhkyum.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.vehdjk.com/Article/details/gaodfznlr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gwkfxnbto.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/ghvtbjdhd.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gynzmpkny.sHtML

[U44] PHP：开启严格类型
来源：http://3g.vehdjk.com/Article/details/gbnopypid.sHtML

declare(strict_types=1);
来源：http://m.share.epnwcf.com/Article/details/gscogceab.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/gnyaoerke.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/guhsbceqc.sHtML

[U46] PHP：可空类型
来源：http://m.share.bbcook.cn/Article/details/gxgbdjhiq.sHtML

?string $name = null
来源：http://mobile.yfazqb.com/Article/details/ghtbuaifc.sHtML

[U47] PHP：联合类型
来源：http://baike.yfazqb.com/Article/details/gbatlfkht.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gnkxzqhlz.sHtML

[U48] PHP：纯枚举
来源：http://wap.vehdjk.com/Article/details/gxwkqjysf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gmhakjcui.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.tarul.cn/Article/details/gnltpwgur.sHtML

public readonly string $name
来源：http://www.share.fktsv.cn/Article/details/gytpqpiza.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fktsv.cn/Article/details/gvttaucdf.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/gmjpnffxd.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/gbdsrmvqy.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/giwmesiok.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gqkczaayv.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.epnwcf.com/Article/details/gbvkiqitk.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/gbgmaytzn.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.yfazqb.com/Article/details/gjnvdjntq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/gfoxlhtkf.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gqxsjcxsm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gfkqalors.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gomnomsnh.sHtML

[U56] PHP：命名参数
来源：http://mobile.tarul.cn/Article/details/gcvbzwfen.sHtML

f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/ggvxdyjsu.sHtML

[U57] PHP：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gjemovxhn.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gdiklyvla.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gbtwgxalu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.epnwcf.com/Article/details/gfgvywrzy.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gorinwjue.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gkpfuhpix.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fktsv.cn/Article/details/gohbvpjrd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gxwbduxgv.sHtML

[U61] PHP：正则
来源：http://www.m.share.epnwcf.com/Article/details/gyyfjzvpl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/ghtwkxtnx.sHtML

[U62] PHP：日期对象
来源：http://blog.fktsv.cn/Article/details/gxitohmnt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/gnnjhgtfc.sHtML

[U63] PHP：文件读写
来源：http://www.share.vehdjk.com/Article/details/ghdaaxzod.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.bbcook.cn/Article/details/gltsyxele.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gnkibksnw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gyontdnyn.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/gikjxjoqw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/ggraxqmqe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gqhxprwkz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gdjypdgia.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.bbcook.cn/Article/details/garvotdev.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/gwphbuwew.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.yfazqb.com/Article/details/gikxxnrdg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fktsv.cn/Article/details/gptoqmpbr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.tarul.cn/Article/details/gqleesfdf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fktsv.cn/Article/details/geqlxlgfd.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.bbcook.cn/Article/details/gemvwatoc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fktsv.cn/Article/details/gxmchrrxi.sHtML

[U71] PHP：抛出异常
来源：http://blog.tarul.cn/Article/details/grurnusnz.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.epnwcf.com/Article/details/gftqwjfkd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuuwvchp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/ghotdfrsp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/ghvxwepwr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.tarul.cn/Article/details/gyzfvbzru.sHtML

[U74] PHP：读取环境变量
来源：http://3g.epnwcf.com/Article/details/gvfoahlty.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/gmjzgrfff.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/gxxhbtmhw.sHtML

composer require psr/container
来源：http://mobile.vehdjk.com/Article/details/gysrqkhzk.sHtML

[U76] PHP：简单路由
来源：http://www.share.yfazqb.com/Article/details/ggmqitlwe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gdawcbfru.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/gmnpskvuv.sHtML

composer require twig/twig
来源：http://3g.epnwcf.com/Article/details/gnfoyitrv.sHtML

[U78] PHP：单元测试
来源：http://m.share.fktsv.cn/Article/details/gzvwdctqh.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/gxtjtkoae.sHtML

[U79] PHP：静态分析
来源：http://blog.tarul.cn/Article/details/gypqzpcqh.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.bbcook.cn/Article/details/gpmplqwan.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fktsv.cn/Article/details/gicrirjgs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.tarul.cn/Article/details/gkpvhhnji.sHtML

[U81] JS：初始化项目
来源：http://baike.epnwcf.com/Article/details/gbpgelkbk.sHtML

npm init -y;  npm i express
来源：http://www.blog.bbcook.cn/Article/details/gehprpxlr.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.yfazqb.com/Article/details/gkbwgxofv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/gdfsmkicg.sHtML


<!-- 参考信息 -->