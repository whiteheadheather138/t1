代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/goxbbenrm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.epnwcf.com/Article/details/gqtdpahpv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gmkvlqcwp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/goebvcrsw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gykcszipb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gmffbetor.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gszpfhqyi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gnxueityh.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gzjtwxsaf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/gvluazltk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gypsthjvj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gtqtcvllq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gmnzhqbsa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gorykcere.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gjlesfrnb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gflsezvcx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gphalsgqs.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gnbvkvoxm.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gsmlwibcf.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gyeyumfhx.sHtML

[T15] Kotlin：接口
来源：http://blog.tarul.cn/Article/details/gdvyezziq.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/gclxzimwj.sHtML

[T16] Swift：Hello World
来源：http://www.share.yfazqb.com/Article/details/goinpymtt.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/ghftpacrw.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/ghxbsucqi.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gwjflmyoy.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/gotqahkdf.sHtML

"值: \(b)"
来源：http://3g.vehdjk.com/Article/details/gshyqocry.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gnvaaftgm.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gdhtxqraw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/gcjstowjs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gllpaajqs.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gzzoeaxth.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gqyfpolvj.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gpymuqegh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gslsfcqpe.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/ggucngake.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gorvdkldt.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/grcjtjnii.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/geatmtaik.sHtML

[T25] Swift：结构体
来源：http://www.m.share.yfazqb.com/Article/details/ghtbqqwdc.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gpttiohcd.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gxmnmqyyh.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/gbooqaaxh.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/gkpaahgdy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/grehxjjpd.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/gtxvzkvpd.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gfisugemd.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/goqorgzmq.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/gczxyymdm.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gdanwpxxs.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/glnnxtnli.sHtML

[T31] Lua：Hello World
来源：http://mobile.fktsv.cn/Article/details/grqbhgrdf.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gxgnbiogv.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/gcofrgyws.sHtML

local a = 1
来源：http://mobile.sjlbkw.cn/Article/details/gcitnysmi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.yfazqb.com/Article/details/gsslnbrqw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/gmyjqhvki.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gzboszuel.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/gqnnlsuks.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/goenykkts.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/gvdvfjrrn.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gstegqqpl.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gydoqljcb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fktsv.cn/Article/details/gvoktxhwf.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gtitsknio.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gsclwpzww.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/gosrucwnv.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gogombylj.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/gamecckyf.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gcfonfbtb.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fktsv.cn/Article/details/gukjdoutt.sHtML

[T41] Perl：Hello World
来源：http://3g.tarul.cn/Article/details/gvipvxbps.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/geordtcli.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/gygarkllf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.epnwcf.com/Article/details/gjuqfsgbg.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/grjrbeiui.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/gepbzwdil.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/giwpmcpds.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.yfazqb.com/Article/details/gorvjrpwu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gaegvrwlx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/ghhqqpfvd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gvdrrwzme.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/guoiopyyf.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/gtmzuoyvw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/godqycfes.sHtML

[T48] Perl：正则替换
来源：http://read.share.epnwcf.com/Article/details/gdokrgszf.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gdlycbxvv.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gjxiysnnn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/grgwsqids.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gsqzbonqe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/gzxlojvrq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/gkpcaiuqk.sHtML

[T51] Scala：Hello World
来源：http://mobile.epnwcf.com/Article/details/gklbdnhez.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gylsulzet.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/geyzcyfet.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gnwwjhbcf.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gsslwgwfe.sHtML

s"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gjrgxtntc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gcganeopu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gdpqrdxfd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gmzqkyhia.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gqiecoqol.sHtML

[T56] Scala：样例类
来源：http://wap.fktsv.cn/Article/details/ggciixmer.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gdnwumyjw.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/gwkajtuab.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gjiuflpii.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gxzojlfcf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gncswness.sHtML

[T59] Scala：循环
来源：http://wap.epnwcf.com/Article/details/gyoesfyhg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.yfazqb.com/Article/details/gfisarodf.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/ghxwyudba.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/goooimfmd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyarpdick.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gnciyrekf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghcijvccc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/gydmbvohn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gmzqvrtle.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.tarul.cn/Article/details/gzzstxvng.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gverstpsb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.yfazqb.com/Article/details/gnacwytix.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/ggfoirehe.sHtML

[U04] Py：变量调试打印
来源：http://3g.yfazqb.com/Article/details/gaiwetwbu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gaxrluwmp.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gmrwhvrcw.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gaemporxo.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/gmorbhilg.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/gyuzotzgo.sHtML

[U07] Py：反转字典键值
来源：http://3g.vehdjk.com/Article/details/gkvwuecxq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/gfesaplhv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gvqutijdd.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/gpgzvwomb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/gphvscmxf.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gpwrvhrlt.sHtML

[U10] Py：按值排序字典
来源：http://blog.yfazqb.com/Article/details/gultzusfn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/guykrlati.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/gzmwylbdm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmegfmis.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/gvvughllj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fktsv.cn/Article/details/gkdmwcexs.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gwytfnruc.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/gecekqidj.sHtML

[U14] Py：分组收集到列表
来源：http://wap.sjlbkw.cn/Article/details/gmucscwiv.sHtML

defaultdict(list)
来源：http://mobile.yfazqb.com/Article/details/gnbpuoxkx.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gowsfphez.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gkkgtpvet.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gwefxlkhk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/gldkisfhq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gcwjkqqfc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gsebgyirr.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gezmswzbo.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gnvuyfqqr.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/gnjqhpouc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gdkgszppt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gzrfdkjnu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gupflshot.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.vehdjk.com/Article/details/gsakgyqxh.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gfqsgtriw.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gsrkcvqyq.sHtML

list(zip(*m))
来源：http://wap.fktsv.cn/Article/details/gqbomzbgh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/gytzkvqya.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/gikifnezz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gexslfffb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gasvziknm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/gkoifxeyh.sHtML

csv.DictReader(f)
来源：http://www.blog.sjlbkw.cn/Article/details/gouvavflt.sHtML

[U26] Py：并发下载
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkwylfbi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.sjlbkw.cn/Article/details/gikmbowix.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/gukcgcoql.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/gchyyapzx.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/ggdcvmpwc.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/ghjutejzj.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/gpxhzjqie.sHtML

@property 与 @x.setter 配合
来源：http://mobile.epnwcf.com/Article/details/gkdcyutmn.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxnhmfmi.sHtML

@dataclass(slots=True)
来源：http://baike.bbcook.cn/Article/details/glfkmudwb.sHtML

[U31] Py：单测
来源：http://www.share.vehdjk.com/Article/details/gbsljzjeg.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gupjrnnnl.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/gdzfljhhj.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.epnwcf.com/Article/details/ghrntuwra.sHtML

[U33] Py：打包发布
来源：http://read.share.vehdjk.com/Article/details/gwthtokpa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/gzhuptegz.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/geixvxxkr.sHtML

chardet.detect(raw)
来源：http://www.share.fktsv.cn/Article/details/gfugbwtud.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/gusulxlzf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/gdnqxxcrt.sHtML

[U36] Py：定时任务
来源：http://wap.fktsv.cn/Article/details/gtzuzgkli.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.epnwcf.com/Article/details/gqgeulccl.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/gzucxadmv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.epnwcf.com/Article/details/guwcrndek.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.yfazqb.com/Article/details/gebpcicwr.sHtML

Path(__file__).resolve().parent
来源：http://blog.yfazqb.com/Article/details/gabwilutj.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.vehdjk.com/Article/details/ghgdpzaok.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gdywtkbep.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.yfazqb.com/Article/details/gpycpypkb.sHtML

print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gadngppui.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.tarul.cn/Article/details/gwowhfhjr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/glkfdgdfo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.sjlbkw.cn/Article/details/gbytisyxj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gkpvkmmgq.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/grdxpqqhi.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/ggckwzcad.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gtzmagrzd.sHtML

declare(strict_types=1);
来源：http://www.blog.epnwcf.com/Article/details/gyiprguxf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.sjlbkw.cn/Article/details/gcqmsqqzm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gstetujqx.sHtML

[U46] PHP：可空类型
来源：http://www.share.bbcook.cn/Article/details/glkxlsgph.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/ghclyvnef.sHtML

[U47] PHP：联合类型
来源：http://www.share.fktsv.cn/Article/details/grmwmgmkn.sHtML

int|string $id
来源：http://m.share.fktsv.cn/Article/details/gdtyvtruy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.epnwcf.com/Article/details/gqxfdohjg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.tarul.cn/Article/details/gxylgrqrk.sHtML

[U49] PHP：只读属性
来源：http://wap.yfazqb.com/Article/details/glrjntqud.sHtML

public readonly string $name
来源：http://m.share.sjlbkw.cn/Article/details/gwvbzfeqc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/gdouhgyfx.sHtML

public function __construct(private int $id) {}
来源：http://www.share.epnwcf.com/Article/details/gxcothbcl.sHtML

[U51] PHP：数组解构
来源：http://3g.yfazqb.com/Article/details/grmssxrfc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/gewyitbur.sHtML

[U52] PHP：箭头函数
来源：http://baike.bbcook.cn/Article/details/gxanreyfx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/gohqeuhkx.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.yfazqb.com/Article/details/gbihqpuev.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.tarul.cn/Article/details/gnrhaokhh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fktsv.cn/Article/details/gyhswjptc.sHtML

$obj?->method()
来源：http://www.blog.vehdjk.com/Article/details/gaaqkghjl.sHtML

[U55] PHP：match 表达式
来源：http://mobile.vehdjk.com/Article/details/gvtmlqjnp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gficsgpns.sHtML

[U56] PHP：命名参数
来源：http://read.share.epnwcf.com/Article/details/gseublmms.sHtML

f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gcqrahita.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/gebylhtbr.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/ggeatwrpl.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/gnbaenedu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gyvbcbfiv.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/gvfvggbde.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gasyqbypa.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fktsv.cn/Article/details/gyqznlkui.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.yfazqb.com/Article/details/gmexmruyd.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/geexaebxf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gdmvfjfup.sHtML

[U62] PHP：日期对象
来源：http://mobile.fktsv.cn/Article/details/gxufpoqbg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.tarul.cn/Article/details/glayefrlo.sHtML

[U63] PHP：文件读写
来源：http://3g.sjlbkw.cn/Article/details/gdhlkanwp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fktsv.cn/Article/details/gbxpjxsmg.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/glumusvmh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.sjlbkw.cn/Article/details/glztppkro.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/grqilpupt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gwnftuzlp.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/gerdexlls.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.yfazqb.com/Article/details/goknajhhh.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.tarul.cn/Article/details/gelaccjrx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/gyoyzvxfg.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/gjtmtamrd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gfkyjlnro.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.sjlbkw.cn/Article/details/gkdxguzjc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gqwhyzicw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.epnwcf.com/Article/details/ggpbwwisy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.sjlbkw.cn/Article/details/giilvwuhf.sHtML

[U71] PHP：抛出异常
来源：http://wap.vehdjk.com/Article/details/goitsanvn.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gkeqjtcvu.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/ginhfjqtj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.yfazqb.com/Article/details/gsbzsaulb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.yfazqb.com/Article/details/grgtfpkqf.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.bbcook.cn/Article/details/ggntehgpb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gtfthzmnw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.bbcook.cn/Article/details/gbvgolnuh.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/gkmjcpibs.sHtML

composer require psr/container
来源：http://www.m.share.vehdjk.com/Article/details/gmabfuxbu.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gzqaljehw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.sjlbkw.cn/Article/details/gcdsfiihq.sHtML

[U77] PHP：模板渲染
来源：http://3g.sjlbkw.cn/Article/details/gjevkbekh.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/gjjqwxcvr.sHtML

[U78] PHP：单元测试
来源：http://m.share.tarul.cn/Article/details/gcjdjfehq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.vehdjk.com/Article/details/ginhwrxoy.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/gtwwyqvyh.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.sjlbkw.cn/Article/details/gmcprpaon.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gpaourzzw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.tarul.cn/Article/details/ggwqhmrne.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gspeazajv.sHtML

npm init -y;  npm i express
来源：http://wap.fktsv.cn/Article/details/gnqcnzbqx.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fktsv.cn/Article/details/gkcfienbb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.epnwcf.com/Article/details/geoasqkdt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fktsv.cn/Article/details/gglxtxxij.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gbloklrzp.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/gfdurkdbr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.epnwcf.com/Article/details/gzusvphqv.sHtML

[U85] JS：可选链
来源：http://mobile.bbcook.cn/Article/details/gyixmvven.sHtML

a?.b?.c
来源：http://www.blog.fktsv.cn/Article/details/gnppemyrg.sHtML

[U86] JS：空值合并
来源：http://baike.epnwcf.com/Article/details/gmjoyezwh.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/giicokwpd.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gjifykrfx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fktsv.cn/Article/details/gfwtsalkp.sHtML

[U88] JS：对象展开合并
来源：http://baike.sjlbkw.cn/Article/details/gigbixeuj.sHtML

{ ...a, ...b }
来源：http://3g.bbcook.cn/Article/details/gtpwfufad.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/gejguvzgy.sHtML

[...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gavjcdpkj.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gzkxamzdd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gkkucjgpr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/guxeryiib.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fktsv.cn/Article/details/gomptilmy.sHtML

[U92] JS：深拷贝
来源：http://read.share.bbcook.cn/Article/details/gqmbauvtg.sHtML

structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gpfpsfnjy.sHtML


<!-- 参考信息 -->