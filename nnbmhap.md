代发 wailian999

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/gqrezgecy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gqoahigzt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.bbcook.cn/Article/details/gmhsgnzaw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/grzfvvqzw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/gimbzchwu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gehhkvdbc.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/gksalvpvj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/girivmzvf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gjmkuwmpt.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gducjvlxc.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/gvkuyxgwi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gfatcsulb.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gzdjqompu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gotaeuwau.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/gavfgdpys.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvvnkesv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.yfazqb.com/Article/details/gcdozadjj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/gfkzxknjd.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gaeaprjqb.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gokuxcxmx.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gbzkqjmzl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gbucpfale.sHtML

[T16] Swift：Hello World
来源：http://mobile.yfazqb.com/Article/details/gsawhylfj.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gfvubwcjo.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/grqscmoxr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gwcufkyqu.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/gxedrlgja.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gmtzemmsq.sHtML

[T19] Swift：可选绑定
来源：http://baike.epnwcf.com/Article/details/gzxiukphf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/giapofkxe.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gsmtcgued.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gpchdjlcw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.yfazqb.com/Article/details/gyukbyexh.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gkgtguhrr.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/glosjsitp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gwxehynou.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gsblxsspa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/goigwuxrq.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gjrknhvzs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gvvebqgzp.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/gufnoasuy.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gkbayjfoi.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gthhwmrmt.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gfvmnzvgy.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gygsmwgpq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gaxthegnn.sHtML

[T28] Swift：枚举
来源：http://3g.epnwcf.com/Article/details/gjwjpewoy.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/grlauclpc.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.vehdjk.com/Article/details/gbkedprjc.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gtxaqqdfo.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/gwlvexnaj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gmvxdwtvd.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gguftfmti.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gywyrvphw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.bbcook.cn/Article/details/gawvttltl.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gbmgxzrsp.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/gwrjnhzsg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gywrprgoq.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gsnirtvcu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gnzrvhdgr.sHtML

[T35] Lua：字典表
来源：http://www.blog.sjlbkw.cn/Article/details/ggxsfazjt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.epnwcf.com/Article/details/gcyjjtvgf.sHtML

[T36] Lua：函数
来源：http://blog.sjlbkw.cn/Article/details/getcauqsd.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/ggsgzlvgo.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gyqjavbtt.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gjelnihjn.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/gmbxsvpbr.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gymsapxxd.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gnggyjgvt.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gprsnqytl.sHtML

[T40] Lua：元表
来源：http://read.share.bbcook.cn/Article/details/gifmrbwmv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.epnwcf.com/Article/details/gxmrlzeqt.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gfbdjpeqm.sHtML

print "Hello\n";
来源：http://wap.vehdjk.com/Article/details/glaztgjzf.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gvwfgqvce.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/grmjkcwhi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gsasmetpf.sHtML

"值: $a"
来源：http://blog.fktsv.cn/Article/details/gubjqdylr.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/gbywuyryx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/gaisarokd.sHtML

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gneggtzei.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.tarul.cn/Article/details/gakkkmevz.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gxircabiu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/glqcsorbn.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/gvupqnvyc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gyhzzsewx.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/gzsqcjzrq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/glpryrhfy.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gggmykxhh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gzzrjgjos.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/ghzullqux.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/ghcagbyfz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gsrjnkgyl.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/glqwyhbpe.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gzetcknbw.sHtML

[T52] Scala：变量
来源：http://mobile.bbcook.cn/Article/details/gknprnmwf.sHtML

val a = 1;  var b = 2
来源：http://baike.tarul.cn/Article/details/gqjlcpsyt.sHtML

[T53] Scala：字符串插值
来源：http://3g.bbcook.cn/Article/details/gpvaelija.sHtML

s"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gjdvrluhs.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gcszqaaby.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gjboznnoa.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fktsv.cn/Article/details/glkkmkrzl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gokxelqwa.sHtML

[T56] Scala：样例类
来源：http://www.blog.vehdjk.com/Article/details/gyeobsbkr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gqiexynhq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gvzjgxwph.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/ghyqrpwgp.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gimdspprw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.epnwcf.com/Article/details/gciptgkzo.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gbdujqmqp.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.tarul.cn/Article/details/gjyczfmjc.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/ghsjodzxq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gfprpcyzb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbleuxiub.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gqxkzadhs.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdyykidlt.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.bbcook.cn/Article/details/gfnmtbmwt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/grgkvneyv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.bbcook.cn/Article/details/gzrfuevgk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gkcyufsui.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.yfazqb.com/Article/details/gjakkqffa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/gimkgwxtn.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gvhlysfqd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gprgbqryb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gkwakusjo.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gykvvrogs.sHtML

[U06] Py：合并两个字典
来源：http://www.share.tarul.cn/Article/details/gjvibfxpm.sHtML

{**a, **b}
来源：http://www.m.share.bbcook.cn/Article/details/ghjxgvcif.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gwtlffpoa.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/gttumpsft.sHtML

[U08] Py：展平二维列表
来源：http://3g.tarul.cn/Article/details/gfkoktepp.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gbcidundb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/gmfbjhpmm.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/gklbfbizj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.yfazqb.com/Article/details/ggaxinroh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.tarul.cn/Article/details/gqfibakmc.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fktsv.cn/Article/details/glqixtgpj.sHtML

(x * 2 for x in arr)
来源：http://mobile.epnwcf.com/Article/details/gqssvdokf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/guxarqfzj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/gtxvajord.sHtML

[U13] Py：固定长度队列
来源：http://wap.vehdjk.com/Article/details/gsxlqjjbq.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gjexaoijh.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gbyhpvbhv.sHtML

defaultdict(list)
来源：http://wap.sjlbkw.cn/Article/details/gnrpzbvcv.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.vehdjk.com/Article/details/ggvvpvvul.sHtML

t = time.perf_counter()
来源：http://m.share.sjlbkw.cn/Article/details/gjwssgyji.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/gesnpzfud.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gulmgfmlv.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gvpjuvkyj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gncvkxmuw.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/gvxhhnmtf.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/gugdzkeho.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gfbwqrmnh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.vehdjk.com/Article/details/ggrfqabqr.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.sjlbkw.cn/Article/details/gmvuvijit.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/ghlrqzyto.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.epnwcf.com/Article/details/glqpqhqje.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gpqcyzmnq.sHtML

[U22] Py：矩阵转置
来源：http://3g.tarul.cn/Article/details/gsqppkkmo.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/gzjuexnsa.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/gncynqtcb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fktsv.cn/Article/details/gdkusiuvz.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gnosehdbe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gouymxbwo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.vehdjk.com/Article/details/gmzwcmdel.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gxvbjarvu.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/gzltjafnz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/grlwjsnka.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/genfmhnfa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.bbcook.cn/Article/details/gexzdrlog.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/grhesdkhz.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gvqrieidu.sHtML

[U29] Py：属性校验
来源：http://m.share.tarul.cn/Article/details/gzejznzkj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/gzpkhsacn.sHtML

[U30] Py：数据类
来源：http://wap.epnwcf.com/Article/details/gxogpvaok.sHtML

@dataclass(slots=True)
来源：http://blog.fktsv.cn/Article/details/gbgrnuwsq.sHtML

[U31] Py：单测
来源：http://read.share.vehdjk.com/Article/details/godtbbopy.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gnnemuhil.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/gjrzhmxht.sHtML

ruff format . && ruff check --fix .
来源：http://blog.vehdjk.com/Article/details/gyznzuytk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/gblhkuqwi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gypwpsuga.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gdkblwmch.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/glehocjtf.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/gakoexefx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/ggozcrhcw.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gvbvravwv.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.epnwcf.com/Article/details/guglimbsd.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/gdlfefqho.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.epnwcf.com/Article/details/gouzporib.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.vehdjk.com/Article/details/gvprrjjjf.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.tarul.cn/Article/details/gqbyzkwpg.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.bbcook.cn/Article/details/gznyudltg.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/gdghcnlki.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/guyzhsfxy.sHtML

print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gssneejfe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.bbcook.cn/Article/details/gcczjbjpx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fktsv.cn/Article/details/geioejtjr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.yfazqb.com/Article/details/grjtyumhn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.bbcook.cn/Article/details/gweifhfsx.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.bbcook.cn/Article/details/ghhybjklp.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gwcmcegte.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gnkbqcdfo.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/gybqtyozl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/giccgqxcn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gvattpvwl.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gzqsfamxl.sHtML

?string $name = null
来源：http://www.share.sjlbkw.cn/Article/details/grfwymqup.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gulqruhce.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gaqrdsong.sHtML

[U48] PHP：纯枚举
来源：http://baike.tarul.cn/Article/details/gjefilclw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gzagwpivk.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gbbdzjayg.sHtML

public readonly string $name
来源：http://read.share.epnwcf.com/Article/details/gyxwwmhqs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/glocwxysf.sHtML

public function __construct(private int $id) {}
来源：http://mobile.tarul.cn/Article/details/gyrrsteof.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gsonafxyz.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gakkzzveh.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gqwhelhex.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fktsv.cn/Article/details/grdeckdsl.sHtML

[U53] PHP：空合并运算符
来源：http://wap.bbcook.cn/Article/details/gxtnbmddp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.yfazqb.com/Article/details/gjjtqztis.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/graoqaovt.sHtML

$obj?->method()
来源：http://mobile.yfazqb.com/Article/details/ghipzofys.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/gmqcejvts.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.vehdjk.com/Article/details/gxjqjfous.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gsmobdmnq.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/glsczjijt.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gbbsinsgr.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gvdfbmyft.sHtML

[U58] PHP：数组三件套
来源：http://m.share.vehdjk.com/Article/details/ghimpaueu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gveraxtwz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gmeqymczd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/gwksxrrzs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/gopledcwm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/gtbofjcgo.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gwpfkzhxv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gocbpjkio.sHtML

[U62] PHP：日期对象
来源：http://m.share.epnwcf.com/Article/details/gzbtaalfb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.sjlbkw.cn/Article/details/gotqlwmbc.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/genudqbye.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/grxgcdkfw.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gzgybfiqn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/ggclbzesv.sHtML

[U65] PHP：会话
来源：http://blog.vehdjk.com/Article/details/gvzvoidai.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gmqnwesxs.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/gnpjcjvmu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/gtsxorzjf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.vehdjk.com/Article/details/grkrminge.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.bbcook.cn/Article/details/gbtfowkcr.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gtplaizcg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.tarul.cn/Article/details/gjrkyqaft.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.tarul.cn/Article/details/gnzyqwfqx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gdxqwklax.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fktsv.cn/Article/details/gwmafaqve.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.sjlbkw.cn/Article/details/ggcjnvfvt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/goxtajczl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/gglvqhhxg.sHtML

[U72] PHP：写错误日志
来源：http://wap.fktsv.cn/Article/details/gbfatlrvd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/gxwwvqmdy.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/ghhubjxpo.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.sjlbkw.cn/Article/details/gwvactwlo.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gmykyvwcz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gylhunbxd.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/ggzaerkar.sHtML

composer require psr/container
来源：http://m.share.vehdjk.com/Article/details/gsqkhlwou.sHtML

[U76] PHP：简单路由
来源：http://wap.epnwcf.com/Article/details/ghujqluya.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.epnwcf.com/Article/details/gezoqlnsm.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gcuexsghk.sHtML

composer require twig/twig
来源：http://3g.bbcook.cn/Article/details/gsitfsmzu.sHtML

[U78] PHP：单元测试
来源：http://baike.bbcook.cn/Article/details/gljcnemmh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.yfazqb.com/Article/details/goabmkixo.sHtML

[U79] PHP：静态分析
来源：http://3g.epnwcf.com/Article/details/gfnbsbzck.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.epnwcf.com/Article/details/guftcofpr.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gdhzyqbtx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/gstsuemlb.sHtML

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/glhevlviy.sHtML

npm init -y;  npm i express
来源：http://www.share.vehdjk.com/Article/details/gxcthxsqb.sHtML

[U82] JS：package.json 脚本
来源：http://wap.vehdjk.com/Article/details/ghpgrzibj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.tarul.cn/Article/details/ghkcbpwba.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.vehdjk.com/Article/details/gxcfgagwn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gkxqmbanq.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.yfazqb.com/Article/details/gvnohgqnw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.tarul.cn/Article/details/gbyehecjl.sHtML

[U85] JS：可选链
来源：http://3g.epnwcf.com/Article/details/glvpokpaw.sHtML

a?.b?.c
来源：http://www.share.bbcook.cn/Article/details/gcoqupjup.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gpyxxcnwv.sHtML

a ?? b
来源：http://www.share.sjlbkw.cn/Article/details/gzvoewybs.sHtML

[U87] JS：解构默认值
来源：http://www.share.sjlbkw.cn/Article/details/ghzvbeaan.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.vehdjk.com/Article/details/gtimsafmf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.vehdjk.com/Article/details/ghmsxufot.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gyjlkwisw.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gwoeeqcsx.sHtML

[...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gmgztprxj.sHtML

[U90] JS：数字数组排序
来源：http://baike.yfazqb.com/Article/details/grkmsxlmf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gussvtvgw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.sjlbkw.cn/Article/details/grqfflxgp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fktsv.cn/Article/details/gqgwhkguq.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/grxjyhrkc.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gdufykmel.sHtML


<!-- 参考信息 -->