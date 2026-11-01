代发 wailian999

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gugfljlag.sHtML

"值: $b"
来源：http://blog.bbcook.cn/Article/details/gxivoabvm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/glvohtorg.sHtML

val n: String? = null;  n?.length
来源：http://blog.yfazqb.com/Article/details/gmodzvfba.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/gqxeuapva.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gumvyywgh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.epnwcf.com/Article/details/gvpebvkxt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/gxffcrlnz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/grmxvmyqb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gvnbnpevh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/gdnicupbw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gnuqxpweh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gqnavzzzk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/gvpxajlih.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/guxfcrnpz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gwlxxnzdp.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gtypzjopu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/gwbwdozhq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gniarazji.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gtayjhbbs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.yfazqb.com/Article/details/gvoowvnqt.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gydzpklut.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/gqlzolsjq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gtmbckzsh.sHtML

[T15] Kotlin：接口
来源：http://mobile.bbcook.cn/Article/details/gawvkmfyv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gczmklygn.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gyylkeybc.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gdyfkhoec.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gugdnxcbk.sHtML

var a = 1;  let b = 2
来源：http://read.share.tarul.cn/Article/details/guytbnwsv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/guhiurccy.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gnuzsofna.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gcycotdkb.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gnikicmus.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/gebfnltwy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gdtlgcejz.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/ggptbpgwu.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/ghmbxoaoq.sHtML

[T22] Swift：字典
来源：http://www.blog.vehdjk.com/Article/details/gywexydyi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gfcumwkqs.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/gdtxtfahp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/guhgopcoz.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gcoetvjqn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gfvocltad.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gnslxlvbv.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/gfbucyuiw.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gukuoqppz.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gphmbuukt.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gaamhxocm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.epnwcf.com/Article/details/gvhhutllh.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gmmofstqq.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/grgedgvqi.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/ganrnofae.sHtML

guard let x = opt else { return }
来源：http://m.share.vehdjk.com/Article/details/gbanffrts.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gzszketqm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gvaqdniub.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gzedbycql.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gjguyngct.sHtML

[T32] Lua：局部变量
来源：http://www.blog.tarul.cn/Article/details/ghhirnaiv.sHtML

local a = 1
来源：http://m.share.tarul.cn/Article/details/glvnsbnye.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gntnuypko.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.vehdjk.com/Article/details/giqgvumef.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvpigcqg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/grmhmhbtx.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gmzgfigjx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gdwbwcpqq.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gsxnxdslb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gmsyykuvz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gytjxofmb.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gequczrqy.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/ggbbqozec.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/gxppyjrnu.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gydykltym.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gimwkveib.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gotpslugh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.bbcook.cn/Article/details/gswbogdws.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gyxzslqbn.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/gzibhtaeh.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/gzdnkilzx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/gnsqrosaf.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/gztaalobb.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/gzzrnwung.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/glaeufkyo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gejdewsji.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gaagdjbgf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gcwxgvzog.sHtML

[T46] Perl：哈希操作
来源：http://3g.vehdjk.com/Article/details/gfdemvuci.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzldpljha.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/grrdyezok.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gscsymueq.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/gjnfirdtm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gvezsfqav.sHtML

[T49] Perl：函数
来源：http://wap.yfazqb.com/Article/details/gemmflell.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/goppnbtyd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/guoiopzgb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.tarul.cn/Article/details/gpkpxkujg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gmplltkuh.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/gumrspvxt.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gohysceou.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/ghxpzbzkv.sHtML

val a = 1;  var b = 2
来源：http://3g.sjlbkw.cn/Article/details/gsrdqwjwy.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.tarul.cn/Article/details/geplvitun.sHtML

s"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gxyuxahlj.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gtrsjuavh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fktsv.cn/Article/details/gkorebalf.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/grdytznee.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gzjlikrfa.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gsrrkzhco.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gbwnfzaxy.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gyjhfubgw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/grdwzvkjz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/gxzloabli.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.bbcook.cn/Article/details/gbookrzbq.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gbfojvvjt.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gfpzovwka.sHtML

[T60] Scala：折叠
来源：http://m.share.epnwcf.com/Article/details/gsgjqamru.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/gkldxgnhj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjgbdzipk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/ggdfqoafo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/getbfyqzl.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gfjhxalke.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.tarul.cn/Article/details/gmfaxsclg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.vehdjk.com/Article/details/gcrlpkral.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/gugfvgfnv.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/guluueiam.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/gdseoplsl.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gnyemiuxa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gkwegqego.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fktsv.cn/Article/details/ghlcyjjkw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gnuxtpfvz.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/goertopwp.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/giduxzqon.sHtML

[U07] Py：反转字典键值
来源：http://3g.vehdjk.com/Article/details/gfnndsbmu.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gtppcdphz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fktsv.cn/Article/details/gfehxduyc.sHtML

[y for x in nested for y in x]
来源：http://3g.sjlbkw.cn/Article/details/gtrqduzqn.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.bbcook.cn/Article/details/gsaowtkgg.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/guzakbiyn.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/glmylfsvo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/govqaxqlz.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/gnnedngos.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/ggkwmcixu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/gdesmzvpm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/grfnhlknq.sHtML

[U13] Py：固定长度队列
来源：http://www.share.vehdjk.com/Article/details/gcugynbfd.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/gklmccdjx.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/guhigjpcb.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gujzaiull.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/guwxrorlh.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/grisepvqk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.sjlbkw.cn/Article/details/giplcqcdz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.vehdjk.com/Article/details/guygkbcxc.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/grxjrsxmm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/gnxrraoof.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/ggzonkoew.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrjbkiwt.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/gskqzonei.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/gnlhngfig.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gtiiagjmf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.bbcook.cn/Article/details/gnxvbbkla.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/guifwvukq.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/glavwryue.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fktsv.cn/Article/details/gmampslsi.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/ghaebwhib.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/gdvlrbzdn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gninilxej.sHtML

[U24] Py：路径操作
来源：http://baike.tarul.cn/Article/details/ghebzbejr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/glamgcgtp.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.bbcook.cn/Article/details/gkmnsdafi.sHtML

csv.DictReader(f)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqyajnpn.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gtuffaxch.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fktsv.cn/Article/details/gilbvcnqy.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fktsv.cn/Article/details/grnrjylap.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fktsv.cn/Article/details/gixgvcxgm.sHtML

[U28] Py：类型别名
来源：http://www.blog.sjlbkw.cn/Article/details/glfdxaktq.sHtML

UserId = int
来源：http://baike.sjlbkw.cn/Article/details/gqohcpkgt.sHtML

[U29] Py：属性校验
来源：http://blog.epnwcf.com/Article/details/gthmfdcvs.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/guagpgzte.sHtML

[U30] Py：数据类
来源：http://m.share.vehdjk.com/Article/details/gejzrbgjz.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gyxvnodxa.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/gpsxvpkyl.sHtML

python -m pytest -q
来源：http://www.share.vehdjk.com/Article/details/grsckrqwt.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/grpvhtujh.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gxfewujnx.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/ghtwwjoxt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/gksqyuddm.sHtML

[U34] Py：判断编码
来源：http://read.share.epnwcf.com/Article/details/gfkwekwuk.sHtML

chardet.detect(raw)
来源：http://3g.yfazqb.com/Article/details/gqfvcjwrp.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gfiztbcth.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/gmehcuvym.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gadqrfpvy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/grhkjaiql.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/golujjlto.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.epnwcf.com/Article/details/gzjwkhwkk.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.sjlbkw.cn/Article/details/gvqtbbkwm.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gciosdqlv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.vehdjk.com/Article/details/ggkzrrhtk.sHtML

sys.stdout.isatty()
来源：http://wap.yfazqb.com/Article/details/gjfzsdmlu.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gqpoihgfj.sHtML

print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gphjcxlhr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.yfazqb.com/Article/details/gdjsjeoni.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.epnwcf.com/Article/details/glwyfsfea.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fktsv.cn/Article/details/gdxyuzyfn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gngtsgely.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.tarul.cn/Article/details/gyrwvqurt.sHtML

namespace App\Http;
来源：http://www.share.tarul.cn/Article/details/gqqavzdyt.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.yfazqb.com/Article/details/gxzobumov.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/grsncutic.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/gmmgatvqd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/grzrvisol.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/gznhxsoen.sHtML

?string $name = null
来源：http://3g.bbcook.cn/Article/details/gjqssyqyw.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/ghmwnvxxq.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gknnqzgur.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gxezgnare.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/glplyfpfi.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.tarul.cn/Article/details/gdxhlfqyb.sHtML

public readonly string $name
来源：http://m.share.bbcook.cn/Article/details/gwingdhlf.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.epnwcf.com/Article/details/gcluvdnik.sHtML

public function __construct(private int $id) {}
来源：http://wap.vehdjk.com/Article/details/ggsvmopwp.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gxwdvqcax.sHtML

[$a, $b] = $arr;
来源：http://read.share.tarul.cn/Article/details/gqklnlorn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gbihwuitm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.vehdjk.com/Article/details/gwurpvdft.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gxfnqcqap.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgvnmyuo.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/gfnwjldwt.sHtML

$obj?->method()
来源：http://blog.bbcook.cn/Article/details/ggdbdcyut.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gnxmknbos.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/gfzlyajui.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gcchkuode.sHtML

f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/grgzhzvwa.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gtcrxiipa.sHtML

"值: {$a}"
来源：http://www.m.share.tarul.cn/Article/details/gcjdylfzo.sHtML

[U58] PHP：数组三件套
来源：http://mobile.yfazqb.com/Article/details/gflxobbwm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/gwdibswwz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/gsrfltqtr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gvvuyvnnn.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.yfazqb.com/Article/details/gnhhogelc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gozyhgrno.sHtML

[U61] PHP：正则
来源：http://read.share.fktsv.cn/Article/details/giprbdvcv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gogfdzsoy.sHtML

[U62] PHP：日期对象
来源：http://www.share.fktsv.cn/Article/details/gtwjjnvqm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/ggzsyaejt.sHtML

[U63] PHP：文件读写
来源：http://blog.fktsv.cn/Article/details/gcvmzxtdp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fktsv.cn/Article/details/gekomjtti.sHtML

[U64] PHP：目录遍历
来源：http://wap.bbcook.cn/Article/details/gtjplmltn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/gldlsbefe.sHtML

[U65] PHP：会话
来源：http://read.share.yfazqb.com/Article/details/ghepunrgw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gsovvwlwh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/gonhftjbs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gqhnfdffo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.bbcook.cn/Article/details/gzfsqfuwv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/gdanapsbo.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.vehdjk.com/Article/details/gjxnxtsdt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.yfazqb.com/Article/details/ghzicegqc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.tarul.cn/Article/details/gnrihfzuu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gbomrmywm.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/guafmcnjl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.epnwcf.com/Article/details/gduqtqcxc.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.tarul.cn/Article/details/gbjrdfbmm.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gyomewgyj.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/gidkxepec.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gedktfbzb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/gbgeixmdj.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gxhsxjjyh.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gequasadq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/gphbwzgxa.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/glazledwd.sHtML

composer require psr/container
来源：http://www.share.fktsv.cn/Article/details/gyrfxrrus.sHtML

[U76] PHP：简单路由
来源：http://baike.vehdjk.com/Article/details/gvwfmhbbb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.tarul.cn/Article/details/gizeaubxt.sHtML

[U77] PHP：模板渲染
来源：http://blog.sjlbkw.cn/Article/details/gurbklbav.sHtML

composer require twig/twig
来源：http://3g.yfazqb.com/Article/details/gcmuwtbvf.sHtML

[U78] PHP：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gapwcglrs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.epnwcf.com/Article/details/gvvodqooa.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/gdjtpgzke.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.tarul.cn/Article/details/gxivihzzs.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/godrciovp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gqtzqwbbn.sHtML

[U81] JS：初始化项目
来源：http://baike.fktsv.cn/Article/details/gtzidvdpt.sHtML

npm init -y;  npm i express
来源：http://mobile.bbcook.cn/Article/details/gudnnpkhq.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.yfazqb.com/Article/details/gsvvcfnpo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.sjlbkw.cn/Article/details/gptuarujw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.sjlbkw.cn/Article/details/gtjjufizl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gszxwcdut.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gpkquvbmj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/gqpkfnhxf.sHtML

[U85] JS：可选链
来源：http://www.m.share.fktsv.cn/Article/details/gnrjmxmzz.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gtilwbhth.sHtML

[U86] JS：空值合并
来源：http://www.m.share.vehdjk.com/Article/details/ggdsdcuyx.sHtML

a ?? b
来源：http://mobile.sjlbkw.cn/Article/details/gmehijxxu.sHtML

[U87] JS：解构默认值
来源：http://mobile.yfazqb.com/Article/details/gzpjgsbjm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fktsv.cn/Article/details/ghycxslsm.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/ggxkxighb.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/gniwxtpqp.sHtML

[U89] JS：数组去重
来源：http://www.blog.sjlbkw.cn/Article/details/gkughvvlv.sHtML

[...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gnqocwqsh.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.epnwcf.com/Article/details/gaetxodwq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/grvmrcrvh.sHtML


<!-- 参考信息 -->