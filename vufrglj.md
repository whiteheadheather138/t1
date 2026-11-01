代发 wailian999

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gyoqvcmpn.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gikzctswk.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/gnjsiohmf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gbuwynvki.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/gbqriowcg.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gignqwubr.sHtML

[T04] Kotlin：空安全
来源：http://blog.fktsv.cn/Article/details/gkwynyvsd.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gurmkwnrg.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gikrbidpo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/gpyyqwubg.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gvmuggwop.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gmyrtrdxk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gzkdhldmy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gtcbhppom.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/grzlxbdgi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/giloryhht.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gbvcfmjag.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.bbcook.cn/Article/details/guxqecnrz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.epnwcf.com/Article/details/goyayhnjf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gwgiveaad.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/ghuwogpst.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/grbcpgfne.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gtqpmltta.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gbmoyomua.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/grgvlhkax.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/grdznncbp.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/ggdxxbbvx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gnmfiepfj.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gcvdvyyil.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gqctxolzn.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gatwdflit.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gcbmqwuex.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gvllanzhp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gyecxbvov.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gpwasrbwi.sHtML

"值: \(b)"
来源：http://3g.tarul.cn/Article/details/gbjsjrkud.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gsehsxrhg.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/ghyilpshh.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gjvqsmldq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gqrqbecgr.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/goifwossl.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/gmvpfjvod.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/glavkzjem.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gaerpdokw.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/ghaohfidt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.epnwcf.com/Article/details/gpnonbmdi.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/geazxibyg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gmepdnhqy.sHtML

[T25] Swift：结构体
来源：http://3g.epnwcf.com/Article/details/gavdfgzzw.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gyykshccq.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gnyhbjttr.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/gybciekmv.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/geqzgvili.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/gvhnbehfp.sHtML

[T28] Swift：枚举
来源：http://www.share.fktsv.cn/Article/details/gbvevtepu.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/gipsprwhs.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.epnwcf.com/Article/details/gaebcgrvl.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/ggaabyklf.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gffoplyjs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/gysfruifv.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gowhetjip.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/grjqqjvdv.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gedgwdole.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/gmphbotqg.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gklbgskrx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/gjxtlmbag.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.vehdjk.com/Article/details/gfvcwtclj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/giwavhgzl.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/gucbinkzv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/ghpxmxpsx.sHtML

[T36] Lua：函数
来源：http://3g.bbcook.cn/Article/details/ggekvtbfg.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gsvraxgnh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/ggbjyfpqk.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/gxynkuscc.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/gzftqdsml.sHtML

if x > 0 then print("正") end
来源：http://www.blog.tarul.cn/Article/details/gsfimwfvd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gvojoezww.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gqbiomdfj.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gyquirxap.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gspbyqpvk.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/guimmkbsf.sHtML

print "Hello\n";
来源：http://www.share.fktsv.cn/Article/details/gypwmxxmh.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/ghzfldcnx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.epnwcf.com/Article/details/gwnwikhpa.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/ggxpehzew.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/gxrgnnixa.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/gzljjtvsh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gwdmziawv.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gszkzjhcb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/gyisorhxd.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/ghmcokjxp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gopoikcjq.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.sjlbkw.cn/Article/details/gkfvyxgwl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/gwpzshngs.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gwmmnensf.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gglmoudhi.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gtuciyfuz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gmuuqnirw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gjoyhosmr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/gukkxxeto.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/gvktkgpxr.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gfcxephei.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gdxdswbdn.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gvjyarlha.sHtML

val a = 1;  var b = 2
来源：http://wap.fktsv.cn/Article/details/guykelhmd.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/goekiandt.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/gkwfwzlhz.sHtML

[T54] Scala：集合映射
来源：http://3g.bbcook.cn/Article/details/grdslukdw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.tarul.cn/Article/details/ggatfpeot.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gpjgapakh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/gshugexfd.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gxmsahtkg.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gnfrqppew.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gdvmwpzoz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gihfegjwj.sHtML

[T58] Scala：函数定义
来源：http://m.share.tarul.cn/Article/details/ggcuxwyca.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/ggtlsvxyi.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gwvygafmj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.vehdjk.com/Article/details/gboqduzpk.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gxnnkhapq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gwwezuhfd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzjfptjyt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/ghughddip.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzddqzmcv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/glbcnhujc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gkejboohm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.epnwcf.com/Article/details/gatmnowpa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gnecrqfou.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gbyhznago.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gpzlwchcr.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gfxkrzeev.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gayrwzizz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gjkxsbwiq.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gupydwmho.sHtML

[U06] Py：合并两个字典
来源：http://www.share.sjlbkw.cn/Article/details/gerrvukqb.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/giuklbpcx.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gmzxayhym.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gbgunzvcp.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gttxmqpgj.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gybgpjdnj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/gzjunlfcd.sHtML

max(d, key=d.get)
来源：http://wap.bbcook.cn/Article/details/ggeuxwdqb.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/gkkaizcfg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.epnwcf.com/Article/details/grjeizyas.sHtML

[U11] Py：生成器表达式
来源：http://m.share.epnwcf.com/Article/details/gttpppiwf.sHtML

(x * 2 for x in arr)
来源：http://m.share.sjlbkw.cn/Article/details/gjhpsvbtk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gtjzsblpf.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/gjizkryoy.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/givxxpswo.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/gjihlkgxt.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gflvqvpmv.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gfwolrkge.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gfpntedzg.sHtML

t = time.perf_counter()
来源：http://m.share.tarul.cn/Article/details/gssovidtq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.epnwcf.com/Article/details/gzuwmhhnd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gyokuizsk.sHtML

[U17] Py：初始化日志
来源：http://blog.vehdjk.com/Article/details/gszmcfrbd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gpkxxjclx.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gwjapksrd.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.bbcook.cn/Article/details/gjloisyrd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/gksgeskqe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gbgtzquer.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/getkfouti.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.vehdjk.com/Article/details/gvnafelsh.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.epnwcf.com/Article/details/gniejdtbu.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gzitwccie.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.bbcook.cn/Article/details/gygdbdlss.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/gpetaczgb.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gbhanjaxv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.vehdjk.com/Article/details/groxazmfy.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gniywahzq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gaysyoduy.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gvpkhrzfr.sHtML

csv.DictReader(f)
来源：http://mobile.yfazqb.com/Article/details/gmrdihrxp.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/getkktvpq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/gkyeoquwq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.sjlbkw.cn/Article/details/gazxxqjce.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/gcootcows.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gzkghjguh.sHtML

UserId = int
来源：http://www.blog.sjlbkw.cn/Article/details/guuhxxyja.sHtML

[U29] Py：属性校验
来源：http://3g.tarul.cn/Article/details/gsepyubdc.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/gtgfbzrjj.sHtML

[U30] Py：数据类
来源：http://www.blog.bbcook.cn/Article/details/gllpshdsm.sHtML

@dataclass(slots=True)
来源：http://www.m.share.yfazqb.com/Article/details/gtjitwbzv.sHtML

[U31] Py：单测
来源：http://read.share.fktsv.cn/Article/details/gyzjxfhzu.sHtML

python -m pytest -q
来源：http://wap.fktsv.cn/Article/details/gpzyrklin.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/gwirzmlrz.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gtxzzgfyp.sHtML

[U33] Py：打包发布
来源：http://blog.fktsv.cn/Article/details/gxlujlyff.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.vehdjk.com/Article/details/gplnumnbq.sHtML

[U34] Py：判断编码
来源：http://read.share.fktsv.cn/Article/details/gywoahzph.sHtML

chardet.detect(raw)
来源：http://baike.yfazqb.com/Article/details/gpoevlfls.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fktsv.cn/Article/details/gvwaxypoc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gdujltuuq.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gcwzqkzke.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.epnwcf.com/Article/details/gmuwgqrde.sHtML

[U37] Py：读写 Excel
来源：http://www.share.sjlbkw.cn/Article/details/gnopgusof.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/gwcirgkwg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.vehdjk.com/Article/details/gxjourseh.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gsrewikmk.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/gtlfbceud.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/gmgufqyga.sHtML

[U40] Py：打印到标准错误
来源：http://wap.sjlbkw.cn/Article/details/gbiztscwc.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gsjbbgdzu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fktsv.cn/Article/details/gwnoxrksi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.vehdjk.com/Article/details/gfpajpmpd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gekjlbdfc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.bbcook.cn/Article/details/gsdjtlhlf.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fktsv.cn/Article/details/gcpzixmhu.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gizplelgu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gxcalvylc.sHtML

declare(strict_types=1);
来源：http://3g.epnwcf.com/Article/details/grpclibqe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/gjknfhwgp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gwkaizjrl.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/gsswcuuhm.sHtML

?string $name = null
来源：http://www.m.share.fktsv.cn/Article/details/grsdstkju.sHtML

[U47] PHP：联合类型
来源：http://baike.epnwcf.com/Article/details/gdenrlawx.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gbuhlhsbx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.yfazqb.com/Article/details/gnmnhebxj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.sjlbkw.cn/Article/details/gorgyigca.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.tarul.cn/Article/details/gusyxogir.sHtML

public readonly string $name
来源：http://www.share.vehdjk.com/Article/details/gtozpvhkt.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gptferyyy.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/gorquxhix.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gkdtvlhdb.sHtML

[$a, $b] = $arr;
来源：http://m.share.sjlbkw.cn/Article/details/gpbbfgyfg.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gervbeofl.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.tarul.cn/Article/details/gkjwvggwp.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.sjlbkw.cn/Article/details/gpxnspoja.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.epnwcf.com/Article/details/gmtmdetjy.sHtML

[U54] PHP：空安全调用
来源：http://3g.sjlbkw.cn/Article/details/grfwgbgki.sHtML

$obj?->method()
来源：http://www.m.share.bbcook.cn/Article/details/gevkzrgkj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/ggtswewre.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/ghwabakfl.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/guuamyade.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gqgvtcirx.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/giaadsuwd.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gluybvqiq.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/guwajzdwh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.vehdjk.com/Article/details/gbjylnzhv.sHtML

[U59] PHP：自定义排序
来源：http://3g.vehdjk.com/Article/details/ghnejhuie.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/guvgnneea.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.tarul.cn/Article/details/gvqjmvwqn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/goddtwqsc.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/gnzhccexy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gxaibzdpb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.epnwcf.com/Article/details/gqkhfjpxd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/gcyjenyzx.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/gayqsexyb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fktsv.cn/Article/details/gwqoeklig.sHtML

[U64] PHP：目录遍历
来源：http://www.share.epnwcf.com/Article/details/gsvaurhib.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.bbcook.cn/Article/details/gvfprfkhk.sHtML

[U65] PHP：会话
来源：http://www.share.sjlbkw.cn/Article/details/gawkvcwip.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/gnncwbctt.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.yfazqb.com/Article/details/gpkthhclo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.yfazqb.com/Article/details/gqswdpzeg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/gypktpszr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.sjlbkw.cn/Article/details/gzdcstdgh.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.sjlbkw.cn/Article/details/gsmdsbdsm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.tarul.cn/Article/details/gajifblpi.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/gyfjmhwig.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.vehdjk.com/Article/details/gpomespre.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrgmfsud.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fktsv.cn/Article/details/gestuwdmw.sHtML

[U71] PHP：抛出异常
来源：http://3g.tarul.cn/Article/details/gnefayjpd.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/glcckarty.sHtML

[U72] PHP：写错误日志
来源：http://3g.epnwcf.com/Article/details/grygnpycc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.bbcook.cn/Article/details/gofpodyop.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.sjlbkw.cn/Article/details/gahncuewr.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/gsvtyplzz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gwuhhnpyu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fktsv.cn/Article/details/gxnhiphki.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gujhjvzad.sHtML

composer require psr/container
来源：http://m.share.epnwcf.com/Article/details/gfahoyjce.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.sjlbkw.cn/Article/details/guizmsuce.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/gcgrbdxtt.sHtML

[U77] PHP：模板渲染
来源：http://www.share.vehdjk.com/Article/details/gkfgakbpb.sHtML

composer require twig/twig
来源：http://blog.tarul.cn/Article/details/gegqpsemm.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/grxzsvqlf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fktsv.cn/Article/details/gtrhwwnrf.sHtML

[U79] PHP：静态分析
来源：http://3g.bbcook.cn/Article/details/gqlgbemtf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.tarul.cn/Article/details/gaddwhotj.sHtML

[U80] PHP：代码规范修复
来源：http://3g.yfazqb.com/Article/details/gzcvyrxuc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.yfazqb.com/Article/details/gyzthofpi.sHtML

[U81] JS：初始化项目
来源：http://baike.yfazqb.com/Article/details/gtjdtbxho.sHtML

npm init -y;  npm i express
来源：http://www.m.share.bbcook.cn/Article/details/gmhdecmqm.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gofwnmzxm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.vehdjk.com/Article/details/gproonuus.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gmkaejzap.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gmypubpqi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.vehdjk.com/Article/details/gqxxfyifl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/gmbuwnflw.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gdffiqdpe.sHtML

a?.b?.c
来源：http://3g.sjlbkw.cn/Article/details/gjddwxbyr.sHtML

[U86] JS：空值合并
来源：http://3g.vehdjk.com/Article/details/gfkldijbp.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gjcpisles.sHtML

[U87] JS：解构默认值
来源：http://wap.fktsv.cn/Article/details/gtbkqarmt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fktsv.cn/Article/details/gtcplqlxk.sHtML

[U88] JS：对象展开合并
来源：http://blog.epnwcf.com/Article/details/gelcbvihh.sHtML

{ ...a, ...b }
来源：http://www.share.bbcook.cn/Article/details/getsvybkw.sHtML


<!-- 参考信息 -->