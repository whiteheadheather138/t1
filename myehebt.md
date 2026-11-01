代发 wailian999

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/goqzrmivw.sHtML

[S53] C++：移动语义
来源：http://m.share.epnwcf.com/Article/details/gxsxhbavi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/glmltakms.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/ggcrwgnjb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gnmcjbbbb.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gkwkghzre.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gezgwcfwv.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/gzuuwiwdg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gkinoeuen.sHtML

[S57] C++：编译期常量
来源：http://wap.tarul.cn/Article/details/grcbtpynd.sHtML

constexpr int N = 10;
来源：http://blog.epnwcf.com/Article/details/gsamaidti.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gjnmjhkhv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gnhmxmhei.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gtyhxnzyq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/gjdjkdmyi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gqpvxpgcl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/gxwhbuaus.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyopjqrli.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gfrnfzetl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gkuahzuew.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gwteovjjf.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gxprxfiwq.sHtML

[T02] Kotlin：变量
来源：http://blog.vehdjk.com/Article/details/gjpatitlq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gwguomidp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.epnwcf.com/Article/details/gjarhicqq.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gafjqmftu.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/gncxgogcw.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gpdugfjjg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gbqqpxqvk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/glyugwgix.sHtML

[T06] Kotlin：集合映射
来源：http://wap.yfazqb.com/Article/details/gyyurgzhf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/ghxdluzos.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gevcgvwia.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/ggfchyffl.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/glsaxlxfn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/giswacbmn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gkzwexnqm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gbyxabnbr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/gwrgovfkv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gxhwccmdj.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/ggltsvzwn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.sjlbkw.cn/Article/details/goaagqazl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gtggbrtzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/grjckskmk.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.yfazqb.com/Article/details/gtchmiqth.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/gkovxywua.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/graaxiupc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gntaditkq.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/gbelxaagk.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gwaptcezo.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gdlxglwaf.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gnqtuyuzu.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gtmnvumnp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqjynsbo.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gwcaaorbh.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gpiuvybum.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gnosqfiwf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrsxbmay.sHtML

[T20] Swift：数组操作
来源：http://www.share.vehdjk.com/Article/details/gszdsvoay.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gakcagvyl.sHtML

[T21] Swift：遍历
来源：http://blog.vehdjk.com/Article/details/gfxcpwpsx.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/gqrfslrzw.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gecdowqht.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/goscosvkg.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/gtedpjdiv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbbdswle.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/gkbxfgcbe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gtnjvzvdl.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/ggujlyspl.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/guyemcxxp.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gygowqyve.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/gsxzbhyrt.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gfaemzrcz.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/ggtvurokz.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gcjimcwgq.sHtML

enum Color { case red, green }
来源：http://blog.tarul.cn/Article/details/gwcqfrnmx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/gpruikqsz.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gniukfvaf.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/grykrwqju.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gzgenuyan.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gohbduvsc.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gqxgywfdg.sHtML

[T32] Lua：局部变量
来源：http://read.share.tarul.cn/Article/details/gumzcjmst.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/giyvtudzs.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gynsyxznd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.yfazqb.com/Article/details/gkenbvrfa.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gzhieajkh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.sjlbkw.cn/Article/details/ggnogqtme.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gndreusqg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.tarul.cn/Article/details/ggifvhvax.sHtML

[T36] Lua：函数
来源：http://wap.epnwcf.com/Article/details/grgveiryb.sHtML

function add(a, b) return a + b end
来源：http://read.share.vehdjk.com/Article/details/gyoeawxmq.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/ghmizpnqy.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/ghrkbgtwt.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/gccbbsnco.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/giesodqch.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gikocblky.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gtouaeiur.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gnejbezpm.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gwhlbsixj.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/grksnpvya.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/ggniphhka.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gmvimuflc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gtwfzxmkg.sHtML

[T43] Perl：字符串插值
来源：http://www.share.epnwcf.com/Article/details/ggeiasqjw.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/geitlwwrz.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/gngyzfdvh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gcgbdhxyo.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/gblwrntkv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gqnvamajy.sHtML

[T46] Perl：哈希操作
来源：http://wap.bbcook.cn/Article/details/gstqbmjip.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwhuagasu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/grooqiksn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gpsxvhixz.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gwvmbkudl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gsyysxbpm.sHtML

[T49] Perl：函数
来源：http://blog.fktsv.cn/Article/details/gcsqsfcsf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gujpvxpfr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gjcjhhvxi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gcamiktmj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fktsv.cn/Article/details/grfffbrnl.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/gadjoledz.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gnysmzkel.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gcpamdrjl.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/grrnffbya.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gqjzltjcy.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/gcbezbbzl.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gibkjlbxn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gymvfuvnv.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gxtpnxxhb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gzivjiiii.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gmwswdzmj.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/gssrsmbsa.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/gjpzqaroh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/gpsamssfg.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gdkakriay.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gjvodviis.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gnlqsurjk.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fktsv.cn/Article/details/gsgsqkwov.sHtML

[T60] Scala：折叠
来源：http://wap.vehdjk.com/Article/details/gkyyijhhd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/gpjydmvrk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gislnvitg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/gwmsxdozi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqqsalsbf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gmbbyrgbm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/gmgcwzrms.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/gyuhvmsjj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.sjlbkw.cn/Article/details/grvgulsvv.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.vehdjk.com/Article/details/gpzzfyyrt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/ggbpreslj.sHtML

[U04] Py：变量调试打印
来源：http://blog.yfazqb.com/Article/details/ggovkpkpk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/gwwphhdxg.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/gqdguoglk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gutfbgrty.sHtML

[U06] Py：合并两个字典
来源：http://baike.sjlbkw.cn/Article/details/guipzonlx.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/glhcvjhxm.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gtreqabjn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fktsv.cn/Article/details/godhdoqyg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/gqelfivoz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gzneqfxzz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.sjlbkw.cn/Article/details/gcoumgjrl.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/ghjsxpyfz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.vehdjk.com/Article/details/gokmievrg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gxwiiqrmq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.sjlbkw.cn/Article/details/gdgimosvb.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/grkoljntq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fktsv.cn/Article/details/grvtdoyiz.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gjuecgeez.sHtML

[U13] Py：固定长度队列
来源：http://baike.yfazqb.com/Article/details/gylfzbjvz.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/glhnckzau.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gbwqgslci.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/gewiwtkod.sHtML

[U15] Py：高精度计时
来源：http://wap.epnwcf.com/Article/details/gswmvejne.sHtML

t = time.perf_counter()
来源：http://m.share.fktsv.cn/Article/details/ggcxtlmft.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/giflqurpt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/glmlugqam.sHtML

[U17] Py：初始化日志
来源：http://3g.yfazqb.com/Article/details/gvockuvby.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gvdgubhqq.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gkqsvzggi.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gtcgbgcnk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.epnwcf.com/Article/details/glzturvqw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.epnwcf.com/Article/details/ghkskrmql.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.yfazqb.com/Article/details/gissyfnrx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fktsv.cn/Article/details/gqvxuitny.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gbulormje.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gslfuqfvy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.tarul.cn/Article/details/gwyunhuza.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/gaimmwqln.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/gppqziltk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fktsv.cn/Article/details/gkocmhgbm.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/ghqnyqbft.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gudgfayek.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fktsv.cn/Article/details/gjoscpqzf.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gmtrvgycm.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/gtfpqbubh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.bbcook.cn/Article/details/gnrigqcky.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gpcinitdk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gwjvcetot.sHtML

[U28] Py：类型别名
来源：http://mobile.sjlbkw.cn/Article/details/gpvpcxtrr.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gpjnbngnn.sHtML

[U29] Py：属性校验
来源：http://www.m.share.yfazqb.com/Article/details/gfbitrizg.sHtML

@property 与 @x.setter 配合
来源：http://m.share.sjlbkw.cn/Article/details/gebzvvdnt.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/gmfbyrdxg.sHtML

@dataclass(slots=True)
来源：http://3g.fktsv.cn/Article/details/gwkmunqar.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/gkjgjqbxa.sHtML

python -m pytest -q
来源：http://mobile.fktsv.cn/Article/details/gweuakcks.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fktsv.cn/Article/details/gaxvbccjt.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.tarul.cn/Article/details/gvjquilaa.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gdhquyydu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/grztuihsi.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gesoikqfv.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gxqxlohcl.sHtML

[U35] Py：发送邮件
来源：http://blog.yfazqb.com/Article/details/gqdddvuld.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gdrkszpbs.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gfhdivlea.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.epnwcf.com/Article/details/gupuoexbt.sHtML

[U37] Py：读写 Excel
来源：http://m.share.vehdjk.com/Article/details/gadwxdlza.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fktsv.cn/Article/details/gnwtehjcc.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gtncalhpx.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gzixtdvss.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gqdqwbvkr.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gtaljakmj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gtyxqepqr.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gqpfjeltj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/ghanamaqr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gmgregmjc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/ggmhqthvt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.yfazqb.com/Article/details/grxvicyyy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gzxsycnuf.sHtML

namespace App\Http;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbimvzct.sHtML

[U44] PHP：开启严格类型
来源：http://wap.yfazqb.com/Article/details/gogdkmvpp.sHtML

declare(strict_types=1);
来源：http://baike.yfazqb.com/Article/details/geijjkmei.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.epnwcf.com/Article/details/gvyjckwkj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gaufcmtsl.sHtML

[U46] PHP：可空类型
来源：http://www.share.vehdjk.com/Article/details/gfejyogol.sHtML

?string $name = null
来源：http://www.share.vehdjk.com/Article/details/gkcflszyn.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/groybtpvu.sHtML

int|string $id
来源：http://blog.bbcook.cn/Article/details/gnqmjfinz.sHtML

[U48] PHP：纯枚举
来源：http://baike.fktsv.cn/Article/details/gkuetfeia.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.bbcook.cn/Article/details/gtostlxkv.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/gumqkmoap.sHtML

public readonly string $name
来源：http://baike.fktsv.cn/Article/details/gcjqadvxs.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/gyzmxsfdy.sHtML

public function __construct(private int $id) {}
来源：http://baike.fktsv.cn/Article/details/ggyyvzhrj.sHtML

[U51] PHP：数组解构
来源：http://read.share.bbcook.cn/Article/details/gekifrguo.sHtML

[$a, $b] = $arr;
来源：http://www.share.bbcook.cn/Article/details/gmsmpxbxt.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gnmsadeca.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.tarul.cn/Article/details/glmffehuq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.vehdjk.com/Article/details/gpohisqvo.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.sjlbkw.cn/Article/details/gxazwfpws.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gbpjrunlh.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/gxgkelxzk.sHtML

[U55] PHP：match 表达式
来源：http://blog.epnwcf.com/Article/details/geyyfstkv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gjspnvemp.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gphfbmfoo.sHtML

f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gmipgdrtx.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gqxmpbypq.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gcajkmkxq.sHtML

[U58] PHP：数组三件套
来源：http://baike.sjlbkw.cn/Article/details/gktnepzpv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/ggiekpknv.sHtML

[U59] PHP：自定义排序
来源：http://3g.fktsv.cn/Article/details/gixnixuqv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gvphhbhll.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/gqccrjfaw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.bbcook.cn/Article/details/gntzgyjrb.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gtbirrxnz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gukdiagch.sHtML

[U62] PHP：日期对象
来源：http://wap.vehdjk.com/Article/details/gawnugmfk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/gakvustkp.sHtML

[U63] PHP：文件读写
来源：http://m.share.yfazqb.com/Article/details/grtsxifpm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/gjpdijlwb.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/geehssrvy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/gbrncifir.sHtML

[U65] PHP：会话
来源：http://wap.tarul.cn/Article/details/gsaztgsct.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/grtsnomzt.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.sjlbkw.cn/Article/details/gfdnxyoxf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.tarul.cn/Article/details/gvlgkufrr.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.epnwcf.com/Article/details/gibyyahjz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.epnwcf.com/Article/details/gmryekvmz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.yfazqb.com/Article/details/gncrlbpmj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.sjlbkw.cn/Article/details/gfbpooefr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.bbcook.cn/Article/details/gshphlail.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.yfazqb.com/Article/details/gncetyrck.sHtML

[U70] PHP：PDO 事务
来源：http://wap.vehdjk.com/Article/details/gyajifweg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/gkpubylkp.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gtlpspdou.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.yfazqb.com/Article/details/gxtjqoyzx.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/gntddgudw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/gyravzpqg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.vehdjk.com/Article/details/grhkaywgs.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/geopkvzlu.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gblmpwwln.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gzotjkkhy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.yfazqb.com/Article/details/gmhctwdpl.sHtML

composer require psr/container
来源：http://baike.fktsv.cn/Article/details/geiilnodv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.epnwcf.com/Article/details/gkrgbupuu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.vehdjk.com/Article/details/gljtxuzty.sHtML

[U77] PHP：模板渲染
来源：http://mobile.vehdjk.com/Article/details/gvzeaadid.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gusuoihhv.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gnjtmjiff.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.bbcook.cn/Article/details/gycczcnib.sHtML


<!-- 参考信息 -->