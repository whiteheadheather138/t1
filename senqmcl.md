代发 wailian999

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gaqpcdeby.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gvzmlhybc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/glghmdnlw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.tarul.cn/Article/details/ghfwaqjlb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/ggippjjtb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/gtycerepu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/glebwjqdw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/ghhubclaj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.bbcook.cn/Article/details/gawscaeyv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gtavbwfhq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gzirmihzi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.sjlbkw.cn/Article/details/golofeypq.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/ganqelpyc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.sjlbkw.cn/Article/details/gdmzwwjvy.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gwagtmbjm.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/guqnmchaj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/gaqkjqyho.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gdvqdpiia.sHtML

[T14] Kotlin：循环
来源：http://wap.yfazqb.com/Article/details/ggxkjvsir.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/ggfrmzfbn.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gievszllh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gfhvgksqb.sHtML

[T16] Swift：Hello World
来源：http://m.share.bbcook.cn/Article/details/gwjhehkya.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gxrvtruju.sHtML

[T17] Swift：变量与常量
来源：http://3g.epnwcf.com/Article/details/gortwbobg.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gyuazjkie.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gtasxruuw.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gxkfjdjpx.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/gvbxfeeok.sHtML

if let n = opt { print(n) }
来源：http://wap.epnwcf.com/Article/details/gcdfuqfwz.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/grggacjkd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gunvnkhce.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gnesemnuu.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/grrxzryfe.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/gsbzhyqbl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/gblmymfyy.sHtML

[T23] Swift：函数
来源：http://read.share.yfazqb.com/Article/details/gwvpnrorw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gauuwfmir.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gjqqgsxob.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/glsfqovkl.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gmsjvpzko.sHtML

struct P { var x: Int }
来源：http://mobile.bbcook.cn/Article/details/gbzlqsbxa.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/gnavxsdzm.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/gogaborzb.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gjjhbelgi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gxhrpckom.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gzobrgppb.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/ganzsxffc.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/gcmlrpyzu.sHtML

guard let x = opt else { return }
来源：http://3g.bbcook.cn/Article/details/gemtgcrjy.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gdugnjfeb.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.sjlbkw.cn/Article/details/goumwokmp.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gzvunzpoz.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gzrvokivx.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gnrtarwwl.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/gqbjtzyzq.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/gvpxypxkt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.vehdjk.com/Article/details/gjaedlcfh.sHtML

[T34] Lua：遍历表
来源：http://blog.sjlbkw.cn/Article/details/gomsvomeo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gtcgrytff.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/gbshjgjii.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gixchnavp.sHtML

[T36] Lua：函数
来源：http://baike.sjlbkw.cn/Article/details/gohnsqvmj.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gstflymjp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/govdrdgpe.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gvuwtudvy.sHtML

[T38] Lua：条件
来源：http://www.m.share.epnwcf.com/Article/details/geetegsfc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.tarul.cn/Article/details/gceqvsolk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/grofocwah.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/grroxgnwc.sHtML

[T40] Lua：元表
来源：http://baike.epnwcf.com/Article/details/gujntmpme.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gdyxwtiqd.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/gohbcjafh.sHtML

print "Hello\n";
来源：http://www.share.tarul.cn/Article/details/gohfkijog.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/greygdejk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/guwpepltd.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gfoppxdei.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gwecsvecz.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gwsxznanv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gsxxtzjrq.sHtML

[T45] Perl：数组遍历
来源：http://wap.fktsv.cn/Article/details/gxzhxumsf.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/gnswintky.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/ghswjfyxi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/gyvvteati.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gtbsguczg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/gucbhfsxh.sHtML

[T48] Perl：正则替换
来源：http://blog.fktsv.cn/Article/details/grlolhbge.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/guvayhhnt.sHtML

[T49] Perl：函数
来源：http://read.share.epnwcf.com/Article/details/grflnsntg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gsemrlgsm.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gxfqqrard.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.yfazqb.com/Article/details/gctgxrcrk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/ghslcgfxm.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/gktxablnh.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gdmqkprsa.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gshidknjs.sHtML

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/gfzphafxh.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gsilzjeql.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gsowdvtam.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gnmurzopz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gqyukazrs.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/gzdnczsjg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fktsv.cn/Article/details/gtykhtaov.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/glurhjpgn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gmdxvjevu.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/glnjonaln.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/grlpjwnbo.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.vehdjk.com/Article/details/gazioftmn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gybzravsa.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/gsbqqtjru.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gclcsyjcg.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/grpyhmfup.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fktsv.cn/Article/details/goarvxdjy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gggytodhn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/gktuksnkt.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmdexbjjh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/glsfmobgy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gvvzccdqa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.sjlbkw.cn/Article/details/gzezivllr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gqxoymtlm.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gutnvxjty.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gviammsmu.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/gsucrlekv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/guwemkhgl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gxoxfdccl.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gijojluvd.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/gihvzntbs.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gfmqjgxlf.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/gnstygedn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/gsjfxpygo.sHtML

[U08] Py：展平二维列表
来源：http://blog.epnwcf.com/Article/details/gylixnxop.sHtML

[y for x in nested for y in x]
来源：http://read.share.epnwcf.com/Article/details/gbvzspujd.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fktsv.cn/Article/details/gueupximx.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gtkflreyx.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gmzuhmcow.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/gcmbyvpav.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gwpkeqdun.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gyahvhmqy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gypfmfnam.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gidfxpomb.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gefrdwfac.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gyefrgtxh.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gclkcyrno.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/ggdjmurit.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gsjeiaahu.sHtML

t = time.perf_counter()
来源：http://www.blog.fktsv.cn/Article/details/guhjhlise.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gdqrivmti.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.epnwcf.com/Article/details/gkgzzpcbn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.sjlbkw.cn/Article/details/ggiylvrnm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.epnwcf.com/Article/details/gkefjncnd.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/gkvxddjpx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/goylrlmrc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gfcghnizr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/gbbkrntox.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gxlpbljfo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gzpsojdyx.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gqxypvfdy.sHtML

@contextlib.contextmanager
来源：http://read.share.bbcook.cn/Article/details/gfwjmczuv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fktsv.cn/Article/details/gorbmgvly.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/gnirqnepp.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/gvghidift.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.tarul.cn/Article/details/gnlntudav.sHtML

[U24] Py：路径操作
来源：http://www.m.share.epnwcf.com/Article/details/gwrqwcsrj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/grksfgnkc.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/guvmtmnit.sHtML

csv.DictReader(f)
来源：http://baike.vehdjk.com/Article/details/gazrbpksp.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gqgefhnfs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/gxjzmhxgx.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gcyoemhxf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gwwwuhbwj.sHtML

[U28] Py：类型别名
来源：http://wap.fktsv.cn/Article/details/gvratkglc.sHtML

UserId = int
来源：http://mobile.tarul.cn/Article/details/gotkfditm.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/grijslwtg.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/gjjlkqtka.sHtML

[U30] Py：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gvguirdso.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/gzkqplbud.sHtML

[U31] Py：单测
来源：http://www.share.yfazqb.com/Article/details/gbwuahgeq.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gfggdevmw.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/gxpizhrfc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.tarul.cn/Article/details/gybaaapyn.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gfznnpdok.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.bbcook.cn/Article/details/gprjkpddh.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/guqhjkozc.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/gicgtsaqz.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/godyaiiqs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fktsv.cn/Article/details/gtzjesyec.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/ghpfbdwfb.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.tarul.cn/Article/details/gbyhkaiqy.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gxbozsayl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.epnwcf.com/Article/details/gywuysezd.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/guxzkmoex.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.yfazqb.com/Article/details/gaoljkiqf.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/gbodejkmo.sHtML

sys.stdout.isatty()
来源：http://www.share.vehdjk.com/Article/details/gncsanzxq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fktsv.cn/Article/details/grduunwey.sHtML

print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gdmzzgyea.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/gcxczxklf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gyktabbyc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/gnmabmuev.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.yfazqb.com/Article/details/gtarcypho.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gnzhvkblm.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gvlvevrhj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gkidzeugq.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/gbotzqyxs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.yfazqb.com/Article/details/gqrawuriq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gclzgqznm.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gfqygexho.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/ghoamzbpq.sHtML

[U47] PHP：联合类型
来源：http://baike.tarul.cn/Article/details/gbupcnuyr.sHtML

int|string $id
来源：http://mobile.yfazqb.com/Article/details/guxbmylla.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.tarul.cn/Article/details/gvrytyqmq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gsupxxxsn.sHtML

[U49] PHP：只读属性
来源：http://www.share.yfazqb.com/Article/details/gtdetrqgc.sHtML

public readonly string $name
来源：http://read.share.bbcook.cn/Article/details/gwpiafkgx.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/gcqtpokvs.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geyymexsb.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gnnvkhdki.sHtML

[$a, $b] = $arr;
来源：http://www.blog.epnwcf.com/Article/details/gpvazwnlm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.yfazqb.com/Article/details/geyqfcslo.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/gwwybiofy.sHtML

[U53] PHP：空合并运算符
来源：http://wap.epnwcf.com/Article/details/gwlsnxmun.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gptzxjkob.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/gsaysnafv.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gtbeorqhl.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/gwvisgxxa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gohjvhifp.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/gtmpfuogo.sHtML

f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gaczemkex.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gbxwdside.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/goozmljaw.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gmveooyty.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.yfazqb.com/Article/details/gymclkstb.sHtML

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/gruvstftj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gotyltgnp.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fktsv.cn/Article/details/gtvnyohgc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.epnwcf.com/Article/details/gqhkaidnh.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/gaztrniqs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gqwkondvz.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gzhjczmrb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.epnwcf.com/Article/details/gvasxqele.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/gbqbigpig.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gdfkexkrf.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/gvwefvbbf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.tarul.cn/Article/details/gyvgabcsa.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/gilbfrigj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/gexptgzde.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.sjlbkw.cn/Article/details/gwgnrxony.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/glvdfwefz.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/gcwvowgep.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fktsv.cn/Article/details/gvmhmodhg.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.sjlbkw.cn/Article/details/gkudhsyov.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fktsv.cn/Article/details/gtaqzgbeq.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.sjlbkw.cn/Article/details/gobpmkbpn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gbdypvlzk.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.epnwcf.com/Article/details/gwrzlllpq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.yfazqb.com/Article/details/gkrkvewnz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/gtcookeru.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/ggbuvigqi.sHtML

[U72] PHP：写错误日志
来源：http://3g.bbcook.cn/Article/details/gtbmmakib.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.sjlbkw.cn/Article/details/gysluuoqq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gdbryyiov.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fktsv.cn/Article/details/gifvmjhtz.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/gymgrbgdj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.epnwcf.com/Article/details/grrcelxem.sHtML

[U75] PHP：依赖注入
来源：http://blog.fktsv.cn/Article/details/gfguhlbrt.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gzcagwjvl.sHtML

[U76] PHP：简单路由
来源：http://blog.bbcook.cn/Article/details/gkciuvobt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.bbcook.cn/Article/details/gjesavxfh.sHtML

[U77] PHP：模板渲染
来源：http://3g.fktsv.cn/Article/details/gyfbxdzxi.sHtML

composer require twig/twig
来源：http://baike.yfazqb.com/Article/details/gepghjqki.sHtML

[U78] PHP：单元测试
来源：http://baike.tarul.cn/Article/details/glbqhaipl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.sjlbkw.cn/Article/details/gcmrekjct.sHtML

[U79] PHP：静态分析
来源：http://m.share.tarul.cn/Article/details/gtowsjpkw.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.tarul.cn/Article/details/gfgczjbqq.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/geqnlnzar.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gafrowirv.sHtML

[U81] JS：初始化项目
来源：http://blog.tarul.cn/Article/details/gguzagabs.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gjvxdkzje.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/grftponlx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.epnwcf.com/Article/details/gdujldoir.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.epnwcf.com/Article/details/gzpnvctii.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gsglqsics.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gibnhmyzk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.yfazqb.com/Article/details/gdgepxkre.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gfrzznbof.sHtML

a?.b?.c
来源：http://www.share.bbcook.cn/Article/details/gslyxtvae.sHtML

[U86] JS：空值合并
来源：http://baike.yfazqb.com/Article/details/ggesxkvbe.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/glubakdiz.sHtML

[U87] JS：解构默认值
来源：http://read.share.vehdjk.com/Article/details/gddffrweg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fktsv.cn/Article/details/guwgcrnhc.sHtML

[U88] JS：对象展开合并
来源：http://read.share.sjlbkw.cn/Article/details/gyoozztcx.sHtML

{ ...a, ...b }
来源：http://m.share.vehdjk.com/Article/details/gprvnsotq.sHtML

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gzkyxrldy.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/ghildxaex.sHtML

[U90] JS：数字数组排序
来源：http://baike.tarul.cn/Article/details/gjzlhoujf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gdqbkmzox.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/gkhidpafb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.yfazqb.com/Article/details/gdmkpwqay.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcytwybl.sHtML

structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/ghfoymxxy.sHtML


<!-- 参考信息 -->