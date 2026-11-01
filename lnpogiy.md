代发 wailian999

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/guekgyfcl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gymidkqwn.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gpfmrwexx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/gkgaiknqb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.yfazqb.com/Article/details/gsfzzquiu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gigdsqiqs.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gpwekwyrc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/ghfhnviqy.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gwaltfswj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsczyovnt.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gbocxtkgx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fktsv.cn/Article/details/gdncyczok.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/gqzofjnvg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gyuyvuhnj.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.tarul.cn/Article/details/goaplrkbq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gobdspwfq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gvwbdakff.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/giqrpcukk.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gktadfkfn.sHtML

for (i in 1..10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gagqqyvyx.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gylbezwfw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gdqolimut.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glqupioay.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gqdfibniq.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gybbiopzc.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gevpxsmkf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gjzrrnrgf.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gfwpbuczr.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gbktadcfh.sHtML

if let n = opt { print(n) }
来源：http://baike.yfazqb.com/Article/details/gtdolnbut.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gndramneo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.yfazqb.com/Article/details/gqslahlpp.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/ggezujpjg.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gxvgfslpi.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gxdrmsrew.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gwpgdauvp.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gnfaaegfq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.tarul.cn/Article/details/glwopkjlo.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gjyaduebh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gtzodzjrl.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/gnmxmbspg.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gwqtfucly.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gntigyjja.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gwicmmaee.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/gqxhsdevt.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/gdzspgutb.sHtML

[T28] Swift：枚举
来源：http://blog.epnwcf.com/Article/details/gsfiowosc.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/gmrdqkpwn.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.epnwcf.com/Article/details/gxlqpuswr.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/gsnuphpeg.sHtML

[T30] Swift：协议
来源：http://3g.yfazqb.com/Article/details/gvaoxpndi.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gvdrmhozn.sHtML

[T31] Lua：Hello World
来源：http://read.share.vehdjk.com/Article/details/gqkleiifp.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gezyzskjk.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gwpvbeoyt.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gwjowulhl.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/gkjcxxxor.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.tarul.cn/Article/details/gdnnymgbe.sHtML

[T34] Lua：遍历表
来源：http://read.share.fktsv.cn/Article/details/graxfnvrm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/gonqmzmsr.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gnteruona.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gnmstgqit.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/gfxqzejyl.sHtML

function add(a, b) return a + b end
来源：http://www.share.tarul.cn/Article/details/gkooztbbv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gfakykhfo.sHtML

"a" .. "b"
来源：http://blog.tarul.cn/Article/details/grdxhenac.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gzlubtqah.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/ghdgmtcxz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gbmkowpwp.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gvkgshcic.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gkogumnbm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.tarul.cn/Article/details/geifdbbrx.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gndorxntz.sHtML

print "Hello\n";
来源：http://baike.sjlbkw.cn/Article/details/ghhidyljw.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gzupjpxgy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/ghlinzete.sHtML

[T43] Perl：字符串插值
来源：http://3g.tarul.cn/Article/details/gomxzytpa.sHtML

"值: $a"
来源：http://blog.epnwcf.com/Article/details/gvuxyqotn.sHtML

[T44] Perl：条件
来源：http://read.share.sjlbkw.cn/Article/details/gabjnzzzs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gclfssbqx.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fktsv.cn/Article/details/gtykbxsub.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/govvfscfc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gmodnabwz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gpzqestfn.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/ghaxgsqae.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gvqhjjklx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.bbcook.cn/Article/details/gsgvnqwvc.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gjgnozxqq.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gedsjixks.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gimdicrqg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gukkpovox.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gontwajbf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.bbcook.cn/Article/details/geenkrabp.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gncpismcl.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gscnumxgt.sHtML

[T52] Scala：变量
来源：http://m.share.yfazqb.com/Article/details/gyqrlrruz.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gmwcjjbwg.sHtML

[T53] Scala：字符串插值
来源：http://3g.tarul.cn/Article/details/gzfevgtxj.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/glzcsalxp.sHtML

[T54] Scala：集合映射
来源：http://mobile.fktsv.cn/Article/details/gohfzwnom.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.bbcook.cn/Article/details/geqidkrje.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/glundhnrf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/gfaijmaje.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gnvfsjzzw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gxprrzwyq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gexrrbxfv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/grzpgslbv.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/gnyfmdzdq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gfvnpeftq.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gswxuyzsk.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gniscokci.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/galkywqze.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gapytonxb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grbjkflom.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gmxcduvlu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpdifloiu.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.bbcook.cn/Article/details/gmnyhvnqw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gknlwfrqa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.bbcook.cn/Article/details/gsqjpwwmr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gtwkandqe.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gcurwmuje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gkruxogkm.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gefzrszvl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gzcfzthux.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.epnwcf.com/Article/details/gdhmxbcoh.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/ghsdhhkti.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/gydizvvwx.sHtML

{**a, **b}
来源：http://3g.bbcook.cn/Article/details/gecirkbpp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.vehdjk.com/Article/details/gkxqtvzfo.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/gptovhrmy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/gumlaneoe.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gfpvxbovb.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/ggnsaweyc.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gnqofdqwf.sHtML

[U10] Py：按值排序字典
来源：http://read.share.sjlbkw.cn/Article/details/ghrbepruf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gmjmpukyr.sHtML

[U11] Py：生成器表达式
来源：http://wap.vehdjk.com/Article/details/grggxyyke.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gfyoflpiy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.sjlbkw.cn/Article/details/glywmvqaw.sHtML

Counter(arr).most_common(3)
来源：http://blog.fktsv.cn/Article/details/gdiecvdtd.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/getyltfhg.sHtML

deque(maxlen=10)
来源：http://mobile.fktsv.cn/Article/details/gocewbscu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/gylfyfjfl.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gdbvzbnjv.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/goyxtvevr.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gqletclma.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/gphvmrzub.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gkwlqmhcu.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gjtixcstt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.sjlbkw.cn/Article/details/gcahwvqnu.sHtML

[U18] Py：预编译正则
来源：http://baike.epnwcf.com/Article/details/gmdzbwbwi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gxtjrqfnz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gjuobzpwb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/gtixtkwaj.sHtML

[U20] Py：缓存函数结果
来源：http://3g.bbcook.cn/Article/details/geashtgqj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/gnfpzfzxc.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.vehdjk.com/Article/details/gfegwwiir.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fktsv.cn/Article/details/gskddlnto.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gijatvhcj.sHtML

list(zip(*m))
来源：http://m.share.fktsv.cn/Article/details/gytcqfqcg.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/ggekoxqay.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gmegcgfjv.sHtML

[U24] Py：路径操作
来源：http://m.share.epnwcf.com/Article/details/gkjttqcix.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gdpxmztug.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/gfsmfxomo.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/grvntqece.sHtML

[U26] Py：并发下载
来源：http://read.share.yfazqb.com/Article/details/gkxipefpu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/gfrjlsvjb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.yfazqb.com/Article/details/gutofmhbd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.vehdjk.com/Article/details/gctdbbzml.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/gxnlrqmpa.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/grjyjefzc.sHtML

[U29] Py：属性校验
来源：http://read.share.bbcook.cn/Article/details/gixeiqiol.sHtML

@property 与 @x.setter 配合
来源：http://wap.tarul.cn/Article/details/gpwhzytak.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/golbmtbvz.sHtML

@dataclass(slots=True)
来源：http://mobile.bbcook.cn/Article/details/gcufanfuf.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/glvlkuorw.sHtML

python -m pytest -q
来源：http://m.share.tarul.cn/Article/details/gnlrwlert.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gfetqgxxz.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gwmopmaka.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/gjmbqxotn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.epnwcf.com/Article/details/gbaclvtfk.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/ghrvqxurh.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/gqymvvwtz.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/ggunrhsub.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.epnwcf.com/Article/details/ginfmoena.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gxviqetho.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.yfazqb.com/Article/details/gnedardwu.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gnzgtqbio.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/gpyltoxmm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.vehdjk.com/Article/details/ggumbigzt.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gowiqeqee.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/groipvncr.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/ghhbumgga.sHtML

[U40] Py：打印到标准错误
来源：http://baike.tarul.cn/Article/details/gmarjdqcr.sHtML

print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gbiqoixaw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gcgnkkxmj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/gbnyntrwc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.epnwcf.com/Article/details/gcndhymme.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.tarul.cn/Article/details/gwlcsgbqs.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fktsv.cn/Article/details/gkrvosusf.sHtML

namespace App\Http;
来源：http://www.blog.bbcook.cn/Article/details/gdaaalmxc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gipdyvlhh.sHtML

declare(strict_types=1);
来源：http://3g.tarul.cn/Article/details/gegkuwqfq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gyewilsyi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gwtfkhjnv.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/ghiczqhgi.sHtML

?string $name = null
来源：http://mobile.fktsv.cn/Article/details/gsiecouur.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/grojsbyhm.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/guspvqfgx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/gggxdcbvg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.sjlbkw.cn/Article/details/gtzkojdtq.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/guunhjlqg.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/gsckqbbkl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.yfazqb.com/Article/details/giopuqkrt.sHtML

public function __construct(private int $id) {}
来源：http://wap.yfazqb.com/Article/details/ghbjbsikm.sHtML

[U51] PHP：数组解构
来源：http://wap.bbcook.cn/Article/details/ggqochyde.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/galsvvoqm.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gqajenywq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gntpsqvzu.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fktsv.cn/Article/details/gkcrtbkew.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.epnwcf.com/Article/details/gilatnjdl.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/gqbppolue.sHtML

$obj?->method()
来源：http://www.m.share.tarul.cn/Article/details/gxnmlnonx.sHtML

[U55] PHP：match 表达式
来源：http://blog.fktsv.cn/Article/details/gdtnfrtey.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gnfvumxbx.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gznigewtq.sHtML

f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gpmcykbkf.sHtML

[U57] PHP：字符串插值
来源：http://3g.fktsv.cn/Article/details/gvezwrhal.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gixrxhtcb.sHtML

[U58] PHP：数组三件套
来源：http://3g.sjlbkw.cn/Article/details/gddvmujbe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gyusqdfxu.sHtML

[U59] PHP：自定义排序
来源：http://3g.vehdjk.com/Article/details/gcxpopbda.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gevlnzweq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.tarul.cn/Article/details/getixsgrr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gznqnprdo.sHtML

[U61] PHP：正则
来源：http://m.share.yfazqb.com/Article/details/gmqaegmuy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gqqaoqjwl.sHtML

[U62] PHP：日期对象
来源：http://read.share.epnwcf.com/Article/details/gadapbayv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.yfazqb.com/Article/details/gnsnktxga.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/gjadwsyay.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/gcmtseahs.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/goethkfkj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gkovdogwt.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/ggqhxqiun.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gxctcsgiz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.epnwcf.com/Article/details/gbsnseppq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.tarul.cn/Article/details/gsbueahhn.sHtML

[U67] PHP：处理文件上传
来源：http://wap.tarul.cn/Article/details/gjmnylaah.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gtsjeezph.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gnitihift.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.sjlbkw.cn/Article/details/gkizpjuex.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gwejzydnr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.vehdjk.com/Article/details/gmenplqjy.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.vehdjk.com/Article/details/gvxqxurgr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.vehdjk.com/Article/details/gfmuvedjs.sHtML

[U71] PHP：抛出异常
来源：http://www.share.vehdjk.com/Article/details/gfvksjglu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.epnwcf.com/Article/details/gijvajznz.sHtML

[U72] PHP：写错误日志
来源：http://wap.epnwcf.com/Article/details/gwudxxfxl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/gxfmkevik.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.epnwcf.com/Article/details/ghjmadgen.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.tarul.cn/Article/details/gtjfkbgrb.sHtML

[U74] PHP：读取环境变量
来源：http://blog.epnwcf.com/Article/details/gcjdrekzj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gvknxhzfc.sHtML

[U75] PHP：依赖注入
来源：http://mobile.sjlbkw.cn/Article/details/gfvghxtnd.sHtML

composer require psr/container
来源：http://baike.epnwcf.com/Article/details/glmbxwuxn.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.tarul.cn/Article/details/gcbapjhim.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/ghloluhwk.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gyadmqcme.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/gqygvzovq.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gqvkfhusp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.yfazqb.com/Article/details/gbvahjwtu.sHtML

[U79] PHP：静态分析
来源：http://mobile.fktsv.cn/Article/details/goqcicdbd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gvrbmkigm.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/grekngkkh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gtcuhmgdt.sHtML

[U81] JS：初始化项目
来源：http://m.share.epnwcf.com/Article/details/gmfgnffej.sHtML

npm init -y;  npm i express
来源：http://blog.epnwcf.com/Article/details/gerfnhvzk.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fktsv.cn/Article/details/gbxqaxsjp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.tarul.cn/Article/details/gbzutmulk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.epnwcf.com/Article/details/ghvcjoroz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.tarul.cn/Article/details/ggounuile.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/gqmruibsk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.yfazqb.com/Article/details/gfifqtoki.sHtML

[U85] JS：可选链
来源：http://blog.tarul.cn/Article/details/gsyjypsnq.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/gizcyxeti.sHtML

[U86] JS：空值合并
来源：http://mobile.bbcook.cn/Article/details/ggwvwoamo.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gorifrgdv.sHtML

[U87] JS：解构默认值
来源：http://wap.tarul.cn/Article/details/gpsbtwfzn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.yfazqb.com/Article/details/grdzaskig.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.tarul.cn/Article/details/gmorczkmh.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gzaoymcdw.sHtML

[U89] JS：数组去重
来源：http://m.share.sjlbkw.cn/Article/details/gxhdvvjan.sHtML

[...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/givqlyjsh.sHtML

[U90] JS：数字数组排序
来源：http://read.share.yfazqb.com/Article/details/gbyfbwode.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gckepkbdq.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.sjlbkw.cn/Article/details/guibnfxri.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.vehdjk.com/Article/details/geixyanua.sHtML

[U92] JS：深拷贝
来源：http://read.share.vehdjk.com/Article/details/gyvcwfciq.sHtML

structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/geavhaael.sHtML


<!-- 参考信息 -->