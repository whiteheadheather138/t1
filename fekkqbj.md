代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/gkeruhhwx.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gijabzpzu.sHtML

[T04] Kotlin：空安全
来源：http://m.share.tarul.cn/Article/details/gsnmsfzxr.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gruvqkaan.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gawvobptp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/ghrzqbirf.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gfsbxypyg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.tarul.cn/Article/details/gkknitbyo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gboxopcfz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.yfazqb.com/Article/details/gvjhwaqas.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.epnwcf.com/Article/details/gcfchrtmz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.vehdjk.com/Article/details/galtmdcbi.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gnbkqusjq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/glqlwcecn.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/grkxtmlhm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/ggyogtjhu.sHtML

[T11] Kotlin：协程
来源：http://3g.vehdjk.com/Article/details/gaawcowws.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gdckkzisk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.tarul.cn/Article/details/goyzdabnl.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gjtmxebgu.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gldkszaur.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fktsv.cn/Article/details/gjzkzbgue.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fktsv.cn/Article/details/gqhuaxqpe.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gczskhplj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gpbzutovm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gtxulshix.sHtML

[T16] Swift：Hello World
来源：http://3g.fktsv.cn/Article/details/gohaxmjwy.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gthioniec.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gxbdjvawc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gefsruiwb.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gfmltugzx.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/ggmoyzddy.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/goplaxrdk.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gkuoilsuz.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gwngvdkuj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/gndkqchbw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/ghlxgpctw.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gpexsnvif.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gczvshinq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gxdejtmqh.sHtML

[T23] Swift：函数
来源：http://3g.epnwcf.com/Article/details/gbeeojzyo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgnckixd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gniqmynuv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.yfazqb.com/Article/details/gugeiabgc.sHtML

[T25] Swift：结构体
来源：http://wap.yfazqb.com/Article/details/gkevdwkjn.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/govbqfwrk.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gehbmxffz.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/ggejrrkla.sHtML

[T27] Swift：错误处理
来源：http://baike.tarul.cn/Article/details/ggblnpxwj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.yfazqb.com/Article/details/gkvgyerye.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gzkobfzmf.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/giuopajsp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/gzxdglyco.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/giawcvwfc.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gkzjyeodj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gelerqvsf.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gisspqblc.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gqxwlzrrc.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gmpokrghd.sHtML

local a = 1
来源：http://mobile.tarul.cn/Article/details/gafcozrsn.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gbhcntejk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.epnwcf.com/Article/details/gvcgxcnxa.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/gjqpbheam.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gebnctqnt.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gyveyonoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gfbgrauje.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/gassusptu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/gdrxggrqk.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gglvcbhaf.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/geihaungn.sHtML

[T38] Lua：条件
来源：http://wap.fktsv.cn/Article/details/grhvftlyn.sHtML

if x > 0 then print("正") end
来源：http://3g.vehdjk.com/Article/details/gjbaxjdcu.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/gzngmmunz.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gkhfwoykj.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gmmlgkrev.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.yfazqb.com/Article/details/geszazzjk.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/gvhhcoxhc.sHtML

print "Hello\n";
来源：http://mobile.vehdjk.com/Article/details/glpizjdug.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/gzxgfigtt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gifboowje.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/gibggdhuk.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/gobojophl.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gzwlkppce.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/grtbviljj.sHtML

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gqwfrilpo.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gxdndhwyn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gnecasjvb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.yfazqb.com/Article/details/gcpwrfnvo.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gqgpwajci.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/gpfqxgqju.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gdceepmcn.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gqttzjavj.sHtML

[T49] Perl：函数
来源：http://www.m.share.tarul.cn/Article/details/gftnlygkb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/ghsndubcr.sHtML

[T50] Perl：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gzoglvixk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqypkkfd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/ghegrddla.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/glayjphdp.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gijxnaudi.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gmvutgpsb.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gerofueas.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gixxppxmp.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/guliywkyb.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/goejxntvt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gfgojsfxq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gqlzpdozp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/gpwnjeeof.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/ggpgddqju.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.tarul.cn/Article/details/gfeziwqal.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/ggmvnsaww.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gjjmmowqu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.epnwcf.com/Article/details/gfrvlozct.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fktsv.cn/Article/details/gnplarlop.sHtML

[T59] Scala：循环
来源：http://www.m.share.fktsv.cn/Article/details/gwvqofcwn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gyoxxcjyp.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/gsantklfp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.sjlbkw.cn/Article/details/grodoetvw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvfrqluvq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gbgfsifsl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxigirzsu.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gwwekaqwd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/gzbkiuesg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.epnwcf.com/Article/details/goreoeuhn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gkrlnetun.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.sjlbkw.cn/Article/details/ggzrinnrg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gfuodfloi.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gcmbhwcvo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gtlzpkyfn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.vehdjk.com/Article/details/gfxifrlye.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/goaamhovj.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/ggbjcleug.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gjhtsctyj.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/gwdywciwz.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/grwistqdd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gowpizvdw.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gxvznximg.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gzgrazobz.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gcljozsuw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gjazcxjnv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.sjlbkw.cn/Article/details/gahitptkb.sHtML

[U11] Py：生成器表达式
来源：http://3g.yfazqb.com/Article/details/glbtsakvx.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gihebvquw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/gnslrcdxo.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gryhnkglt.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gomjatpwd.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/gysxmlncy.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.yfazqb.com/Article/details/gcfwzupvv.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/ghzceniuu.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/gkbutjwal.sHtML

t = time.perf_counter()
来源：http://mobile.fktsv.cn/Article/details/gonrjmcdz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.bbcook.cn/Article/details/gpownxfbd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.sjlbkw.cn/Article/details/gwzgqzuzd.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gnjjhjhdo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gkcxeimwt.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/ghuarriwg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gjfkzpdhk.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gamurykll.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.tarul.cn/Article/details/gmbhajtho.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gurqwnrpy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.bbcook.cn/Article/details/gsaixbloq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.tarul.cn/Article/details/gpwwtrzjc.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gwmmnyunw.sHtML

[U22] Py：矩阵转置
来源：http://3g.tarul.cn/Article/details/ganiwkxqq.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/guhnkehuj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.epnwcf.com/Article/details/gaajbzeqd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.yfazqb.com/Article/details/giddvgpzn.sHtML

[U24] Py：路径操作
来源：http://www.blog.bbcook.cn/Article/details/gmdivbhvn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gpeozwxnk.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/glummowan.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gnwzgjyae.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/grnaoayye.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.bbcook.cn/Article/details/gojeykkrl.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gvzguzozo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/gtrivafqu.sHtML

[U28] Py：类型别名
来源：http://www.blog.yfazqb.com/Article/details/gmknufrig.sHtML

UserId = int
来源：http://read.share.fktsv.cn/Article/details/glqdqmpvd.sHtML

[U29] Py：属性校验
来源：http://www.blog.yfazqb.com/Article/details/gmmrvfgci.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/gzurjlbez.sHtML

[U30] Py：数据类
来源：http://baike.bbcook.cn/Article/details/gscpphadz.sHtML

@dataclass(slots=True)
来源：http://baike.epnwcf.com/Article/details/gcasaxtjd.sHtML

[U31] Py：单测
来源：http://wap.epnwcf.com/Article/details/gsntbwlay.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/ghpugsyvo.sHtML

[U32] Py：代码格式化
来源：http://www.share.yfazqb.com/Article/details/gndouzaml.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.vehdjk.com/Article/details/gybuhxjkr.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/gyhfqeujw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gxdklkzcg.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/gdoajsvoe.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gimerwzoz.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/gyvmwjxkf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gzrdjxbll.sHtML

[U36] Py：定时任务
来源：http://baike.yfazqb.com/Article/details/gtdpcwzpt.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gnoxzmkem.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fktsv.cn/Article/details/gpfqhszab.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/gyookzxgq.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.epnwcf.com/Article/details/gxwnbapnz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/gtaxxlrgj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/glivlbpux.sHtML

sys.stdout.isatty()
来源：http://www.m.share.tarul.cn/Article/details/gprhdoxep.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/grxrikiyy.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/ggtxvyntk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/gqscrbsbu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwxysmcq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fktsv.cn/Article/details/gfdtefvst.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.vehdjk.com/Article/details/gtjmeyhwm.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.bbcook.cn/Article/details/gdffjacss.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/guhgojlip.sHtML

[U44] PHP：开启严格类型
来源：http://baike.epnwcf.com/Article/details/gyihynkxl.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gagybghgt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.yfazqb.com/Article/details/goxsgnpem.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gatsmmhbg.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gzjfodcjz.sHtML

?string $name = null
来源：http://baike.vehdjk.com/Article/details/gmassjjxy.sHtML

[U47] PHP：联合类型
来源：http://3g.bbcook.cn/Article/details/gbmxfoahd.sHtML

int|string $id
来源：http://baike.bbcook.cn/Article/details/gibrwjggp.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.bbcook.cn/Article/details/gqpjbzhnk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.epnwcf.com/Article/details/giibzlhpl.sHtML

[U49] PHP：只读属性
来源：http://m.share.tarul.cn/Article/details/gvrhshfqf.sHtML

public readonly string $name
来源：http://m.share.sjlbkw.cn/Article/details/gqqjiffcq.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/gzvblrhhe.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/gcooiuwja.sHtML

[U51] PHP：数组解构
来源：http://3g.sjlbkw.cn/Article/details/ggiiqygvw.sHtML

[$a, $b] = $arr;
来源：http://www.blog.sjlbkw.cn/Article/details/gnnuiflox.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/glnnycxje.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gxvmnorno.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.epnwcf.com/Article/details/gvqfzzpls.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gqrmdmity.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gyfnbuhyr.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gwennjwba.sHtML

[U55] PHP：match 表达式
来源：http://www.share.vehdjk.com/Article/details/gldgsroqw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.epnwcf.com/Article/details/gxgipzuji.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gjichfghf.sHtML

f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gzqvzbkvn.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/geduigpqq.sHtML

"值: {$a}"
来源：http://read.share.yfazqb.com/Article/details/gbfpmeenf.sHtML

[U58] PHP：数组三件套
来源：http://wap.vehdjk.com/Article/details/gcqbfflmm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/gaxwtrgxn.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/girfogqzr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gbpkhjhci.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.tarul.cn/Article/details/gpofxdglo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.vehdjk.com/Article/details/guelmtadv.sHtML

[U61] PHP：正则
来源：http://wap.yfazqb.com/Article/details/glxfgapgs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gfzuyumeb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.vehdjk.com/Article/details/gvkgaragz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.tarul.cn/Article/details/gsyimujvc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/gjmvcjwry.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.epnwcf.com/Article/details/gwcwxview.sHtML

[U64] PHP：目录遍历
来源：http://3g.bbcook.cn/Article/details/gaqjzkqza.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.epnwcf.com/Article/details/gdwrultgi.sHtML

[U65] PHP：会话
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkhyrlvz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/glaigdhjq.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.bbcook.cn/Article/details/gehxckfay.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/ghixqopnr.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/ghftzzdlv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fktsv.cn/Article/details/gjulptaez.sHtML

[U68] PHP：PDO 连接
来源：http://wap.vehdjk.com/Article/details/gcvtdhbda.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.yfazqb.com/Article/details/gznimmcyi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.epnwcf.com/Article/details/gtgdosqee.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fktsv.cn/Article/details/gvsaiirws.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/gzozqgkng.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.sjlbkw.cn/Article/details/gtughuxxb.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gvisinyym.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.bbcook.cn/Article/details/gooxtrrjo.sHtML

[U72] PHP：写错误日志
来源：http://3g.tarul.cn/Article/details/gfbchhdqh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gjssbbhtq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/gcbilyrfd.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fktsv.cn/Article/details/gleskzzxf.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/gfrafegou.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.bbcook.cn/Article/details/geoubnkph.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/gwtgizixe.sHtML

composer require psr/container
来源：http://m.share.epnwcf.com/Article/details/gccanfupr.sHtML

[U76] PHP：简单路由
来源：http://baike.fktsv.cn/Article/details/gyfkcfcxx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.bbcook.cn/Article/details/gflovsnga.sHtML

[U77] PHP：模板渲染
来源：http://3g.epnwcf.com/Article/details/gkrkdtchb.sHtML

composer require twig/twig
来源：http://www.m.share.vehdjk.com/Article/details/gnopfjvvf.sHtML

[U78] PHP：单元测试
来源：http://read.share.yfazqb.com/Article/details/gxdihehap.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.bbcook.cn/Article/details/gokrxlwsy.sHtML

[U79] PHP：静态分析
来源：http://3g.bbcook.cn/Article/details/gzouglzdt.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fktsv.cn/Article/details/gbtjiftgs.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fktsv.cn/Article/details/gteouvgjy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.tarul.cn/Article/details/gmyooiwzo.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gnnzfbleg.sHtML

npm init -y;  npm i express
来源：http://www.share.fktsv.cn/Article/details/gwyqnuouh.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gxvczqyfu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/gscslsnri.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fktsv.cn/Article/details/gxgtmzfqi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gqbqffdui.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.tarul.cn/Article/details/gortwdalq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.yfazqb.com/Article/details/gbvqqgage.sHtML

[U85] JS：可选链
来源：http://wap.yfazqb.com/Article/details/gfuyabqrk.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/gihbvzqbm.sHtML

[U86] JS：空值合并
来源：http://www.share.epnwcf.com/Article/details/grvrtnenb.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/ggxwjhzcn.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/gjwitxytn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fktsv.cn/Article/details/gjmktnxxu.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gjefenttf.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/gpcbpgkcs.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/grhetbvfe.sHtML

[...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gmiwoeldd.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fktsv.cn/Article/details/gqfkpwmxf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gszeycile.sHtML


<!-- 参考信息 -->