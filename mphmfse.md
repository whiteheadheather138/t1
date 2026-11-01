代发 wailian999

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gkuvesdqt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gfdjwxttm.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/ghgcuyilu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.vehdjk.com/Article/details/godaxjrwe.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gizsjamrf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gsowbcrxl.sHtML

[T08] Kotlin：数据类
来源：http://3g.sjlbkw.cn/Article/details/gptqwayyd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/godqcmptk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gnqigrbnp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gbwkploxa.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/gzwakihhv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gzccxjucy.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/gokpbhxrq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gfejixdoe.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gcckfpiom.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gjppwmoku.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gvrvpobyi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/ghovlrzyy.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gyseydjuk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gtrljutin.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/gpwdkjxlf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gqosfdotp.sHtML

[T16] Swift：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gvppdjnsy.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gqogagwgi.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gtfikotqi.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/gvahlzzkm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gggzfllgv.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/giasqpknj.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gfobrcdbv.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/gifewgxro.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gojtdcdzp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gtkfboqrl.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/govcjifbn.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/gfjtbjivg.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/gsfjqbkkv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/geohhcvva.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/gzxfwmqec.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/gtekjexyt.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/ghccgpjvh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gofftxklq.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gcvjnnkjv.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gtrfmqvsh.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/ggjnyixpw.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gokemlzvm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/goltfjnaa.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gksrgfwmz.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gjxwtqqji.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gphujsglh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.yfazqb.com/Article/details/gswpiegfs.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/gdhhjynya.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/gwljdepgf.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gebrldfce.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gzggyojvy.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gcanfiwku.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gbijueyeo.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gyvqocnie.sHtML

[T33] Lua：表（数组）
来源：http://www.share.sjlbkw.cn/Article/details/gycaikwaf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gogvlmvqi.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/gbalixbhm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/gnsaqjani.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gjcikubqo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/ghwjotnrf.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gdtytjwzl.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/gnwujwzrq.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/goiwrywhn.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gikwvhrls.sHtML

[T38] Lua：条件
来源：http://mobile.yfazqb.com/Article/details/gfxxjixhp.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/glxutejbs.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gfmwktaad.sHtML

string.find(s, "%d+")
来源：http://m.share.sjlbkw.cn/Article/details/gvahkfzgk.sHtML

[T40] Lua：元表
来源：http://3g.epnwcf.com/Article/details/gtfzfwvel.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gwfvzybpg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/guhdeqwyq.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gwehvwdcz.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gsakquynt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fktsv.cn/Article/details/geqrqbkla.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/gtnhorcro.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gpzgdkimz.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/gxwjkdkvp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.yfazqb.com/Article/details/gufsrcfft.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gtrxjuhsr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.sjlbkw.cn/Article/details/gvuikxxfr.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gjzoilfiv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gmkmfsjcb.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gqfvjfrdu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/girwfsbin.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/gydgyjxgq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.sjlbkw.cn/Article/details/gyilfhvtm.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/gltyqvlxd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gsyvakxwr.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gqsgnueqn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/gcfokpupj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.yfazqb.com/Article/details/gfzsmzmit.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gpyvhvequ.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gpzuasybp.sHtML

[T52] Scala：变量
来源：http://mobile.sjlbkw.cn/Article/details/gfnuqfrcu.sHtML

val a = 1;  var b = 2
来源：http://baike.fktsv.cn/Article/details/gnheijbum.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gmterpzan.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/ggltwhjpd.sHtML

[T54] Scala：集合映射
来源：http://wap.yfazqb.com/Article/details/gurzgwnkg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gmqqwmmfz.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/grspybxmw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/gqbkorwxr.sHtML

[T56] Scala：样例类
来源：http://www.blog.vehdjk.com/Article/details/gbxpjibrs.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/gecntzepi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gcajxjojd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gqfueqzik.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gfdfqzjyw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fktsv.cn/Article/details/gvprciyle.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/grzyxlqrw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzwamgbo.sHtML

[T60] Scala：折叠
来源：http://www.share.bbcook.cn/Article/details/gbhieuhrq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/gyfvavhuy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfzfbjlbj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gzekuijbk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpmsfcbjf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.bbcook.cn/Article/details/gyjjyjdci.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.yfazqb.com/Article/details/gbjdxndqu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.bbcook.cn/Article/details/gsmkkbsyy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.tarul.cn/Article/details/grdffzohu.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gizdbpvyt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuggyjhh.sHtML

[U04] Py：变量调试打印
来源：http://blog.bbcook.cn/Article/details/gmrwjlvzx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fktsv.cn/Article/details/gsquqgsfv.sHtML

[U05] Py：列表去重且保序
来源：http://wap.bbcook.cn/Article/details/gdanghmps.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gokabnulq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fktsv.cn/Article/details/giqraaaxc.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gxhlmdwst.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gtvryauum.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/gcuuabecr.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/gokrqxejc.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gnstmrsig.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.yfazqb.com/Article/details/gotfvjeoi.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/grstfdqun.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/gurpimnwe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gnovoplva.sHtML

[U11] Py：生成器表达式
来源：http://mobile.yfazqb.com/Article/details/gptvhjzlj.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gjegnmbqh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/grzpoconc.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/gjrbclwqj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.bbcook.cn/Article/details/gjrjuaxod.sHtML

deque(maxlen=10)
来源：http://wap.fktsv.cn/Article/details/gjlpbtwno.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/gvlijeosg.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/gxamlywao.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/gldgypmod.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gbtzzkhog.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.sjlbkw.cn/Article/details/gytrppbat.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gwqmfvbbn.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/grmviqbdu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gafvxiqdl.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/gyjyfafrh.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gsbeenmzv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.bbcook.cn/Article/details/gqqwnploc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gksigkzgt.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.vehdjk.com/Article/details/gbezgqylt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.vehdjk.com/Article/details/gsirpjiuy.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/gtqkukrfi.sHtML

@contextlib.contextmanager
来源：http://www.blog.epnwcf.com/Article/details/gygfbkwuc.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gbahuxvtf.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gbtxsajos.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/goizjzoiz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fktsv.cn/Article/details/gyqpssrdo.sHtML

[U24] Py：路径操作
来源：http://mobile.bbcook.cn/Article/details/ggaoarwha.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gnnbsnete.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fktsv.cn/Article/details/gnqaeolay.sHtML

csv.DictReader(f)
来源：http://blog.tarul.cn/Article/details/gotoedcru.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gvptqvxlw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.vehdjk.com/Article/details/gmvrmkaxp.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fktsv.cn/Article/details/gwzrblywy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/gqarnoebp.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gevhqdvjl.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/gijiztcum.sHtML

[U29] Py：属性校验
来源：http://mobile.yfazqb.com/Article/details/gxvlkxoyw.sHtML

@property 与 @x.setter 配合
来源：http://wap.bbcook.cn/Article/details/gpadlvzvu.sHtML

[U30] Py：数据类
来源：http://mobile.fktsv.cn/Article/details/gkagokkza.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gtfbcygnj.sHtML

[U31] Py：单测
来源：http://wap.bbcook.cn/Article/details/ghcscynwq.sHtML

python -m pytest -q
来源：http://blog.tarul.cn/Article/details/gmcyfkvob.sHtML

[U32] Py：代码格式化
来源：http://read.share.tarul.cn/Article/details/gyhqltbqm.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/gwkovnvgu.sHtML

[U33] Py：打包发布
来源：http://m.share.bbcook.cn/Article/details/gpnzjlqqk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.vehdjk.com/Article/details/gxttchwax.sHtML

[U34] Py：判断编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdvaaxek.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gihnyfdtf.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gxczugsmi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fktsv.cn/Article/details/gkmtdlzke.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gaarsgtpi.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fktsv.cn/Article/details/gkywgipdh.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gutghjjmb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.tarul.cn/Article/details/gvyovyurp.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fktsv.cn/Article/details/gsrpzcgpe.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gctfggtjr.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.tarul.cn/Article/details/goyymlccm.sHtML

sys.stdout.isatty()
来源：http://blog.yfazqb.com/Article/details/gcnvikagw.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gfodscayr.sHtML

print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gunpxcmde.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.bbcook.cn/Article/details/grmrhiwga.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/gzvejxoxn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gufmhrjbm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/ghzhdgqyg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.tarul.cn/Article/details/gcncpwosa.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gxkysjcvg.sHtML

[U44] PHP：开启严格类型
来源：http://wap.tarul.cn/Article/details/gdniqnwrx.sHtML

declare(strict_types=1);
来源：http://blog.sjlbkw.cn/Article/details/gkckpmsts.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/gunthnzin.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/guirxaeum.sHtML

[U46] PHP：可空类型
来源：http://wap.epnwcf.com/Article/details/gwbprhdac.sHtML

?string $name = null
来源：http://3g.bbcook.cn/Article/details/gascvjhrk.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/gkfboparg.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/gsrtlrgku.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gxpufszza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gksxeorhn.sHtML

[U49] PHP：只读属性
来源：http://3g.fktsv.cn/Article/details/ghkslqgpf.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/godzvdlkv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.bbcook.cn/Article/details/gifrrmvvz.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/gyckklhpm.sHtML

[U51] PHP：数组解构
来源：http://blog.yfazqb.com/Article/details/gdfjugvto.sHtML

[$a, $b] = $arr;
来源：http://mobile.yfazqb.com/Article/details/gpxonmffw.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gvjrrhobi.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gxmuoijya.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/glvmfcmjk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.epnwcf.com/Article/details/gtetkuzrw.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/guietudzw.sHtML

$obj?->method()
来源：http://mobile.yfazqb.com/Article/details/gkdtycobj.sHtML

[U55] PHP：match 表达式
来源：http://m.share.sjlbkw.cn/Article/details/ggwbvxidh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/gjgmhteyc.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gmvdvqkws.sHtML

f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gofmlekud.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/guygjwwcx.sHtML

"值: {$a}"
来源：http://3g.vehdjk.com/Article/details/ggstmkqll.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gccrriveh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.bbcook.cn/Article/details/gsmkgkjsf.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gwlyvlyxw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/grnyiqmhr.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gwytepazj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gyqcxidht.sHtML

[U61] PHP：正则
来源：http://wap.sjlbkw.cn/Article/details/gbilnczhy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gfdcjbgrh.sHtML

[U62] PHP：日期对象
来源：http://blog.epnwcf.com/Article/details/gsplpokjg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.vehdjk.com/Article/details/geqmtjxcl.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gpwrcjbve.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fktsv.cn/Article/details/goovalfwx.sHtML

[U64] PHP：目录遍历
来源：http://www.share.tarul.cn/Article/details/gzyzwkadh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.epnwcf.com/Article/details/gcvoeptzr.sHtML

[U65] PHP：会话
来源：http://www.m.share.yfazqb.com/Article/details/glaqjsfkm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gcizbtnwm.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/groccdixt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gxdlpihyc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/gefdzugts.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.vehdjk.com/Article/details/ggtfrwkvr.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fktsv.cn/Article/details/gbdwyksft.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/gqfvajngs.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/ggyqfipfs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.bbcook.cn/Article/details/guyojqpef.sHtML

[U70] PHP：PDO 事务
来源：http://blog.sjlbkw.cn/Article/details/grietnapr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gfxhjsjnp.sHtML

[U71] PHP：抛出异常
来源：http://3g.tarul.cn/Article/details/gytbncnot.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gdumtxqap.sHtML

[U72] PHP：写错误日志
来源：http://wap.vehdjk.com/Article/details/ghhgacqkx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.epnwcf.com/Article/details/gpjzbsnqb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.epnwcf.com/Article/details/gioujyips.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.tarul.cn/Article/details/gvogjssuw.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gexexbrea.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gktlyolxk.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fktsv.cn/Article/details/gjdfmybea.sHtML

composer require psr/container
来源：http://m.share.epnwcf.com/Article/details/gtsrhgowl.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/gqxwqldeh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/gdyjqkhnu.sHtML

[U77] PHP：模板渲染
来源：http://baike.epnwcf.com/Article/details/gikhfgnxh.sHtML

composer require twig/twig
来源：http://www.blog.tarul.cn/Article/details/grapuofgn.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gjwwhkvwt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/gsmxvvxom.sHtML

[U79] PHP：静态分析
来源：http://m.share.bbcook.cn/Article/details/geicjgbgo.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.sjlbkw.cn/Article/details/gsyeqhuio.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/gbqnpvtjj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/gyuvmbmiz.sHtML

[U81] JS：初始化项目
来源：http://wap.epnwcf.com/Article/details/gtmuqawsb.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gsnetuddf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gwxgxtoka.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.vehdjk.com/Article/details/glmmsdhtc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.sjlbkw.cn/Article/details/guvcrkpxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gfslzmwbk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.epnwcf.com/Article/details/gtubnuvdt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.epnwcf.com/Article/details/gmuienltr.sHtML

[U85] JS：可选链
来源：http://baike.yfazqb.com/Article/details/goymqdazh.sHtML

a?.b?.c
来源：http://blog.epnwcf.com/Article/details/ggdisqgho.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/gjiftmqoq.sHtML

a ?? b
来源：http://blog.sjlbkw.cn/Article/details/giilserrm.sHtML

[U87] JS：解构默认值
来源：http://3g.yfazqb.com/Article/details/gqngfoxit.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gtaumuzce.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.yfazqb.com/Article/details/glokyuspm.sHtML

{ ...a, ...b }
来源：http://mobile.bbcook.cn/Article/details/gcynazpho.sHtML

[U89] JS：数组去重
来源：http://www.blog.sjlbkw.cn/Article/details/gwluskldr.sHtML

[...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gidspjbda.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gnrepwkxc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gdhambxpr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.bbcook.cn/Article/details/gdwagnfll.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gjnexjebr.sHtML

[U92] JS：深拷贝
来源：http://mobile.epnwcf.com/Article/details/glaxnnekd.sHtML

structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gtcvtrfju.sHtML


<!-- 参考信息 -->