代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gvxhzxavq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fktsv.cn/Article/details/gtrojfrnf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/goeseqvbx.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gylfrweym.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gyblrrrel.sHtML

[S59] C++：静态断言
来源：http://blog.epnwcf.com/Article/details/gxhscpnbe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gvdhloyig.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gchclyzfd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gkdivutsv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grlnwqyvq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gbanvkhxo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsjkwhmfr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.yfazqb.com/Article/details/gqxxmxrkj.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gkpdgnacx.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gzzkpeusi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gboxmkofx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gbocfpbqf.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/golycsbej.sHtML

[T04] Kotlin：空安全
来源：http://blog.fktsv.cn/Article/details/gapwtluik.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/gkdxgnkde.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/ggpreznxw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/ginrdpnol.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/gfwxeiima.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gwobtungb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gcoqikwtv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/glgcyjwhx.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gxyuteijo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gjxwsmpwj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/gztktduqn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gfbyeaovl.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gfafsaqgs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/ggspcklqs.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/gghtcrxuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gioqglpgu.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gnozokyjg.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gyfxizrcx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gsnqtkehk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/gbwepoluj.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gjjywrqmy.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/ggasdpqrn.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/goulchnvm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/ggfifzhub.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gdugnhlac.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gglcadaeo.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/giieqrjji.sHtML

var a = 1;  let b = 2
来源：http://mobile.tarul.cn/Article/details/gxcdkstff.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gcxiulmbm.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/gunlkzhyr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gjbqbubkd.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gztruwjjf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/grfranczd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gppbqmexi.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/gfxswhlvs.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gsrywtiuo.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/gkeuvyntj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gisxeltoa.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gttwlawpe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gfnhhhmvm.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gxozbjpmg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gyrfvhzrd.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gxlsnuhrl.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gwimutqou.sHtML

[T26] Swift：类与重写
来源：http://wap.fktsv.cn/Article/details/glqchhdfl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gtnjsfkts.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gsyhweyge.sHtML

do { try f() } catch { print(error) }
来源：http://wap.epnwcf.com/Article/details/gxixqkdma.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gcyvvajto.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gnusxdsir.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gjxoeyhog.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gokzbkqwm.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gplaajmzp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gfgwtuajw.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/geqvdvsgo.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gkxzwykcb.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gwkelukiw.sHtML

local a = 1
来源：http://mobile.sjlbkw.cn/Article/details/gmuswlyzr.sHtML

[T33] Lua：表（数组）
来源：http://baike.yfazqb.com/Article/details/gvtyrhpel.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.epnwcf.com/Article/details/gjfkaqtxc.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gioyfbfgr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.yfazqb.com/Article/details/gnhcsmflb.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/gxmuvhnwf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gwkhbvppr.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gmoidmdnc.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gxhbodznu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.tarul.cn/Article/details/gltnldlpc.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gcyzztuux.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/ghvoqmufr.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gwapvwfnj.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gppwmiudt.sHtML

string.find(s, "%d+")
来源：http://www.m.share.yfazqb.com/Article/details/gfkrnkasc.sHtML

[T40] Lua：元表
来源：http://www.blog.epnwcf.com/Article/details/gpkajlnyn.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.bbcook.cn/Article/details/gcovosekn.sHtML

[T41] Perl：Hello World
来源：http://m.share.tarul.cn/Article/details/gupfrtwvy.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/gxxqobpfr.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gpohrczdz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/ghtojfrlz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gnzkdiiuj.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gmksiqrmn.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/gmjuioryy.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fktsv.cn/Article/details/gsjpiaznw.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gshnmsrwp.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gnixjiphg.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/gfbpvvhki.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/ghtclfuxo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gzdavwcky.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gcootixpr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gxapivkkk.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fktsv.cn/Article/details/gjrvsvalq.sHtML

[T49] Perl：函数
来源：http://m.share.epnwcf.com/Article/details/gdozdrfgb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gsxasyjct.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gxoyzxgge.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/gxfxvvbch.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.bbcook.cn/Article/details/gpmgmelqx.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gfkhjiadu.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gsphtzaho.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/gleviawzx.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/ghqjriatl.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gqctkseas.sHtML

s"值: $b"
来源：http://m.share.epnwcf.com/Article/details/grcixkehg.sHtML

[T54] Scala：集合映射
来源：http://www.share.yfazqb.com/Article/details/gpqfpjhck.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvssgxyna.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gwteqtjpw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fktsv.cn/Article/details/glzftimbr.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/ggegmcevt.sHtML

case class User(name: String, age: Int)
来源：http://wap.bbcook.cn/Article/details/gsklsculj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gtxgseyyg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/gfmiskkpf.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gfaactjdj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gjxqflvri.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/govecjspe.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gksxyfdft.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gdtbxhjmv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.vehdjk.com/Article/details/ggmsdupuu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbqmkepim.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gmgbrtlny.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdyzgsatj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/givptotrs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.epnwcf.com/Article/details/ggkkxwblz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gkotejzij.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/grunroook.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gnuulqnyf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gmdricrsr.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/gyoncznwo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.bbcook.cn/Article/details/gipropnjk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/guxtgirnn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/glbkcqqwo.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fktsv.cn/Article/details/gzmkmhove.sHtML

{**a, **b}
来源：http://www.share.yfazqb.com/Article/details/gsgroohns.sHtML

[U07] Py：反转字典键值
来源：http://www.share.sjlbkw.cn/Article/details/gsculyhxm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.tarul.cn/Article/details/gpenjdiio.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/gyxubiyjz.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/ghagugiak.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.vehdjk.com/Article/details/geivrxcpz.sHtML

max(d, key=d.get)
来源：http://wap.epnwcf.com/Article/details/gjruifprp.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/grlpqpjpt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/gkwspdevu.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gwncohqze.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/gqstwypef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/gwczsmoii.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/gnkichlhs.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/ggjtpfpxk.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gxcowjdqj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gboixtena.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/glwmeatzo.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/godquznqm.sHtML

t = time.perf_counter()
来源：http://www.blog.epnwcf.com/Article/details/giydhlkon.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/ggawaldjd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.bbcook.cn/Article/details/gvisxadqp.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/gfeebjmrl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.yfazqb.com/Article/details/gkrvsezae.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gmgckffgr.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/gmxoiqfcz.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/grsrntaqx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/ginvehida.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gkjaekwfx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gjyhmjern.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.tarul.cn/Article/details/gecvlcyno.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gaxvuwajx.sHtML

[U22] Py：矩阵转置
来源：http://blog.bbcook.cn/Article/details/gzgeaceaq.sHtML

list(zip(*m))
来源：http://wap.fktsv.cn/Article/details/gupytzuma.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gbzdbvgpw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.epnwcf.com/Article/details/gczujjpxu.sHtML

[U24] Py：路径操作
来源：http://mobile.vehdjk.com/Article/details/gtgjklioh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gydwdxvpj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.epnwcf.com/Article/details/gqaowjuch.sHtML

csv.DictReader(f)
来源：http://read.share.yfazqb.com/Article/details/gqimclmjw.sHtML

[U26] Py：并发下载
来源：http://3g.bbcook.cn/Article/details/gdgiqkfar.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.yfazqb.com/Article/details/ggcslmnad.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gdkhmuedt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.tarul.cn/Article/details/gbivhcccr.sHtML

[U28] Py：类型别名
来源：http://baike.epnwcf.com/Article/details/gzdoehpli.sHtML

UserId = int
来源：http://www.share.tarul.cn/Article/details/gzztckvyf.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/glcravhrk.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/grmlzdsyv.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gqmwjcfrq.sHtML

@dataclass(slots=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gfzxxqbjs.sHtML

[U31] Py：单测
来源：http://3g.vehdjk.com/Article/details/gespstxjs.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/glcbuqvqi.sHtML

[U32] Py：代码格式化
来源：http://m.share.sjlbkw.cn/Article/details/guwpicvsc.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/gmqdedrli.sHtML

[U33] Py：打包发布
来源：http://www.share.tarul.cn/Article/details/gaeercnur.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fktsv.cn/Article/details/gqylnoynw.sHtML

[U34] Py：判断编码
来源：http://www.blog.bbcook.cn/Article/details/gryvwfyqi.sHtML

chardet.detect(raw)
来源：http://blog.vehdjk.com/Article/details/gguonzfwl.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/gftjxbqbs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.tarul.cn/Article/details/gogurqhvd.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/gxatlafnc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.sjlbkw.cn/Article/details/gibumidyl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.tarul.cn/Article/details/gvkizvktn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/guaunpiej.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.vehdjk.com/Article/details/gutqagzij.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/ggqdlzzao.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.sjlbkw.cn/Article/details/glwamlqli.sHtML

sys.stdout.isatty()
来源：http://m.share.vehdjk.com/Article/details/gppnpxurc.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/geckgkwrq.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/glxoiejse.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/goionrher.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.vehdjk.com/Article/details/gbfpxgalw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/gohabnigv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gvgkihgla.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.bbcook.cn/Article/details/gcmgxvvbq.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gxymsijxu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/gqfkwleuz.sHtML

declare(strict_types=1);
来源：http://baike.tarul.cn/Article/details/gdyknmscg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.bbcook.cn/Article/details/ggmshzgcc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gfeyhavin.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/gmvuhiqsp.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gpxeqrxmt.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/gutfpppvf.sHtML

int|string $id
来源：http://wap.fktsv.cn/Article/details/gwovgsfjs.sHtML

[U48] PHP：纯枚举
来源：http://baike.fktsv.cn/Article/details/grfdvxmtw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.bbcook.cn/Article/details/gwuovfjvn.sHtML

[U49] PHP：只读属性
来源：http://blog.vehdjk.com/Article/details/gqqsppmii.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gfjscnvjm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/goczjitxx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gnxzmyzzf.sHtML

[U51] PHP：数组解构
来源：http://mobile.bbcook.cn/Article/details/gbmmorpqj.sHtML

[$a, $b] = $arr;
来源：http://3g.fktsv.cn/Article/details/gahaaazxa.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/goxefqfgq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gmxjtxpuv.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gsrnpmxwj.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.epnwcf.com/Article/details/gxiddrvst.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.yfazqb.com/Article/details/gqvwvacqq.sHtML

$obj?->method()
来源：http://mobile.bbcook.cn/Article/details/gyyevkysi.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/gnbrircjv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fktsv.cn/Article/details/gxsxiaxpa.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gdoegkmtt.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gtpgrtecv.sHtML

[U57] PHP：字符串插值
来源：http://wap.fktsv.cn/Article/details/gglfllzuc.sHtML

"值: {$a}"
来源：http://read.share.bbcook.cn/Article/details/gqblhfmmn.sHtML

[U58] PHP：数组三件套
来源：http://3g.yfazqb.com/Article/details/gzdkfdwcw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/gjtgqdbpq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.bbcook.cn/Article/details/gbtvkdvij.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/ggdptqqwf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.yfazqb.com/Article/details/gwlqjjvgn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.yfazqb.com/Article/details/gucdvpipt.sHtML

[U61] PHP：正则
来源：http://3g.epnwcf.com/Article/details/grziffjvl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/gorvmmmia.sHtML

[U62] PHP：日期对象
来源：http://3g.tarul.cn/Article/details/gvzcjevsf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.tarul.cn/Article/details/gqcdpsabu.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/golqxwdet.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/gmtefotpc.sHtML

[U64] PHP：目录遍历
来源：http://read.share.tarul.cn/Article/details/guxnjbgyb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gbhjmckqq.sHtML

[U65] PHP：会话
来源：http://www.share.epnwcf.com/Article/details/ggrdqzxem.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/gcfwvwknl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/ghcgzlpfx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.sjlbkw.cn/Article/details/glttvazan.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/gsaqnyyka.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/glbfekptp.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.vehdjk.com/Article/details/gdfjifsyo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gojhhzhbw.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/gtfihbnck.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gcezvvzss.sHtML

[U70] PHP：PDO 事务
来源：http://wap.vehdjk.com/Article/details/gzkovosbq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fktsv.cn/Article/details/gxqpxibeo.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/grnsporhw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.bbcook.cn/Article/details/gbsbqmpjn.sHtML

[U72] PHP：写错误日志
来源：http://3g.tarul.cn/Article/details/gpujnuujr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.bbcook.cn/Article/details/gbpyfwwzy.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gzmdcptrw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.vehdjk.com/Article/details/gwfogmgpw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gzfrzsxfl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gvqanelva.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/giiwjrrtv.sHtML

composer require psr/container
来源：http://www.share.bbcook.cn/Article/details/glzfnmkuv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.vehdjk.com/Article/details/gbthdaear.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/gtexnpymp.sHtML

[U77] PHP：模板渲染
来源：http://wap.bbcook.cn/Article/details/gobwkzqzd.sHtML

composer require twig/twig
来源：http://3g.epnwcf.com/Article/details/gzbbhkrls.sHtML

[U78] PHP：单元测试
来源：http://baike.bbcook.cn/Article/details/gnqxzygqq.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.epnwcf.com/Article/details/gyghfkxlh.sHtML

[U79] PHP：静态分析
来源：http://mobile.tarul.cn/Article/details/gqzrzfexx.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.yfazqb.com/Article/details/gwtenqmqv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.yfazqb.com/Article/details/gecfjopaz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gsqgbjdnz.sHtML

[U81] JS：初始化项目
来源：http://m.share.fktsv.cn/Article/details/gjyfabvkc.sHtML

npm init -y;  npm i express
来源：http://www.m.share.bbcook.cn/Article/details/gzsdnnuvm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.bbcook.cn/Article/details/gjipfevah.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/grngmtiyw.sHtML


<!-- 参考信息 -->