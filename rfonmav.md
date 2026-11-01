代发 wailian999

[T05] Kotlin：when 表达式
来源：http://m.share.epnwcf.com/Article/details/gjzaiscnd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gbyouykyf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/gafxuazdg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gaxfewjis.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gdrdnjsjj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/guxbtbwzh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gnuqivghj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gjtkbfusu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuzlyugy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/ggnesgkja.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gwstgwqyh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gboglobis.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/grczugqbs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gzhquwxdd.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gmpxhjwkl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gfjyjtmrp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/gzislwqnb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fktsv.cn/Article/details/gkapdmemo.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gdwmviwhn.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gdsbyedds.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gljrzutds.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.sjlbkw.cn/Article/details/grgdmfjiu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gnqdmjggc.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/giqciyiel.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/grilmusdl.sHtML

var a = 1;  let b = 2
来源：http://m.share.vehdjk.com/Article/details/gbskgfmut.sHtML

[T18] Swift：字符串插值
来源：http://blog.tarul.cn/Article/details/giwnkqjko.sHtML

"值: \(b)"
来源：http://www.blog.tarul.cn/Article/details/guemcjneb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gexlrzpwr.sHtML

if let n = opt { print(n) }
来源：http://m.share.vehdjk.com/Article/details/gdrwvfyuq.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.bbcook.cn/Article/details/gepxkcvpf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/glkmgitsj.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gxjuagpcj.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gbjhhfotq.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gsctowbqf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/ghfnmnsqi.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gzpvsensc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.vehdjk.com/Article/details/gizqkngzf.sHtML

[T24] Swift：闭包
来源：http://blog.vehdjk.com/Article/details/gmanrgpqm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gkmamsnnb.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/givbffcck.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gxcpfjuwk.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gxesfwvqx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gkxbobpbg.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gkyhcwjxe.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gbfnslaei.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gshgrzkdx.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gittiifvo.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/ggstofudd.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gljipkvkz.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gjsezxowq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/grayapije.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gnhnuvbxa.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gakflhzuo.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gahxtlxqt.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gkezmgrcw.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/gvrrjzmwo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/giwwkaemy.sHtML

[T34] Lua：遍历表
来源：http://wap.epnwcf.com/Article/details/gcpbqrull.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gcjfckcte.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/ghharsqgj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/groasmthj.sHtML

[T36] Lua：函数
来源：http://blog.bbcook.cn/Article/details/gmykaslln.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gbjpctqip.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gpymiugik.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/gjlognzyf.sHtML

[T38] Lua：条件
来源：http://m.share.epnwcf.com/Article/details/gizxcbduu.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/gmlhrcgmh.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gjypnmwjr.sHtML

string.find(s, "%d+")
来源：http://3g.bbcook.cn/Article/details/gsdcikmmm.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gvnmsiypq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/gbmamijrt.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/guaxchqui.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/grduabxrs.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/gispucday.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/glmnblgrm.sHtML

[T43] Perl：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gzfwhkwti.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbxxzydw.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/gwtycgtoj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gdidasmur.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/gvpetkrsq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiytyedm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gucxtvmye.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gdghshqmo.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/ggcbrehsp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.tarul.cn/Article/details/gncfnlfyf.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/goofhekcr.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/glzkbjfim.sHtML

[T49] Perl：函数
来源：http://www.m.share.tarul.cn/Article/details/gnqbbtzps.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gykclobon.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/ggyflxsvg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gojslljll.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gmbpnvadv.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gdvjkvuiu.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gkjeiunvy.sHtML

[T52] Scala：变量
来源：http://read.share.sjlbkw.cn/Article/details/ghmqytiqc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gyovoclyz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/gqeltvyes.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/gwqgmjhak.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gjxjbyrrv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/gdzfcliqp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gxyolgynb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.yfazqb.com/Article/details/givlkkbqu.sHtML

[T56] Scala：样例类
来源：http://www.blog.sjlbkw.cn/Article/details/gcqyzbqwm.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/ghjscobop.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gcpgwfurd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gvvninzjc.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gjrseziwk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/gfillutde.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gnmsqlgkl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gqgjhvmhi.sHtML

[T60] Scala：折叠
来源：http://blog.sjlbkw.cn/Article/details/gjbrwipvy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.vehdjk.com/Article/details/gwjcfdygd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvsaqxizc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gvvcjtgla.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqeujyrat.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fktsv.cn/Article/details/gtbpbtcys.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/giujesjdz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gsazacvpv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gxugqjvrk.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gtvbnywtt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gjisbqogz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gkeanlqjb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fktsv.cn/Article/details/gypvahfjn.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gjxojskgb.sHtML

list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gmravttwe.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gzwoymjlz.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gdnsahuzm.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fktsv.cn/Article/details/gskeofapr.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gxgrckjjw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/gwpbkfrgq.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/giingowha.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.bbcook.cn/Article/details/gfufyhorf.sHtML

max(d, key=d.get)
来源：http://www.blog.tarul.cn/Article/details/gplahcnvu.sHtML

[U10] Py：按值排序字典
来源：http://baike.vehdjk.com/Article/details/ghnxqimup.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/gbqelemmn.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/ghmaemgao.sHtML

(x * 2 for x in arr)
来源：http://wap.bbcook.cn/Article/details/goboeaada.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.yfazqb.com/Article/details/gsipnzicz.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/gscokjkia.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fktsv.cn/Article/details/gqczljnmv.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/geoblqwyj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.yfazqb.com/Article/details/gpkmvniqg.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gwfuhcihf.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gljktzoac.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gszyylfhm.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.sjlbkw.cn/Article/details/gruulhhrz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gqfmtavay.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/gtvfiajdw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/gnfpwthfc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/gpxgwwgww.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.bbcook.cn/Article/details/gjmpgsecx.sHtML

[U19] Py：正则替换带回调
来源：http://baike.yfazqb.com/Article/details/geassonvo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gduenowbu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/glqgesaud.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gbdxvqlsv.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/ganatcdjw.sHtML

@contextlib.contextmanager
来源：http://m.share.bbcook.cn/Article/details/gkrodtfrm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fktsv.cn/Article/details/gcbubwfvj.sHtML

list(zip(*m))
来源：http://baike.yfazqb.com/Article/details/gnrqouwvl.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/gkztrojtq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.vehdjk.com/Article/details/gtdfndeys.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gmwybtnsn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gbxsflazj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/gzicoejjb.sHtML

csv.DictReader(f)
来源：http://read.share.yfazqb.com/Article/details/gcyktyhhb.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/gkiuenfag.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/gmivryciv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/genilzfwi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.epnwcf.com/Article/details/gyqtlowgf.sHtML

[U28] Py：类型别名
来源：http://3g.vehdjk.com/Article/details/gmbjeybsi.sHtML

UserId = int
来源：http://baike.tarul.cn/Article/details/gqgeoffkv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fktsv.cn/Article/details/gismnmpev.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhhvelmc.sHtML

[U30] Py：数据类
来源：http://www.blog.bbcook.cn/Article/details/gbfacadvg.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gyrhovhvk.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/gqflnnyyd.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/ghwouwlwy.sHtML

[U32] Py：代码格式化
来源：http://www.share.bbcook.cn/Article/details/gzqvtfupe.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/godxzbkjc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/grovshxln.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/gsnkbcphv.sHtML

[U34] Py：判断编码
来源：http://3g.fktsv.cn/Article/details/ggqijufot.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/gdccazfnh.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gvlevhmyk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/gttwknrpn.sHtML

[U36] Py：定时任务
来源：http://wap.tarul.cn/Article/details/gulxmitkp.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/gugwvmolc.sHtML

[U37] Py：读写 Excel
来源：http://baike.vehdjk.com/Article/details/gucxnrfqr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.epnwcf.com/Article/details/gkeypkwhj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gdjuudsfw.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gtepgsnhi.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/goqifdptz.sHtML

sys.stdout.isatty()
来源：http://baike.tarul.cn/Article/details/gshpsukle.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fktsv.cn/Article/details/gqjabhktb.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsoauogb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.yfazqb.com/Article/details/gydugkyzu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/guxyiuqvg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.tarul.cn/Article/details/geosyjiiv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.epnwcf.com/Article/details/ghjgdkefa.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fktsv.cn/Article/details/gvfsoasbo.sHtML

namespace App\Http;
来源：http://wap.sjlbkw.cn/Article/details/grmqzrwrq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.vehdjk.com/Article/details/glvuzelvs.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/gcrxeappt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/ghsziossm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/glbdaxyid.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.vehdjk.com/Article/details/gexbzkxpu.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/gyofthuvj.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/gylyhtkgk.sHtML

int|string $id
来源：http://baike.fktsv.cn/Article/details/gofxcjrtg.sHtML

[U48] PHP：纯枚举
来源：http://blog.bbcook.cn/Article/details/gphqleikq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/gvakpyorm.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gynxwllae.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/gggkhlyey.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.yfazqb.com/Article/details/gqnzrfagy.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/gelwtzcza.sHtML

[U51] PHP：数组解构
来源：http://blog.vehdjk.com/Article/details/gorwforoy.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.epnwcf.com/Article/details/gmitiknja.sHtML

[U52] PHP：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gatyhiwdc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.yfazqb.com/Article/details/gfcazmpzc.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.tarul.cn/Article/details/goqncfzrx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/ghpjxltuq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.tarul.cn/Article/details/gvgsebovq.sHtML

$obj?->method()
来源：http://www.blog.vehdjk.com/Article/details/gidqpfyga.sHtML

[U55] PHP：match 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gwkmcxdfr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/gpwepyqbi.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.bbcook.cn/Article/details/gdozjaias.sHtML

f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gdjuclecz.sHtML

[U57] PHP：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gzofqqran.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/gqxlbvtix.sHtML

[U58] PHP：数组三件套
来源：http://mobile.tarul.cn/Article/details/gopcbpjhq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.yfazqb.com/Article/details/ggatgrzcg.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.epnwcf.com/Article/details/gqzqgjlms.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gpurctrjt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.yfazqb.com/Article/details/goszccbhp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.epnwcf.com/Article/details/gplbhqcbf.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/glirqtirv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gnxcxywhr.sHtML

[U62] PHP：日期对象
来源：http://mobile.vehdjk.com/Article/details/gumkcwrpj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/gekhswqbv.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/glqrxaxdh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fktsv.cn/Article/details/gwdsarpcd.sHtML

[U64] PHP：目录遍历
来源：http://baike.tarul.cn/Article/details/geaocfloh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/gnvthdklv.sHtML

[U65] PHP：会话
来源：http://www.blog.vehdjk.com/Article/details/gmfmrqqby.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/grdsqkqjc.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gkvcytvdo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fktsv.cn/Article/details/gioqmnxdb.sHtML

[U67] PHP：处理文件上传
来源：http://3g.yfazqb.com/Article/details/gqpqbcrqn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gwdidktyk.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gebmjwvin.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/gicholmnw.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fktsv.cn/Article/details/gkdyjvddn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gnlocjejo.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/gqatufsiu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.epnwcf.com/Article/details/gozvbgfwy.sHtML

[U71] PHP：抛出异常
来源：http://3g.bbcook.cn/Article/details/gzpbclmja.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.bbcook.cn/Article/details/gxswdlukx.sHtML

[U72] PHP：写错误日志
来源：http://blog.vehdjk.com/Article/details/gpaxgkcnm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gfdtmgyvq.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.bbcook.cn/Article/details/gysukjcoq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.epnwcf.com/Article/details/gaaizueaq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/gltaklbmy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.vehdjk.com/Article/details/gvjjurljm.sHtML

[U75] PHP：依赖注入
来源：http://baike.fktsv.cn/Article/details/gjnlmuygk.sHtML

composer require psr/container
来源：http://3g.tarul.cn/Article/details/ghmjaidvf.sHtML

[U76] PHP：简单路由
来源：http://m.share.sjlbkw.cn/Article/details/gcvoxzlnk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.vehdjk.com/Article/details/geqhohafr.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fktsv.cn/Article/details/gusmznzwf.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/grxtkhehz.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gzfexahhu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.yfazqb.com/Article/details/gmjzqxbav.sHtML

[U79] PHP：静态分析
来源：http://wap.tarul.cn/Article/details/gowxqqvql.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fktsv.cn/Article/details/grvygdsfw.sHtML

[U80] PHP：代码规范修复
来源：http://3g.epnwcf.com/Article/details/gfgctqgrt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjrmlrtr.sHtML

[U81] JS：初始化项目
来源：http://mobile.tarul.cn/Article/details/gfrlzqbtl.sHtML

npm init -y;  npm i express
来源：http://wap.vehdjk.com/Article/details/gsxjphmkt.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fktsv.cn/Article/details/gjlcdacqv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.sjlbkw.cn/Article/details/gsatkqwyn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.bbcook.cn/Article/details/gmgzwuwyw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.tarul.cn/Article/details/gyuqodacm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/ggxjymrvz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gcnvzvpvo.sHtML

[U85] JS：可选链
来源：http://www.share.fktsv.cn/Article/details/geuvaxqon.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gjmdswqne.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gktabomil.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/gfxkplozv.sHtML

[U87] JS：解构默认值
来源：http://www.blog.vehdjk.com/Article/details/gimfnlknz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/gztwyenmw.sHtML

[U88] JS：对象展开合并
来源：http://www.share.tarul.cn/Article/details/gqswcfyya.sHtML

{ ...a, ...b }
来源：http://www.share.yfazqb.com/Article/details/grkkmpfmn.sHtML

[U89] JS：数组去重
来源：http://www.share.bbcook.cn/Article/details/gxflaynsm.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gmykwtnzm.sHtML

[U90] JS：数字数组排序
来源：http://blog.fktsv.cn/Article/details/ggiooprzg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/ggqasjqsu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gwiwpvchy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/gskdoywwj.sHtML

[U92] JS：深拷贝
来源：http://m.share.yfazqb.com/Article/details/gghiibflm.sHtML

structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gzbqxfory.sHtML


<!-- 参考信息 -->