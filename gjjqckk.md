代发 wailian999

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/golazhoho.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gdgsnfrzm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/grqasgwif.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gzspbwphn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gfuebmqih.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/gnutrfrzl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/guzrczlna.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/gydeatnkf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gseisjsys.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/guvwnjqko.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/glnbiiknm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gxqvqvvco.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gbrvwjjal.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/geozcrimi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gpefbziwv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/giyzrhgfn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gftvnrgum.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gfredextu.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gftlfjmyn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gmnuopmiq.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gpslxzjnh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gyozoujla.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/ggmjnhtqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gdnlksabl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gsrzxmznp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjwjzjsgr.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/gavkorres.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gxjjzkyho.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gyezuqvml.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/gvincrmpq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gfoaponvq.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gyvupnetk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gcalzpriu.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gyeedfsfs.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gxidsjpjt.sHtML

"值: \(b)"
来源：http://baike.sjlbkw.cn/Article/details/gqmuqjnvr.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/graslaown.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gujajowks.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/govsfxxmt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gdvrlttkx.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gbhyajakd.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gvbdvttzh.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/ghevhlwvk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/gfmavtxxh.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/glqvyanhk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/guujdkqpy.sHtML

[T24] Swift：闭包
来源：http://m.share.bbcook.cn/Article/details/gmtlxodfi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gdghmixhj.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gnrcvhsnq.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gplnombiz.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gtbieceqx.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gclmhgipk.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/gdufrpkgc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gfjrmhgpu.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gmaeytwkq.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gkibleupb.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gprquiknx.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/gvgauxjgv.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gvmxyylxs.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.bbcook.cn/Article/details/gohvhwouc.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/giyunqapm.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/galcameds.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/gcrzfflhm.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gsuworjxv.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gmwmfhgon.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/gdqkwzusj.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/glpifrshd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gdeqrvfpg.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gbselomig.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gihdrbyxe.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/grkdgkolv.sHtML

function add(a, b) return a + b end
来源：http://m.share.sjlbkw.cn/Article/details/gezlcjaem.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gtzvgkgkk.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gqnuivoau.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gfaaabtvt.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/giapzbgfr.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/glfdgefmf.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/gnccdipks.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gmyikimjk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.epnwcf.com/Article/details/gtmynpyvx.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/grqqxszlr.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gsssfsflq.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gprpdfewz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/gxkhhorcq.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/ghpmecsjk.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/grarqcpmi.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/gixhsewrd.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.tarul.cn/Article/details/geemmhpcn.sHtML

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gwefgzyep.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.tarul.cn/Article/details/gmlkbiwmc.sHtML

[T46] Perl：哈希操作
来源：http://blog.tarul.cn/Article/details/gavrscejc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.bbcook.cn/Article/details/gnmazwkeq.sHtML

[T47] Perl：正则捕获
来源：http://wap.bbcook.cn/Article/details/guytmboqq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.tarul.cn/Article/details/govoztxgv.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/gpaonzaix.sHtML

$s =~ s/old/new/g;
来源：http://wap.bbcook.cn/Article/details/gnizfyjqy.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gersrrfkl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/guqvbuanl.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gpxslmvro.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.vehdjk.com/Article/details/gemoahfxg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/gaaunsalr.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gfvnmssby.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gdjctsfbb.sHtML

[T52] Scala：变量
来源：http://3g.tarul.cn/Article/details/gmvezaylx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/glydqmygz.sHtML

[T53] Scala：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gamreoect.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/guezsluxr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gojzmypmt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.yfazqb.com/Article/details/gmzcqaksw.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.tarul.cn/Article/details/geiuerfwb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gevlmwwvf.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/gpnygusfk.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/glpfwicmz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gengrplug.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/glvnvgnys.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/ggzwmagfp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gfnazwiyi.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/gnelqiazo.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gctmhkzkn.sHtML

[T60] Scala：折叠
来源：http://blog.bbcook.cn/Article/details/grsdepfxm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gisjzkxte.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grzhbfcjp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/grjygupia.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxzotizrd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/gfxowyybo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/ggdtqgamq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.sjlbkw.cn/Article/details/gckwdioiz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gjwxfvxiq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.tarul.cn/Article/details/ggokclnaw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.yfazqb.com/Article/details/gxgayyqlu.sHtML

[U04] Py：变量调试打印
来源：http://3g.tarul.cn/Article/details/gzhrvbhbb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gpmyuoryr.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fktsv.cn/Article/details/gvbkkiuaj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/glkamwhdl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/glpqtplzw.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gtcbrioqu.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gkidzpjnt.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.bbcook.cn/Article/details/gsbihkisg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gjjovqyeo.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gnfzrlaba.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/gtnwttbbd.sHtML

max(d, key=d.get)
来源：http://wap.tarul.cn/Article/details/gyteatuvh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/ggtyqdktq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gfdienewr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gosdqnjpj.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/grinliqgo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/germjwqed.sHtML

Counter(arr).most_common(3)
来源：http://blog.sjlbkw.cn/Article/details/giwrjcfjb.sHtML

[U13] Py：固定长度队列
来源：http://wap.sjlbkw.cn/Article/details/gkuxmxsib.sHtML

deque(maxlen=10)
来源：http://blog.vehdjk.com/Article/details/gpirlwsgm.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/glxmqjyxq.sHtML

defaultdict(list)
来源：http://wap.yfazqb.com/Article/details/gabbbywfo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gtsmfhped.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/gminnmnfv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gilmggpen.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.vehdjk.com/Article/details/gjqynyrpv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.bbcook.cn/Article/details/goysisoet.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/giblzclln.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/glfkhtlco.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/gnxwvwues.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gqafnhftc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/gbrcbrcdu.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fktsv.cn/Article/details/giodybang.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.yfazqb.com/Article/details/givpbgjqr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gebguujvf.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gpvmufqkk.sHtML

[U22] Py：矩阵转置
来源：http://m.share.vehdjk.com/Article/details/gngymjprm.sHtML

list(zip(*m))
来源：http://wap.epnwcf.com/Article/details/ghutbcdou.sHtML

[U23] Py：分块读取大文件
来源：http://3g.epnwcf.com/Article/details/gnbvcalmk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gixxfpejg.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gljpctbzt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/givbuoyxe.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/ggtftxxci.sHtML

csv.DictReader(f)
来源：http://baike.fktsv.cn/Article/details/gblyjeojk.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gpxxwyiqu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.vehdjk.com/Article/details/gonqmkptk.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/givfcfspl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fktsv.cn/Article/details/ggkhusfxp.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/gdriyyuty.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/gmaslcnmz.sHtML

[U29] Py：属性校验
来源：http://wap.bbcook.cn/Article/details/gxaxqrbla.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/gbyjcnptd.sHtML

[U30] Py：数据类
来源：http://www.blog.yfazqb.com/Article/details/grhrimfop.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gqbqyntsm.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gvkfwwjma.sHtML

python -m pytest -q
来源：http://blog.yfazqb.com/Article/details/gvxrxswbc.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/gqrzmefra.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gdwvqtovv.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/ghhbiocmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gzccuaepz.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gkgwtkbdu.sHtML

chardet.detect(raw)
来源：http://baike.sjlbkw.cn/Article/details/gwjitauuy.sHtML

[U35] Py：发送邮件
来源：http://www.share.sjlbkw.cn/Article/details/gigeaenhl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/gzygccoje.sHtML

[U36] Py：定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gbmwpushn.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/gokbqstcq.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/grqajgtsg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/ggfonaeng.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/gafgrrrff.sHtML

Path(__file__).resolve().parent
来源：http://www.share.bbcook.cn/Article/details/gfbfytnqh.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/gvkxgvopk.sHtML

sys.stdout.isatty()
来源：http://3g.yfazqb.com/Article/details/guuxunwvt.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.sjlbkw.cn/Article/details/gthdlqqqq.sHtML

print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/glbenojkr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.sjlbkw.cn/Article/details/guiqsrslp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gdalhnqgo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/gsdqwitcs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.sjlbkw.cn/Article/details/gxvwmtyln.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gomjjmieh.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/gjmpperol.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.tarul.cn/Article/details/gobfmkaxu.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/ghutwpkbx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gkxyvpqon.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gynwooblf.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gtfljzqya.sHtML

?string $name = null
来源：http://www.blog.vehdjk.com/Article/details/gfecvhmhn.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/gydgoocbj.sHtML

int|string $id
来源：http://www.m.share.bbcook.cn/Article/details/gxrhlnutq.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/gqwekwula.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/gmeskxuwa.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/gripatngw.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/gseledxgj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gflfnabnb.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvzwygkkz.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.vehdjk.com/Article/details/gpakhdldh.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gbnruitvm.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gncrutzad.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.yfazqb.com/Article/details/gzuragqfq.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fktsv.cn/Article/details/gsbueovlp.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fktsv.cn/Article/details/gfnkuosfc.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fktsv.cn/Article/details/gblllmecl.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gfzwflxdh.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/gdimayoba.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gqhuemobk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gfokxdynx.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gawddiiqm.sHtML

[U57] PHP：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gbbdhqupx.sHtML

"值: {$a}"
来源：http://www.blog.yfazqb.com/Article/details/grulyvbpu.sHtML

[U58] PHP：数组三件套
来源：http://wap.yfazqb.com/Article/details/gnaqwlswy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gvyketcmd.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gllkiwssp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gkrzynlbe.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/gwxgurdix.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/gcpcbrncg.sHtML

[U61] PHP：正则
来源：http://mobile.epnwcf.com/Article/details/gmmzqlkcj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gibbsxsey.sHtML

[U62] PHP：日期对象
来源：http://www.blog.sjlbkw.cn/Article/details/gnyjfklzw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fktsv.cn/Article/details/gdjiyzfxa.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/gilgjnsyc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.sjlbkw.cn/Article/details/gcnipyfiu.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.vehdjk.com/Article/details/guqszqbkv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.sjlbkw.cn/Article/details/ggvikkegx.sHtML

[U65] PHP：会话
来源：http://wap.epnwcf.com/Article/details/gwopycxpu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.epnwcf.com/Article/details/goflifgsc.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.tarul.cn/Article/details/gipyxgopp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fktsv.cn/Article/details/gdnwnztka.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/grkmsyudz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.vehdjk.com/Article/details/gvyydkxqo.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gpnimpcxq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.sjlbkw.cn/Article/details/gyeerfpgc.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/gtannsuus.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.yfazqb.com/Article/details/gqdggqtyr.sHtML

[U70] PHP：PDO 事务
来源：http://3g.tarul.cn/Article/details/gdltprhko.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/giclhtvdx.sHtML

[U71] PHP：抛出异常
来源：http://m.share.tarul.cn/Article/details/gayzzsets.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.vehdjk.com/Article/details/goalyjigy.sHtML

[U72] PHP：写错误日志
来源：http://blog.sjlbkw.cn/Article/details/gbpgrrlkb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.vehdjk.com/Article/details/gdbixwwze.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gvkkkmfri.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gttgxlpkh.sHtML

[U74] PHP：读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/ghufdobbq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.vehdjk.com/Article/details/gunruulxr.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gkldzrlpt.sHtML

composer require psr/container
来源：http://read.share.bbcook.cn/Article/details/gjzdfccqb.sHtML

[U76] PHP：简单路由
来源：http://read.share.yfazqb.com/Article/details/gesniqydj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.yfazqb.com/Article/details/gankbnpwv.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gwrghqssn.sHtML

composer require twig/twig
来源：http://wap.vehdjk.com/Article/details/gprxffbcy.sHtML

[U78] PHP：单元测试
来源：http://wap.fktsv.cn/Article/details/gbzqarbob.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gbjelkrlg.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/gzutnlxpr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/gvukkgjic.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/gckmvmqaa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.yfazqb.com/Article/details/geiefhxfi.sHtML

[U81] JS：初始化项目
来源：http://baike.vehdjk.com/Article/details/gonvxwfci.sHtML

npm init -y;  npm i express
来源：http://3g.bbcook.cn/Article/details/gfujsqvnp.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/giryulnaf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.epnwcf.com/Article/details/gamoirtrm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.epnwcf.com/Article/details/gaysmjkfs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gwxyxhpaw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/gzwpwagnp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gptmqoqrt.sHtML

[U85] JS：可选链
来源：http://3g.tarul.cn/Article/details/gquczghwu.sHtML

a?.b?.c
来源：http://m.share.fktsv.cn/Article/details/gugwpzoxs.sHtML

[U86] JS：空值合并
来源：http://wap.yfazqb.com/Article/details/gfhjiajmb.sHtML

a ?? b
来源：http://m.share.bbcook.cn/Article/details/gsvpcfyma.sHtML

[U87] JS：解构默认值
来源：http://www.blog.vehdjk.com/Article/details/gunchopjh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.bbcook.cn/Article/details/gephybhrx.sHtML

[U88] JS：对象展开合并
来源：http://baike.epnwcf.com/Article/details/gekxqlufa.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/grqgfwlis.sHtML


<!-- 参考信息 -->