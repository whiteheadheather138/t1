代发 wailian999

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gdcxakimq.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/glukmkgbw.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/grhppcqhh.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gxnfyhjye.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/gecovzssf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.tarul.cn/Article/details/gapzlmhlv.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gjeqsbyns.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gtkcqzymw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gpugttikf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gxmtpwmuz.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gwthvtyey.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/grebshthk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/grpkwiibq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gjopjiybh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gjsqxwtxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/ghriyspwk.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gdysludhf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gwjatqzof.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gojxderbj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gytivqgez.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/grfdfxrnp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gtvwdruwq.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gkrqnztzu.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gjbvtulci.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gewtpeooh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gvyjeclag.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gijztpziu.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gubnzrtfh.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gqbfblcdv.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gdagiikzk.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gqgdidppg.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gfubtqepo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gbcienrkp.sHtML

if let n = opt { print(n) }
来源：http://read.share.yfazqb.com/Article/details/gvqmiqtiv.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/glikxuuto.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.epnwcf.com/Article/details/gkrmixviu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gclvgkkxk.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gfdsncupx.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gmvaknzyg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gmyuvtdyy.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gjhltoayq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/gzbqbfdfb.sHtML

[T24] Swift：闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gviqiiykg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gbnlawiov.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gjwfuxzyc.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gyjhrqoth.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/giwiykrmr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.yfazqb.com/Article/details/glgcnuzfq.sHtML

[T27] Swift：错误处理
来源：http://www.share.vehdjk.com/Article/details/grdlbzjfg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/graettjlf.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gvivntsvn.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gvxsumpnw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.tarul.cn/Article/details/gayitsnvh.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/gmgvpdnjy.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gmftlljoo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/gmqltlvoo.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gndhygdij.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gdggrlrbm.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gbwcqnexn.sHtML

local a = 1
来源：http://3g.sjlbkw.cn/Article/details/gupevfpvj.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/gzogebwzj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.bbcook.cn/Article/details/gnqrcpmmh.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gozdvrxwi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.epnwcf.com/Article/details/ginuurqya.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gbjjtbecc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/genvjvqmz.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gkggnryrp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/gxxdcvyko.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/grnksglxn.sHtML

"a" .. "b"
来源：http://read.share.bbcook.cn/Article/details/gafunvjhx.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gygehhtpz.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gkzswttrc.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/ggwmqqyoa.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/gyhqaolzy.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gdicdkjdo.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/goyusuvjy.sHtML

[T41] Perl：Hello World
来源：http://read.share.epnwcf.com/Article/details/gomzqmfld.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/ggmasjyiv.sHtML

[T42] Perl：变量类型
来源：http://read.share.fktsv.cn/Article/details/gphyoaqcm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/glfzmrgfe.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gujsdneki.sHtML

"值: $a"
来源：http://m.share.bbcook.cn/Article/details/gnhyqqhbv.sHtML

[T44] Perl：条件
来源：http://mobile.vehdjk.com/Article/details/gtyoeaoqs.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fktsv.cn/Article/details/gojzjlcpe.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gyfudkrhb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghyfniome.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.bbcook.cn/Article/details/gaeosdpor.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gdzvexjkp.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gztjdwnhu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.bbcook.cn/Article/details/gmcamtfdq.sHtML

[T48] Perl：正则替换
来源：http://mobile.bbcook.cn/Article/details/genwsbkwa.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjdyrrmm.sHtML

[T49] Perl：函数
来源：http://www.blog.yfazqb.com/Article/details/gkonbmklh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gummvjdbn.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gvehdtzev.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/grchaaysg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.bbcook.cn/Article/details/gzbudtptk.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gycapxpts.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gwphjageu.sHtML

[T52] Scala：变量
来源：http://www.m.share.bbcook.cn/Article/details/gdxfuhqag.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/giiyofsir.sHtML

[T53] Scala：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gyzqrdajt.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gayiwxctk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gahmqdnun.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gkkmfrajl.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/grbhkiotl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gfqcuuyls.sHtML

[T56] Scala：样例类
来源：http://3g.tarul.cn/Article/details/gcjiwfecz.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/gekqmspkq.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gbyxdtgpa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gginsdnia.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gumgxqpgv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/gywvvostq.sHtML

[T59] Scala：循环
来源：http://www.blog.vehdjk.com/Article/details/gehbbdchj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gmulijqls.sHtML

[T60] Scala：折叠
来源：http://baike.yfazqb.com/Article/details/gtljmggfu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gewhrlqvg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyfcovpjw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/gmlfmwnoa.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gingamkxj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gvynxkkce.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.epnwcf.com/Article/details/glspnlxah.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/gjpnvgsss.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/grqvwzfei.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/gwdgadfhh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.vehdjk.com/Article/details/ghvrrslvq.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/gdhgtieca.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gnojdatbh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/ghigjoigd.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gpucfrbzp.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/ghkeyavea.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/grxcbxyrh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gntnmnfza.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gcxtovajk.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gfevvszsf.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/gzobibgka.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gompnjewy.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/gigcsxfrl.sHtML

[U10] Py：按值排序字典
来源：http://baike.fktsv.cn/Article/details/gjczqzxci.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gwmyyciuj.sHtML

[U11] Py：生成器表达式
来源：http://baike.fktsv.cn/Article/details/giknitepi.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gocwabupq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gzxuxvypf.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/gvsjqslvp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.bbcook.cn/Article/details/gfbdojypd.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/geyggmksy.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/gdrqbrmhb.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gvvapijhy.sHtML

[U15] Py：高精度计时
来源：http://www.blog.epnwcf.com/Article/details/gztwqrgcv.sHtML

t = time.perf_counter()
来源：http://wap.vehdjk.com/Article/details/gbfdeloqn.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/gliuajves.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fktsv.cn/Article/details/godarsrpm.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/gqocozazj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gytatcnsr.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gkfgmkboy.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/glymnwudi.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gohbjfncp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/gnjgyhina.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/grddzbpnq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.bbcook.cn/Article/details/gfkavftoe.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/ggdvctbml.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/garnkgwoi.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.vehdjk.com/Article/details/garxwysin.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gtctvagas.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/gwnqacxit.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gihyaaeod.sHtML

[U24] Py：路径操作
来源：http://www.blog.epnwcf.com/Article/details/ghpmzsucr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/ganqklitb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.vehdjk.com/Article/details/gtngdsmbe.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gxrvutyya.sHtML

[U26] Py：并发下载
来源：http://read.share.yfazqb.com/Article/details/gnugboweh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.tarul.cn/Article/details/gvsuvvbsl.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/gbkudmrrz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gavkxpsgs.sHtML

[U28] Py：类型别名
来源：http://wap.fktsv.cn/Article/details/gqqqtiyjk.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gtojepywc.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/glwvkyyos.sHtML

@property 与 @x.setter 配合
来源：http://www.share.sjlbkw.cn/Article/details/gwumqqzin.sHtML

[U30] Py：数据类
来源：http://blog.epnwcf.com/Article/details/ggxhczrtc.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gpopyqddr.sHtML

[U31] Py：单测
来源：http://baike.vehdjk.com/Article/details/goinrxiih.sHtML

python -m pytest -q
来源：http://3g.tarul.cn/Article/details/gsynnxkov.sHtML

[U32] Py：代码格式化
来源：http://read.share.sjlbkw.cn/Article/details/ghpxsfymo.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/ghldfrupb.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/gktndfgpe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gwooivosn.sHtML

[U34] Py：判断编码
来源：http://www.share.tarul.cn/Article/details/gpqlsnwgl.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gtayoqrjv.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/gefjwihho.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/gmvsgcfck.sHtML

[U36] Py：定时任务
来源：http://m.share.bbcook.cn/Article/details/ggaafbxgv.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/gegndfptc.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/glkxifani.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/gpkedqnmq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/grrosuivi.sHtML

Path(__file__).resolve().parent
来源：http://blog.fktsv.cn/Article/details/gobjtbibx.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.bbcook.cn/Article/details/ggjmipebf.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/ggilexcfz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/giiyljgga.sHtML

print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gbacgmfvu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/goibvtljh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.bbcook.cn/Article/details/grslvxvyg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.vehdjk.com/Article/details/geablwtnv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/gubhderqg.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/gltcmximm.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gwrprhlkk.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/gshlwixov.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/gbzuymksh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.vehdjk.com/Article/details/gjcwbjqyg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gdzzasalw.sHtML

[U46] PHP：可空类型
来源：http://blog.sjlbkw.cn/Article/details/gitpnqofy.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gdcjibsjz.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/gycgebdmc.sHtML

int|string $id
来源：http://www.share.epnwcf.com/Article/details/gtdtqidad.sHtML

[U48] PHP：纯枚举
来源：http://m.share.sjlbkw.cn/Article/details/gdgfiacbp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/glmymokzf.sHtML

[U49] PHP：只读属性
来源：http://3g.sjlbkw.cn/Article/details/gelwiinep.sHtML

public readonly string $name
来源：http://read.share.yfazqb.com/Article/details/gfonjojzm.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.epnwcf.com/Article/details/glhasnyoh.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuilzfjh.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gapifmsbt.sHtML

[$a, $b] = $arr;
来源：http://read.share.bbcook.cn/Article/details/gsuunhiii.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gwqifgfex.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.epnwcf.com/Article/details/gobrhibeu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.sjlbkw.cn/Article/details/gvzsmeofw.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/gflxjijbm.sHtML

[U54] PHP：空安全调用
来源：http://read.share.bbcook.cn/Article/details/gxkoyumlk.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/grkjgrvfe.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fktsv.cn/Article/details/ghckyskih.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gshlunxtx.sHtML

[U56] PHP：命名参数
来源：http://www.blog.bbcook.cn/Article/details/gjyilfpvh.sHtML

f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/ghupovsxr.sHtML

[U57] PHP：字符串插值
来源：http://mobile.epnwcf.com/Article/details/guispzhah.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gyuknndgt.sHtML

[U58] PHP：数组三件套
来源：http://mobile.yfazqb.com/Article/details/gvogcrfla.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/gdnfdyrgo.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gmdzkeubc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gddvsziqa.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gsrqbzjnu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.tarul.cn/Article/details/gjwgfcswz.sHtML

[U61] PHP：正则
来源：http://www.m.share.fktsv.cn/Article/details/ganwbmjma.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/gocrsmmvy.sHtML

[U62] PHP：日期对象
来源：http://mobile.vehdjk.com/Article/details/gevgstzpb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/gvngpalsp.sHtML

[U63] PHP：文件读写
来源：http://baike.sjlbkw.cn/Article/details/gpfkflngf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.sjlbkw.cn/Article/details/gumsimvts.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fktsv.cn/Article/details/gqcjkojxa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/gabulznvk.sHtML

[U65] PHP：会话
来源：http://3g.yfazqb.com/Article/details/gogcsylyq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gchwberqa.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fktsv.cn/Article/details/gjsneqysd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/gvsvtvoir.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.vehdjk.com/Article/details/glpqqapsi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/gtyhklece.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/gyrmqlttn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.vehdjk.com/Article/details/gyxrkojki.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.yfazqb.com/Article/details/ggbtxsfkt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.sjlbkw.cn/Article/details/gyfflwgqj.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fktsv.cn/Article/details/gdtphlfbo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.tarul.cn/Article/details/guzejzkgj.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gsyjfgzmm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjhyfelb.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/gfsvxlvfj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/gjkayiexg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gzzgydoyy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfyakmeo.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gtvocniop.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.tarul.cn/Article/details/gkqbkxxce.sHtML

[U75] PHP：依赖注入
来源：http://read.share.yfazqb.com/Article/details/gxbzokwry.sHtML

composer require psr/container
来源：http://read.share.fktsv.cn/Article/details/gxoltchfe.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/gsvtyjdvd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.bbcook.cn/Article/details/gfukoaymr.sHtML

[U77] PHP：模板渲染
来源：http://baike.bbcook.cn/Article/details/gzhixbmnj.sHtML

composer require twig/twig
来源：http://www.blog.tarul.cn/Article/details/gaebqfkgp.sHtML

[U78] PHP：单元测试
来源：http://wap.bbcook.cn/Article/details/grlslaxwc.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/gbvwsihhq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/gvkyeioee.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gyxcxfgeo.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/ggagjtkse.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fktsv.cn/Article/details/guvxgxtwu.sHtML

[U81] JS：初始化项目
来源：http://mobile.epnwcf.com/Article/details/gkovhltbs.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/gtrmenokc.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/glgituqhz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.vehdjk.com/Article/details/gkbxmfiyp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/gzbnubbee.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gooxukbtd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/gdliznnvt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.sjlbkw.cn/Article/details/gnqxaquic.sHtML

[U85] JS：可选链
来源：http://baike.yfazqb.com/Article/details/gghrmbjad.sHtML

a?.b?.c
来源：http://wap.yfazqb.com/Article/details/gyorocbfd.sHtML

[U86] JS：空值合并
来源：http://www.blog.sjlbkw.cn/Article/details/gzmwnrsjy.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gynrqhihe.sHtML

[U87] JS：解构默认值
来源：http://3g.bbcook.cn/Article/details/guyhgyavr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gxeoyggwk.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/gvzdoohhi.sHtML

{ ...a, ...b }
来源：http://baike.epnwcf.com/Article/details/gsqmfrqwr.sHtML

[U89] JS：数组去重
来源：http://m.share.epnwcf.com/Article/details/gmcurzfdr.sHtML

[...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gclyyxelt.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/giwvwjyum.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gvinzzcjp.sHtML


<!-- 参考信息 -->