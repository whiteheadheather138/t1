代发 wailian999

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/gdlluecso.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gonsculad.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/gnkmllbum.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gibockccb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/gsmsxispz.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gpzvgqqzw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gnukxbclc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gixbolipu.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gnwznbfdb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gbcdjtduw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gfegnzmip.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gqxunkrxp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/gvhawaeba.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/ggsdgkaus.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gwjrhzthh.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gprbtcwpd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gpteupdgj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/grsvenorb.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gpbkwtddl.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gzbpkanme.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gzngriwbm.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gexcxwzec.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gkvcjgbih.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gssaifzzf.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gqcfsfrso.sHtML

if let n = opt { print(n) }
来源：http://baike.sjlbkw.cn/Article/details/gahhneyod.sHtML

[T20] Swift：数组操作
来源：http://blog.fktsv.cn/Article/details/grdxgaiug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gzgolsfzk.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/ggkflnitm.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gfakikiqg.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gfxiymopn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fktsv.cn/Article/details/gvbfrrzln.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/gxjqfrasi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/ghgkqwile.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gjpdnegzp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gkcorrjnx.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/grmhceuts.sHtML

struct P { var x: Int }
来源：http://m.share.tarul.cn/Article/details/gednntued.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gmwxtcpao.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gmgfhcbfp.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/ghodfotnp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gtlboupbn.sHtML

[T28] Swift：枚举
来源：http://wap.epnwcf.com/Article/details/ghjtqmvmr.sHtML

enum Color { case red, green }
来源：http://baike.fktsv.cn/Article/details/grylkghoo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.yfazqb.com/Article/details/gzsustlgt.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gnomysdnh.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/gwnyrlyds.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.sjlbkw.cn/Article/details/gzvciqgcg.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gzedtgbdh.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/grjobkbmd.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gttnhppun.sHtML

local a = 1
来源：http://blog.sjlbkw.cn/Article/details/gluwbwpip.sHtML

[T33] Lua：表（数组）
来源：http://3g.tarul.cn/Article/details/gfybtwrfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/ghskpmdko.sHtML

[T34] Lua：遍历表
来源：http://read.share.yfazqb.com/Article/details/ggnzyvizk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gyqzjqaea.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/guzwpilyb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gjjxjxjjn.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gqrkdzgxl.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gcgmpqevf.sHtML

[T37] Lua：字符串拼接
来源：http://baike.yfazqb.com/Article/details/gstducgch.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gqhfmbhjq.sHtML

[T38] Lua：条件
来源：http://www.share.vehdjk.com/Article/details/gonidoajl.sHtML

if x > 0 then print("正") end
来源：http://mobile.tarul.cn/Article/details/gpfmcggzo.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/genpefwoz.sHtML

string.find(s, "%d+")
来源：http://m.share.tarul.cn/Article/details/gacfyxqcp.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gpiftmjbl.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.tarul.cn/Article/details/gjrdxpyvf.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/giriuaxig.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gvsqbzrip.sHtML

[T42] Perl：变量类型
来源：http://blog.fktsv.cn/Article/details/gtjeqaork.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gyomvitah.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gpjxonrly.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/gvcegvgkn.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/ghammhofn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gbazbirgc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gahnaplnk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gjvjiuybo.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/gtomnrnnn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gijomahyr.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gmyjofizy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/ghcaqqkiy.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/gxfdbjtcg.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/guxxnayui.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gsvjutblz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gnahurovr.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gigtfpsag.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gqljqxpmy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gkvdjabtu.sHtML

[T51] Scala：Hello World
来源：http://blog.yfazqb.com/Article/details/gsgrqwfbi.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/garycwliy.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/gvtxsqybs.sHtML

val a = 1;  var b = 2
来源：http://3g.fktsv.cn/Article/details/gdlimlpbx.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/ghajetolq.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gpjvudxxq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/geehamtrl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gqacyxrup.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gebgiyzrl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gjxtgpxhy.sHtML

[T56] Scala：样例类
来源：http://www.share.tarul.cn/Article/details/gfvlreujk.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/gskfdncdt.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gxrcxeesx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gmxjsihhd.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/gzzscqhns.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gwkyiynmh.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gkjzszztx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gtbyievix.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/gmyzvkbgc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fktsv.cn/Article/details/gjxvqlgeq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbznhddez.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gwrmfgnvc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gabewnqwh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gdugmtsnv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gpsgkfksn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/gflqkalpx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gwubcyhff.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/gqohizhzw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.bbcook.cn/Article/details/gwxsowyet.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/glhinscww.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fktsv.cn/Article/details/gdkxaokkl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gczqvlfst.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/guorrpeym.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gwuudfqto.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/gkgzlmihu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gnmycwxtv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/gvsmddgzm.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/gaqspfejf.sHtML

[y for x in nested for y in x]
来源：http://wap.epnwcf.com/Article/details/grwjcxpab.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gypzkmhob.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/ghqkjlbio.sHtML

[U10] Py：按值排序字典
来源：http://m.share.tarul.cn/Article/details/gdmtxobve.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gvssrqkuq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.sjlbkw.cn/Article/details/gbzvewsce.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gkwyuosud.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gnihilkdl.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gvynulorj.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/gntgpyxod.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/glazdzccq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/gpyvuggxq.sHtML

defaultdict(list)
来源：http://www.share.epnwcf.com/Article/details/gxiojitcy.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gwcrpycoq.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/gljcyalmw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/gphemtosc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.sjlbkw.cn/Article/details/gvwlcwwcx.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/gyknxzjom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.tarul.cn/Article/details/guelhzupg.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/givjrxnny.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gnvlcbsks.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/gfxbmcgcu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fktsv.cn/Article/details/giyamcgwr.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gibfwhpoe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/glogggemz.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/ggbwtlrkc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvgpcbwh.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/grxlmlyoq.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/gsoijagzy.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gibweyuac.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.bbcook.cn/Article/details/ghopuzfgz.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gyyuwyliu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/glxeovnpq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.sjlbkw.cn/Article/details/gosaqyiuc.sHtML

csv.DictReader(f)
来源：http://www.m.share.epnwcf.com/Article/details/gcrywwomk.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/grkqphpvf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.tarul.cn/Article/details/gqmbohnqy.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.sjlbkw.cn/Article/details/ghbywkwdo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/gvyjsoesr.sHtML

[U28] Py：类型别名
来源：http://www.share.yfazqb.com/Article/details/gqxaenvpo.sHtML

UserId = int
来源：http://baike.sjlbkw.cn/Article/details/gpmgobonx.sHtML

[U29] Py：属性校验
来源：http://baike.vehdjk.com/Article/details/gvowqsyjv.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gaypdcjkj.sHtML

[U30] Py：数据类
来源：http://wap.epnwcf.com/Article/details/gqgxeiooh.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gklxhufmj.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/ggzlpujpa.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/gumhqzcar.sHtML

[U32] Py：代码格式化
来源：http://read.share.tarul.cn/Article/details/gdickglnf.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gxmtffjeg.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gxzpstjvq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gsxzsxihj.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/gnrdfjssk.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/gslkdaugo.sHtML

[U35] Py：发送邮件
来源：http://blog.bbcook.cn/Article/details/gpoyklpqe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.tarul.cn/Article/details/gnciomdvi.sHtML

[U36] Py：定时任务
来源：http://www.blog.tarul.cn/Article/details/grobrwrip.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.tarul.cn/Article/details/gmxmcwokc.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/gvnflalnr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.epnwcf.com/Article/details/gmfsnodef.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.bbcook.cn/Article/details/guknfajsn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gtdlsfqrm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.bbcook.cn/Article/details/gglswkbbf.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gmarpxwqh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.vehdjk.com/Article/details/gsdqmlonp.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gxivyltow.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gxxgqyowi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/gexjqljbw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gonnzlcko.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.yfazqb.com/Article/details/glshubrrp.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gsabfxtdp.sHtML

namespace App\Http;
来源：http://read.share.yfazqb.com/Article/details/gxqasnzcu.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gpcrpdtzy.sHtML

declare(strict_types=1);
来源：http://baike.sjlbkw.cn/Article/details/gcddyqtjp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gtsxbrggx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gptrsomsg.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/ggvnmmusz.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gsocniefb.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/gxqqdykxs.sHtML

int|string $id
来源：http://www.blog.bbcook.cn/Article/details/gmjcnyouu.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gjipmlmhc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/gsrrfdndo.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/ghtammnjj.sHtML

public readonly string $name
来源：http://read.share.yfazqb.com/Article/details/glkcybsob.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.bbcook.cn/Article/details/gzruanpqe.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gfctrykxz.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/glcuhxemh.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/grvpsjpgg.sHtML

[U52] PHP：箭头函数
来源：http://blog.fktsv.cn/Article/details/gprcszzfm.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gaioiiomn.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fktsv.cn/Article/details/gzfecbtkh.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gypzblrbt.sHtML

[U54] PHP：空安全调用
来源：http://baike.bbcook.cn/Article/details/gnrfjatwp.sHtML

$obj?->method()
来源：http://www.share.sjlbkw.cn/Article/details/gqlufpuof.sHtML

[U55] PHP：match 表达式
来源：http://www.share.tarul.cn/Article/details/gfcnoqmsa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.yfazqb.com/Article/details/gzhhxmewx.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fktsv.cn/Article/details/gcqjsmocd.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gflvskqqj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/giabofvom.sHtML

"值: {$a}"
来源：http://m.share.epnwcf.com/Article/details/gxcwbafki.sHtML

[U58] PHP：数组三件套
来源：http://read.share.sjlbkw.cn/Article/details/gjmbbfyzz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.epnwcf.com/Article/details/gkxaljimv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gyanmvbtk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gsnyfedsb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.vehdjk.com/Article/details/ghvfptbce.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.tarul.cn/Article/details/gfwquryfi.sHtML

[U61] PHP：正则
来源：http://www.share.sjlbkw.cn/Article/details/gabbgbzxk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gtyhypcsv.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/gcngzdgfr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gqshhcihy.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/gokhvmoek.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/gcbbrfget.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gpsqhdwbt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gzefgwcvx.sHtML

[U65] PHP：会话
来源：http://baike.tarul.cn/Article/details/gyopiyloq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gxakwlkoe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/gmnenhfcj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.tarul.cn/Article/details/gtuqjchzo.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/gchwaqwnq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gwgbgwafc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/gngreypps.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.bbcook.cn/Article/details/gdjqgdspm.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/ggukclzdt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gzclstrgl.sHtML

[U70] PHP：PDO 事务
来源：http://3g.vehdjk.com/Article/details/gpszablpv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gnelykxfw.sHtML

[U71] PHP：抛出异常
来源：http://3g.fktsv.cn/Article/details/gicotidqs.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.yfazqb.com/Article/details/gwjjyjidf.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/gkfcnzzbj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.epnwcf.com/Article/details/gavreziox.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.bbcook.cn/Article/details/gcjjbvlck.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.yfazqb.com/Article/details/geyhilrsd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gymabwnvd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/gllhjkkyr.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/gfihuhqyc.sHtML

composer require psr/container
来源：http://baike.epnwcf.com/Article/details/gudcstgzv.sHtML

[U76] PHP：简单路由
来源：http://3g.bbcook.cn/Article/details/gmjhynisf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fktsv.cn/Article/details/gcwmraxpq.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.vehdjk.com/Article/details/gwmsvddwn.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/gobyjcotm.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/gytmlwhve.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.epnwcf.com/Article/details/gpsjzkuft.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.epnwcf.com/Article/details/gwtsocsvt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.bbcook.cn/Article/details/gaqvuhxtg.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.epnwcf.com/Article/details/gijllvicj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.epnwcf.com/Article/details/gkymsxxpm.sHtML

[U81] JS：初始化项目
来源：http://m.share.fktsv.cn/Article/details/gtskqygux.sHtML

npm init -y;  npm i express
来源：http://www.blog.sjlbkw.cn/Article/details/ghqnzglve.sHtML

[U82] JS：package.json 脚本
来源：http://wap.yfazqb.com/Article/details/grqzbpaqx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fktsv.cn/Article/details/gmmyfcspl.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.tarul.cn/Article/details/gnkkyggkb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gzefbkukc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.bbcook.cn/Article/details/gggbawwcf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/gostzazjo.sHtML

[U85] JS：可选链
来源：http://mobile.fktsv.cn/Article/details/gsuxlejlb.sHtML

a?.b?.c
来源：http://read.share.sjlbkw.cn/Article/details/gikvjdufn.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gjrcbfjfx.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gihnmbixi.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/gsusdmwrg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fktsv.cn/Article/details/gvmxfbhgo.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/gemjkdauh.sHtML

{ ...a, ...b }
来源：http://mobile.sjlbkw.cn/Article/details/gclztfucr.sHtML

[U89] JS：数组去重
来源：http://read.share.yfazqb.com/Article/details/gfjevkxqr.sHtML

[...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/geagdihhq.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/gagtndbrn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gqfqefviv.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.bbcook.cn/Article/details/gzvmnzulu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.sjlbkw.cn/Article/details/gmtknkzqm.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/guhglhjqa.sHtML

structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gtpfztbny.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/giwedgqdk.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gikrwsrjq.sHtML

[U94] JS：箭头函数
来源：http://wap.yfazqb.com/Article/details/gkygpaxav.sHtML

const double = x => x * 2;
来源：http://www.share.fktsv.cn/Article/details/gslxfkvis.sHtML


<!-- 参考信息 -->