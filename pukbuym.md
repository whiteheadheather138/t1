代发 wailian999

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/glkdxcpun.sHtML

[S53] C++：移动语义
来源：http://3g.bbcook.cn/Article/details/gxayevbls.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gtdvvppha.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/goewdsvfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gglqxkrhy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gtqdjnydq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gjiscnhqj.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/grrvqdthn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gqvaqzmnx.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gokbveylq.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gutoguwbg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gmbdflsfr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gqsryesyd.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gebfzqyhf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gavvsvbql.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/gjoglfwjm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gdbtthtkx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqpmkaynr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gsicsynrn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmujrnses.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gqyswxbmf.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gvzbfectq.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gqvflowop.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gyerwgyzu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gwsmbevpd.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gwhfsgzml.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gbhxeidrb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gnpztmkll.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gmrhhsayu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/grrancgke.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gsthtsqsn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gwplzboyq.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gfgrbcxfm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/ggytfnmcl.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/ghiazysbo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gihozmcib.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gpqysuhox.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gurcqzbqp.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gjoumcwqv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gkarknnnh.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gbohfnxaw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gkpszkalb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gpfqophgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gotsgqrnm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/gfhwfrmdc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/gmqlqqfwn.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gddwdkgsl.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gajamaqsm.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/gaeaejzjw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/ggmkaeyni.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gmsjkkuva.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gluyypnzu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gvbymkawr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/gxgmjvxnx.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gyubnbqeo.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gwiufmowc.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gzxktinch.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/glhieakoi.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/giugcfibm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gibihrxfw.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gopoziqhl.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/ggfkiccka.sHtML

[T22] Swift：字典
来源：http://blog.sjlbkw.cn/Article/details/gdbyvsmmi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/gvtidkjwz.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/gmzwxmvuw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gnawizwax.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/gkzrhlsif.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gixsudnmt.sHtML

[T25] Swift：结构体
来源：http://m.share.fktsv.cn/Article/details/gjluejrxu.sHtML

struct P { var x: Int }
来源：http://www.blog.yfazqb.com/Article/details/gbfyjrpno.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gvxfuawnd.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/gserhdwbz.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gesiwfnyw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/ghjlwvigt.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/ggpkalmlg.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gjnrjftxy.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gpxomvtxw.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gsdveffcc.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/gxpxozhnn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.vehdjk.com/Article/details/gsbcwwntf.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/gksvopuap.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gsurfbgzl.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gxpgvlxmv.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/gemivslhg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gwltkdfts.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gulqevbfb.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/ggpvchzks.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/gigsbeqyz.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/ggqanmwdl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/ghavygoel.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gydexrlqj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fktsv.cn/Article/details/grzbskkbd.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gtwfwfprp.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/guozdiywg.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gtajghwyb.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/gtioihnou.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gkdwqsuqp.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/ggztwcdjl.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gixbofrtx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.vehdjk.com/Article/details/gcjnjbmfw.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gyuexegmg.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/gffkcbtiu.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/giaepsppo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fktsv.cn/Article/details/gyqurzgqa.sHtML

[T43] Perl：字符串插值
来源：http://blog.bbcook.cn/Article/details/gobytrryj.sHtML

"值: $a"
来源：http://www.blog.yfazqb.com/Article/details/gxixwkolv.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gpvmlgjya.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gdofrllwq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/gjfmdfyvq.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.sjlbkw.cn/Article/details/gjipmcicd.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gskvbxzar.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/gdlawggev.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gdcirfyar.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gukiazyrp.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gfyvipwxr.sHtML

$s =~ s/old/new/g;
来源：http://wap.epnwcf.com/Article/details/gtyigkaud.sHtML

[T49] Perl：函数
来源：http://read.share.yfazqb.com/Article/details/gxtszlnwh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.tarul.cn/Article/details/ggpewxyod.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gzsifexlc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.bbcook.cn/Article/details/guaucalgh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fktsv.cn/Article/details/guchhxnxz.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/gimjghipi.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gppuzmipl.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gltinwkcs.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gizqxfwmo.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gltccrdmj.sHtML

s"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gmcdgooop.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gukjzbkfz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gjdnvyusq.sHtML

[T55] Scala：集合过滤
来源：http://blog.fktsv.cn/Article/details/gorssxgth.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/ghsafhhrn.sHtML

[T56] Scala：样例类
来源：http://baike.sjlbkw.cn/Article/details/glkfagxbo.sHtML

case class User(name: String, age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gomhsdvgw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gpozstroq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/gaicgwtvt.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gqdqpssvy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.epnwcf.com/Article/details/gdfzhwycb.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gleegrklo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gnwbbsbwm.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gnrqddkzr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/gvvswqpyq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gslqbefpt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/guptcevvh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggynnhunf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fktsv.cn/Article/details/gzbbbfdjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/guvpktzgk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/guwkhaygj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gzqebxjhm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/glssotbks.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.tarul.cn/Article/details/ggicytqlj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.epnwcf.com/Article/details/gyqtjfmdv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/gpxqtklvn.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fktsv.cn/Article/details/gojmhbinn.sHtML

list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gpffewdcr.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gruglhear.sHtML

{**a, **b}
来源：http://www.m.share.vehdjk.com/Article/details/ghabnvaby.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gisegkojk.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/gafitrvsf.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gusyxzrib.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gllqtvpao.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gqbczwinv.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/ggymhugsb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.yfazqb.com/Article/details/gqhokiuka.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.tarul.cn/Article/details/gmmblsezt.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/glgedzusi.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/guixmgiau.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gfmgaeatd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fktsv.cn/Article/details/ggjtvbjbt.sHtML

[U13] Py：固定长度队列
来源：http://mobile.sjlbkw.cn/Article/details/guyjwumxt.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/goykoabrc.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/gqsmxypvj.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gfhwqshrw.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/geequjqhk.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gtsyyfqoh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/gixgizdsq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fktsv.cn/Article/details/gaublhbuv.sHtML

[U17] Py：初始化日志
来源：http://m.share.fktsv.cn/Article/details/gdyhlfonu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.yfazqb.com/Article/details/goulsjakt.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/gycgwisyt.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.tarul.cn/Article/details/gmhvkltft.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/gjwtrkgpa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/gpdivhozn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.bbcook.cn/Article/details/gcsjjrfni.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gttsmtmge.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gzttdbqgs.sHtML

@contextlib.contextmanager
来源：http://m.share.bbcook.cn/Article/details/gvgmgyyil.sHtML

[U22] Py：矩阵转置
来源：http://mobile.yfazqb.com/Article/details/gcbjgobfc.sHtML

list(zip(*m))
来源：http://www.blog.tarul.cn/Article/details/gvienpmxd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/gekcjtcay.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gfzviwwtu.sHtML

[U24] Py：路径操作
来源：http://3g.sjlbkw.cn/Article/details/gurujncda.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gnbkhqkop.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gywxjybmy.sHtML

csv.DictReader(f)
来源：http://read.share.fktsv.cn/Article/details/glczocyya.sHtML

[U26] Py：并发下载
来源：http://baike.epnwcf.com/Article/details/gnngcasrx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.yfazqb.com/Article/details/gwlknmxti.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/gsgwzrksa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/gygfeambt.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gfadgefwr.sHtML

UserId = int
来源：http://mobile.tarul.cn/Article/details/gycwvyibw.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gewbwgbsb.sHtML

@property 与 @x.setter 配合
来源：http://blog.fktsv.cn/Article/details/gkmvzxeak.sHtML

[U30] Py：数据类
来源：http://mobile.tarul.cn/Article/details/ghvrumotw.sHtML

@dataclass(slots=True)
来源：http://www.blog.epnwcf.com/Article/details/gvygxyqwk.sHtML

[U31] Py：单测
来源：http://m.share.fktsv.cn/Article/details/gbgcvmpuv.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/giaxhomsk.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/gjgyfaila.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gmudwqmwh.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gmveiffbb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gvhoxvslb.sHtML

[U34] Py：判断编码
来源：http://www.m.share.yfazqb.com/Article/details/gbskpbyph.sHtML

chardet.detect(raw)
来源：http://m.share.fktsv.cn/Article/details/gndfnowmd.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/giptedtqh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.epnwcf.com/Article/details/grcirudqk.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gzwpjfkut.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gwiguajjr.sHtML

[U37] Py：读写 Excel
来源：http://baike.fktsv.cn/Article/details/ghfxaeksf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/gelqmkdoh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/gsqigxjlk.sHtML

Path(__file__).resolve().parent
来源：http://m.share.epnwcf.com/Article/details/gvyiyzjdb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/gowoghuna.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/gvvivlmta.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.tarul.cn/Article/details/gvnoodjbi.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gagtxsfrq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gmvtpupau.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/gmlmyogzp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/gjeuxawml.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.yfazqb.com/Article/details/gcmzlyyuh.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/gmcbejypy.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/gqmgfpdbv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.epnwcf.com/Article/details/glimjrbpo.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gjphmpqzx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.tarul.cn/Article/details/gigcsgziu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gvndyqxqx.sHtML

[U46] PHP：可空类型
来源：http://blog.yfazqb.com/Article/details/gtgebfxwe.sHtML

?string $name = null
来源：http://www.blog.yfazqb.com/Article/details/gyvuevbei.sHtML

[U47] PHP：联合类型
来源：http://blog.yfazqb.com/Article/details/gbbnstfox.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gtppuluyj.sHtML

[U48] PHP：纯枚举
来源：http://mobile.sjlbkw.cn/Article/details/goemupdgo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/glnhwvtgk.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.yfazqb.com/Article/details/gxpadeorq.sHtML

public readonly string $name
来源：http://mobile.yfazqb.com/Article/details/grzfrwsrl.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/gkmbsgwav.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.tarul.cn/Article/details/gahexphct.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/geyjpsaoy.sHtML

[$a, $b] = $arr;
来源：http://baike.bbcook.cn/Article/details/ghmpapofu.sHtML

[U52] PHP：箭头函数
来源：http://mobile.tarul.cn/Article/details/gimuujnhv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gqccxobbs.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gxymbmbzp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.tarul.cn/Article/details/ghtgbfsie.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gzznnptcl.sHtML

$obj?->method()
来源：http://mobile.yfazqb.com/Article/details/gvxmxndua.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/gblqnoipe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gupcpzolg.sHtML

[U56] PHP：命名参数
来源：http://wap.fktsv.cn/Article/details/gzyuckqao.sHtML

f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/giwimlpme.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gpyffyhiv.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/gqymgstwx.sHtML

[U58] PHP：数组三件套
来源：http://mobile.tarul.cn/Article/details/gqxsaxxxp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gecepcing.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gkqdwnpbz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/glfmbjucf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.yfazqb.com/Article/details/gpkirhcnk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fktsv.cn/Article/details/gzjwilage.sHtML

[U61] PHP：正则
来源：http://wap.bbcook.cn/Article/details/gfnvmynxp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/guzwbsdrk.sHtML

[U62] PHP：日期对象
来源：http://3g.yfazqb.com/Article/details/gjnvaqjfs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/ghfvbfdcn.sHtML

[U63] PHP：文件读写
来源：http://www.blog.bbcook.cn/Article/details/gqxhzwocn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.tarul.cn/Article/details/gitnnnejz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/grcbqynnc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gsjjdozlb.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/gtsdughxn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gcswxhpyz.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.yfazqb.com/Article/details/gbezfolho.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gjcowglus.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/ghxzljgjc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.sjlbkw.cn/Article/details/ghupzxvyv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gjsnelywo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.tarul.cn/Article/details/gcnzaplts.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.vehdjk.com/Article/details/gvdunjwmt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.epnwcf.com/Article/details/gmmixtryn.sHtML

[U70] PHP：PDO 事务
来源：http://blog.bbcook.cn/Article/details/gyhrnycom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.vehdjk.com/Article/details/ggwrzcban.sHtML

[U71] PHP：抛出异常
来源：http://wap.fktsv.cn/Article/details/giwlrymzb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.tarul.cn/Article/details/gmuuocanl.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gpxrdspcs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.vehdjk.com/Article/details/gcmspyrgf.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/ggyqugnwr.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.vehdjk.com/Article/details/gpyallmlg.sHtML

[U74] PHP：读取环境变量
来源：http://baike.yfazqb.com/Article/details/gdnsfrpfb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/gctyxoqxb.sHtML

[U75] PHP：依赖注入
来源：http://read.share.sjlbkw.cn/Article/details/gmtfchilr.sHtML

composer require psr/container
来源：http://www.m.share.epnwcf.com/Article/details/gaftqceju.sHtML

[U76] PHP：简单路由
来源：http://www.blog.vehdjk.com/Article/details/ghfbmfqzj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/gkywpylpt.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/galgvcohx.sHtML

composer require twig/twig
来源：http://wap.yfazqb.com/Article/details/guckxlntn.sHtML

[U78] PHP：单元测试
来源：http://read.share.epnwcf.com/Article/details/grwftklnv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.yfazqb.com/Article/details/ggpvpcraf.sHtML


<!-- 参考信息 -->