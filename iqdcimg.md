代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gorcjtejh.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gyheclmls.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gqdnsohvu.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gjsjmgnti.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gmmyzfirr.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/guenwrbxx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/gaazsykgr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.sjlbkw.cn/Article/details/gzebcupup.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/ggniuohoi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/godwtiysb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gnwhajjia.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbfprsoqb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gldjfcycg.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gydabxskv.sHtML

[T02] Kotlin：变量
来源：http://read.share.sjlbkw.cn/Article/details/gewimdvnd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/gzyhfmerv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gcuasbqei.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/ghzivbupl.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/goufnabbq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/glrllwtiw.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/gobnadhib.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gguzswmel.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/giejsklxr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gxqwomsxh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gbuvjcfml.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gdmigniks.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gjhhwbvuy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gingfaqdv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gqsxmvuli.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gtrdkmwwo.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gwdlywnqc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/gqoamxwvu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gmaofbxbz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gtixibgxe.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gkxycalke.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gjsuysgrl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gmmhqwgpp.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/giuyefffq.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gxodtekqb.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gltkijmgp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gcfrjouds.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/gdklujeyz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gfdewaqdt.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gzlmatzvn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/gdbbuzzmp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gmmpcgvul.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gvakmwsqh.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gojowbgwv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gehugqujs.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gqrloasal.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtzjxdxi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.tarul.cn/Article/details/guhhgybhb.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/gdaghnnat.sHtML

for x in a { print(x) }
来源：http://read.share.bbcook.cn/Article/details/gllpnwoji.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/ghgwmbijw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/gskkxlewm.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gzfjcucqn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gweimhkxz.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gztcakkni.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/grwqmtnrk.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/gtgtwwdvm.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/glqrqzzvw.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gxupnegnd.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gemykapfc.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/ginndlbet.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gnsnenprg.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkasdoac.sHtML

enum Color { case red, green }
来源：http://read.share.epnwcf.com/Article/details/gxyvaclip.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gyxlxngwa.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gfjybtdrv.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gsqhuunay.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/gdkvqmjgn.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/gkoypmipx.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/ghfppavtu.sHtML

[T32] Lua：局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gxntwbrjn.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gpujxnxrj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gqzddmscw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gqtrbdozk.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/gvgthninb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gdjjwrmuh.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/ggfjjljrm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.sjlbkw.cn/Article/details/gvtljalgy.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gsyngucmt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.tarul.cn/Article/details/gcvejymgv.sHtML

[T37] Lua：字符串拼接
来源：http://wap.yfazqb.com/Article/details/ghjebuufa.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/giwcderqv.sHtML

[T38] Lua：条件
来源：http://m.share.epnwcf.com/Article/details/gxuozirvo.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/gkjpoewjd.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/gshfjckuw.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/gxufoqmey.sHtML

[T40] Lua：元表
来源：http://read.share.tarul.cn/Article/details/gvhoedmej.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/gcnfevplc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/gephfqqxv.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gwdocksww.sHtML

[T42] Perl：变量类型
来源：http://www.blog.yfazqb.com/Article/details/gsadfxywe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/gglpjfbey.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gyfjvgbkz.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gfyxlorsi.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gfdqliqky.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.yfazqb.com/Article/details/gxdgwjhdi.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gagqflgck.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.sjlbkw.cn/Article/details/gmdcfnerp.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/golgjhrby.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/gdnprzgmt.sHtML

[T47] Perl：正则捕获
来源：http://mobile.sjlbkw.cn/Article/details/gzurntocr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/ghlmtveeq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gvfufvfcz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/giucilwuc.sHtML

[T49] Perl：函数
来源：http://blog.sjlbkw.cn/Article/details/gbakyhbai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gfeetygkf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/ggsoadbtf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.tarul.cn/Article/details/gmcuvfrci.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/glxnlvuku.sHtML

[T51] Scala：Hello World
来源：http://3g.fktsv.cn/Article/details/gyqfphxpp.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gfpnosvyk.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gajhigrcr.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/gbirbnizy.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gsdlryrsy.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gcodwtpwf.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gztvfpdlo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.vehdjk.com/Article/details/gbqfssqvh.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/ggitauscy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/gboyrcuie.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/ghlumcihg.sHtML

case class User(name: String, age: Int)
来源：http://wap.vehdjk.com/Article/details/gbrdlvvut.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gtazeqndq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gyzgenrza.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/gwdhxqezy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fktsv.cn/Article/details/gppelkpyd.sHtML

[T59] Scala：循环
来源：http://www.blog.fktsv.cn/Article/details/ghwoarjkd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/glhnyxhks.sHtML

[T60] Scala：折叠
来源：http://www.share.yfazqb.com/Article/details/gyhorthul.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fktsv.cn/Article/details/gxdzcxeog.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjcwucjtl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/ggtipuzna.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyqsntocc.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/geoapfbfk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fktsv.cn/Article/details/gdelhhyxm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fktsv.cn/Article/details/grfymphxf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gzaecobpd.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.sjlbkw.cn/Article/details/gfqcpnctf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/gwkugwfcj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gttcppjlk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/gnvgzhqgm.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gpuczifcb.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gxekihwgr.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.epnwcf.com/Article/details/gbabqqfhb.sHtML

{**a, **b}
来源：http://blog.fktsv.cn/Article/details/gnfnodxfw.sHtML

[U07] Py：反转字典键值
来源：http://wap.yfazqb.com/Article/details/gchcymdfd.sHtML

{v: k for k, v in d.items()}
来源：http://baike.vehdjk.com/Article/details/gzuezfhet.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gffpdilek.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gmdzzahdy.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gnfvbgdgv.sHtML

max(d, key=d.get)
来源：http://3g.epnwcf.com/Article/details/guodpzoxd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/guckmfsyr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gbyjghgwb.sHtML

[U11] Py：生成器表达式
来源：http://wap.sjlbkw.cn/Article/details/gnoaygqmp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxqzbkxhu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/gmccepcdj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/gcslvsuoc.sHtML

[U13] Py：固定长度队列
来源：http://blog.bbcook.cn/Article/details/gfwadltfh.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gkvhhdtzk.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/gbykhzlpn.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/gyksctjew.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/ghnezksma.sHtML

t = time.perf_counter()
来源：http://3g.bbcook.cn/Article/details/ghsnpcrsv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gdlonznfm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.yfazqb.com/Article/details/gozujmmmo.sHtML

[U17] Py：初始化日志
来源：http://mobile.bbcook.cn/Article/details/gxunbcxqe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gszensuwx.sHtML

[U18] Py：预编译正则
来源：http://www.share.fktsv.cn/Article/details/gnpdlnass.sHtML

pat = re.compile(r"\d+")
来源：http://baike.yfazqb.com/Article/details/gcgxeobxg.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.vehdjk.com/Article/details/gaxunahav.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.epnwcf.com/Article/details/gvktcavad.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.sjlbkw.cn/Article/details/gqbuxdgpy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/ggbuenpzm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.sjlbkw.cn/Article/details/gyhoutfrq.sHtML

@contextlib.contextmanager
来源：http://3g.sjlbkw.cn/Article/details/giracaseg.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gurabquoq.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gexfuzrrb.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.tarul.cn/Article/details/gushwnbwj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.vehdjk.com/Article/details/gyamwkqvb.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gzqmxhafv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gfizdjsyu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/gxpkkavit.sHtML

csv.DictReader(f)
来源：http://www.m.share.bbcook.cn/Article/details/grdcehtge.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/glhhvnxge.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.sjlbkw.cn/Article/details/gfctkmieb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.vehdjk.com/Article/details/gdcmcholl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/gxxymmcfs.sHtML

[U28] Py：类型别名
来源：http://blog.bbcook.cn/Article/details/gfvrmnmyq.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/getjhyccy.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/gzbdpmmyw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fktsv.cn/Article/details/ganfoelft.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gqamtefmq.sHtML

@dataclass(slots=True)
来源：http://m.share.yfazqb.com/Article/details/gatgzbeng.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/guzyyavcz.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/guosiufyt.sHtML

[U32] Py：代码格式化
来源：http://wap.epnwcf.com/Article/details/gfnuqlfcy.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.epnwcf.com/Article/details/gbfxtmnox.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gllqmjvyr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/grcwanhdn.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/gghkasast.sHtML

chardet.detect(raw)
来源：http://www.blog.epnwcf.com/Article/details/gmfzlftwi.sHtML

[U35] Py：发送邮件
来源：http://www.share.sjlbkw.cn/Article/details/gjamiewlj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.sjlbkw.cn/Article/details/gayrkeuzr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/ggxyrkjpx.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/ggmejryws.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/gkbqpmgay.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.bbcook.cn/Article/details/gutqmdozk.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.bbcook.cn/Article/details/gdqtkkvhu.sHtML

Path(__file__).resolve().parent
来源：http://mobile.vehdjk.com/Article/details/gbddzinjm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.tarul.cn/Article/details/gnxxoybud.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gfawioapk.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/ginmzpjei.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gicdzdizt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.tarul.cn/Article/details/gmmrcnmhy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.vehdjk.com/Article/details/gajxmivsa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/gurctzknv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.vehdjk.com/Article/details/gcrzdarby.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/gzgjjslux.sHtML

namespace App\Http;
来源：http://wap.vehdjk.com/Article/details/gtlvawovy.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/goyfktatf.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gcrwzfmjo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/gfjpngaxu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gzuzxeapg.sHtML

[U46] PHP：可空类型
来源：http://m.share.vehdjk.com/Article/details/gwffjfsem.sHtML

?string $name = null
来源：http://3g.vehdjk.com/Article/details/grcfyttah.sHtML

[U47] PHP：联合类型
来源：http://m.share.yfazqb.com/Article/details/gkfjkuxec.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/gvfabmhku.sHtML

[U48] PHP：纯枚举
来源：http://baike.vehdjk.com/Article/details/gngoaweik.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fktsv.cn/Article/details/gwbppxylx.sHtML

[U49] PHP：只读属性
来源：http://www.share.yfazqb.com/Article/details/gygrczjgr.sHtML

public readonly string $name
来源：http://3g.tarul.cn/Article/details/gdttsetcx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/ghnbhtjsk.sHtML

public function __construct(private int $id) {}
来源：http://mobile.sjlbkw.cn/Article/details/gfqhqjvgz.sHtML

[U51] PHP：数组解构
来源：http://www.share.yfazqb.com/Article/details/gbsserfov.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gwvbzgghr.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/ghnupxtla.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.yfazqb.com/Article/details/gbjvlyghu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.epnwcf.com/Article/details/ggiztuftk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gbafqxewl.sHtML

[U54] PHP：空安全调用
来源：http://baike.fktsv.cn/Article/details/gjvcuiihn.sHtML

$obj?->method()
来源：http://blog.vehdjk.com/Article/details/gewbulqbk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.vehdjk.com/Article/details/ghqfmspps.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/grycigxwd.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/grbcffzrg.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/grrrlepwj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gfmhxbqrg.sHtML

"值: {$a}"
来源：http://read.share.bbcook.cn/Article/details/gmsyuzusn.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fktsv.cn/Article/details/gbituesbi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/godzgrxdr.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/ghrgztdaf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gaeivprei.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/gwdrgbzeu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gozigreqo.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/gyglwapxx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/gnpmqsmtk.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gruwyevxn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.bbcook.cn/Article/details/gdvomxkjw.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gjpiovfyg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gwiwfuhod.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/griermbmt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/gvokavoyi.sHtML

[U65] PHP：会话
来源：http://blog.epnwcf.com/Article/details/gtwrknesn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/grzqhoyom.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.yfazqb.com/Article/details/gbeouootd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.tarul.cn/Article/details/gisptwato.sHtML

[U67] PHP：处理文件上传
来源：http://baike.bbcook.cn/Article/details/gzimksukg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gtukzuucc.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/ghmgngerk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/gezktwhew.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.bbcook.cn/Article/details/gcokywuze.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/gvycjjnhm.sHtML

[U70] PHP：PDO 事务
来源：http://wap.bbcook.cn/Article/details/gqtfkpgts.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gqwgcgmjo.sHtML

[U71] PHP：抛出异常
来源：http://read.share.bbcook.cn/Article/details/gubqttwwg.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.bbcook.cn/Article/details/gorvwtuxw.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gyeawdwbs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.tarul.cn/Article/details/glsvcwaoz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.epnwcf.com/Article/details/gkxvvezpr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/gcmxuasyf.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gdmpqvzib.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.sjlbkw.cn/Article/details/gsftldiqw.sHtML

[U75] PHP：依赖注入
来源：http://blog.epnwcf.com/Article/details/gpfaofbdk.sHtML

composer require psr/container
来源：http://www.share.yfazqb.com/Article/details/glotubfob.sHtML

[U76] PHP：简单路由
来源：http://m.share.sjlbkw.cn/Article/details/grcacxqqh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.vehdjk.com/Article/details/gawifvqez.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gnesizcuw.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/gxxbvyjdh.sHtML

[U78] PHP：单元测试
来源：http://www.share.fktsv.cn/Article/details/givxcczbx.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.sjlbkw.cn/Article/details/ggjmxkcoj.sHtML

[U79] PHP：静态分析
来源：http://wap.yfazqb.com/Article/details/gjvlevxzf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.yfazqb.com/Article/details/gikizajjs.sHtML

[U80] PHP：代码规范修复
来源：http://baike.epnwcf.com/Article/details/geixrknmb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.yfazqb.com/Article/details/ggjshahkj.sHtML

[U81] JS：初始化项目
来源：http://3g.fktsv.cn/Article/details/gdlsrjmig.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gmnkhyzlw.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/giarupgcl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.yfazqb.com/Article/details/gbxisyosr.sHtML


<!-- 参考信息 -->