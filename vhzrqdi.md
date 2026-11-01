代发 wailian999

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gitknytxj.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gvinekixg.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gihcwomud.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gshtgygpa.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gxsncoqab.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gymretvgi.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gicixtjur.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gixljqsrm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gkzmugnna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gqbbksusv.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/guteuoyxo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gyuczqqeu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gjdqslswq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gxgcczzte.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gkyzegsey.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gqoinciiz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/gsrlgkxpz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gwutusznd.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/ggauumipq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gjmlkknrt.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/gzugaxkgb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/ghkpqyvdq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gtdguxkul.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gmjuglzhr.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gvrtvfplb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fktsv.cn/Article/details/ghiuhnmhk.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gliayvqov.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/glbgizezn.sHtML

[T15] Kotlin：接口
来源：http://3g.fktsv.cn/Article/details/gdbfiufnf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gzgeejlmm.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/guzlppnhu.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gtdrszwzd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/glwdfqwzo.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/goskdbuog.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/guxvvcezd.sHtML

"值: \(b)"
来源：http://m.share.epnwcf.com/Article/details/gvjkhqjtl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gaeriiibc.sHtML

if let n = opt { print(n) }
来源：http://baike.yfazqb.com/Article/details/gqvqelcxp.sHtML

[T20] Swift：数组操作
来源：http://blog.bbcook.cn/Article/details/ggmbypesg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gfmkuqtkj.sHtML

[T21] Swift：遍历
来源：http://baike.vehdjk.com/Article/details/gmejwkzkl.sHtML

for x in a { print(x) }
来源：http://3g.sjlbkw.cn/Article/details/gzatxoyya.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/gxwnlhbwe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/grjomoyby.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gltnpdiiq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.tarul.cn/Article/details/gdsdjnbeb.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gouyfcgog.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gdwbkneel.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gyzasxmry.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/geazbknot.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/ggeftrnke.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gjlpszrqd.sHtML

[T27] Swift：错误处理
来源：http://wap.sjlbkw.cn/Article/details/gguwidxhl.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gwsqmmsgn.sHtML

[T28] Swift：枚举
来源：http://baike.epnwcf.com/Article/details/gjfvhsadd.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gmgczpokz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/gvkstvdlv.sHtML

guard let x = opt else { return }
来源：http://baike.bbcook.cn/Article/details/ghkgqsowj.sHtML

[T30] Swift：协议
来源：http://blog.yfazqb.com/Article/details/giazjjpio.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gjoicpsbl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/ggfcievve.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/glpswobcd.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gwsiitpnu.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/girjhgilq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gdkapuqtk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/ghsmkgubv.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gemwfkbyq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.yfazqb.com/Article/details/gonpngvqo.sHtML

[T35] Lua：字典表
来源：http://3g.vehdjk.com/Article/details/gdburbmcf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gwhrobiuc.sHtML

[T36] Lua：函数
来源：http://baike.yfazqb.com/Article/details/ggnqxhldk.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/ghrkaftgo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gewtaysvq.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gcivgcmqq.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/gfpextpej.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/grxpvdidi.sHtML

[T39] Lua：模式匹配
来源：http://m.share.bbcook.cn/Article/details/genzjhqlt.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gwtawnxla.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gnwzsyqcx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/ggmhcjnma.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gxhcngumj.sHtML

print "Hello\n";
来源：http://www.m.share.epnwcf.com/Article/details/ghvtksqpa.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/glucjqzdb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.bbcook.cn/Article/details/gerxwffdj.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/gecfcedwm.sHtML

"值: $a"
来源：http://mobile.fktsv.cn/Article/details/gyxeeughq.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/genftswck.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gwsgvdxlu.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gakryzcfp.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/gldlospuh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.vehdjk.com/Article/details/gnssqaeal.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.vehdjk.com/Article/details/gwpxkyugh.sHtML

[T47] Perl：正则捕获
来源：http://wap.bbcook.cn/Article/details/guuisjlqc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gjqhpgdav.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/glhssyhfe.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/gzqcmwbwh.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/gdqeyqxer.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/grdrjmvey.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/galfvigam.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/gnliwrpgh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.sjlbkw.cn/Article/details/gjvfhwhsr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gmwizjgdv.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gnhlwrsvx.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/guakqykwt.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gbxghfdsa.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gtlkakfdz.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/grvpsmwwd.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gbtksjdeu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.yfazqb.com/Article/details/gxqhhrzvi.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/ghtkvejss.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gqpyqebei.sHtML

[T56] Scala：样例类
来源：http://www.m.share.tarul.cn/Article/details/gxsvqbewg.sHtML

case class User(name: String, age: Int)
来源：http://wap.vehdjk.com/Article/details/gbiuuxcng.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gfavfsqth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gwdcocukg.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/gcmkmgsyo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gyryemsvd.sHtML

[T59] Scala：循环
来源：http://blog.tarul.cn/Article/details/gtwplbsmb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.bbcook.cn/Article/details/gubgphfcx.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gwcuolczu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/gftobpici.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxjqjjzxa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gbrkpynvp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsqorycbp.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.vehdjk.com/Article/details/ghrcxpswh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gqvtsvvqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxxjcxtb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fktsv.cn/Article/details/ghtcyhdtg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.vehdjk.com/Article/details/gmcfscdvs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.yfazqb.com/Article/details/gyommmqsc.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gfckakslw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.vehdjk.com/Article/details/gojtetuxl.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/gjgotcxmh.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gtibafomu.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gsjgdpinr.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/giovaekin.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.yfazqb.com/Article/details/gkspeawwe.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.epnwcf.com/Article/details/goqazphsj.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/gvavjvegs.sHtML

[y for x in nested for y in x]
来源：http://www.share.yfazqb.com/Article/details/gvkbqkmwq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gtapebtaj.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/gksmaymes.sHtML

[U10] Py：按值排序字典
来源：http://3g.fktsv.cn/Article/details/ghhltlvhc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gqdrsyfbt.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/gvfvwziiu.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/gvchohqrc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gaudbjwta.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fktsv.cn/Article/details/guaczqdrw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.yfazqb.com/Article/details/gajgrcowb.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/gifsvwpdn.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fktsv.cn/Article/details/geemoaxuh.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gxdglgqzs.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/grhcruwja.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gnoyknlft.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/gjtietbqc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.epnwcf.com/Article/details/gstknfywi.sHtML

[U17] Py：初始化日志
来源：http://blog.sjlbkw.cn/Article/details/gghzvolla.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gzedncgpn.sHtML

[U18] Py：预编译正则
来源：http://m.share.fktsv.cn/Article/details/gfqnlqzhh.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gzsnpxpxm.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/goftyxyte.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/gvoxwvhun.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/gxtjuswuy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.sjlbkw.cn/Article/details/ggtsnvgpi.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/guzyhwjpo.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/geunvxcgl.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.vehdjk.com/Article/details/gfrxvnsur.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/ggwhoorzm.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.vehdjk.com/Article/details/ggkrvwfqh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.yfazqb.com/Article/details/gcheuksbw.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gqtfqpgrp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gyaehfxzh.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.bbcook.cn/Article/details/gnjxpskgj.sHtML

csv.DictReader(f)
来源：http://www.blog.tarul.cn/Article/details/gmwaxbzmc.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gsclbkxcu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gpyxalnnj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.vehdjk.com/Article/details/gwkudkcvv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/gurvgkxlv.sHtML

[U28] Py：类型别名
来源：http://baike.bbcook.cn/Article/details/gikbirmzv.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gnntxyxkd.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gcckkjpjy.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/ghnpqykop.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gkmhlxiqk.sHtML

@dataclass(slots=True)
来源：http://blog.bbcook.cn/Article/details/gijngqeat.sHtML

[U31] Py：单测
来源：http://blog.tarul.cn/Article/details/gthixclnt.sHtML

python -m pytest -q
来源：http://wap.sjlbkw.cn/Article/details/gbegpyqsd.sHtML

[U32] Py：代码格式化
来源：http://baike.epnwcf.com/Article/details/gkxfkrrwp.sHtML

ruff format . && ruff check --fix .
来源：http://3g.yfazqb.com/Article/details/gbrdbmcna.sHtML

[U33] Py：打包发布
来源：http://read.share.yfazqb.com/Article/details/gyzomnawh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gownoyqwm.sHtML

[U34] Py：判断编码
来源：http://www.m.share.bbcook.cn/Article/details/gcctnbfzl.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/giedwkjiz.sHtML

[U35] Py：发送邮件
来源：http://blog.epnwcf.com/Article/details/ghlywyqtz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.yfazqb.com/Article/details/gkyakftgw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gywpmcxac.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gexkukbhx.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gscbrkcci.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.tarul.cn/Article/details/gqydqrmka.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gfbiyfuev.sHtML

Path(__file__).resolve().parent
来源：http://www.share.sjlbkw.cn/Article/details/gkgtbjois.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/ganzpjeat.sHtML

sys.stdout.isatty()
来源：http://www.m.share.bbcook.cn/Article/details/gqtslfqtm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/gfjdqdjzy.sHtML

print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gjabgkywn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/goyzrhbxv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.tarul.cn/Article/details/gsnagpyxp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.yfazqb.com/Article/details/gybnhdppg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/ggatbmmsa.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.vehdjk.com/Article/details/gqlwdmukd.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/ghngnfmfe.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/guvevcibz.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/glnvoyunq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fktsv.cn/Article/details/ghiyfzcfy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gqvpqioyl.sHtML

[U46] PHP：可空类型
来源：http://3g.vehdjk.com/Article/details/gmpnklnfc.sHtML

?string $name = null
来源：http://read.share.bbcook.cn/Article/details/ghnptqqmr.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/gomjhngkd.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gbwtlypla.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.vehdjk.com/Article/details/gvddmrqxn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.yfazqb.com/Article/details/gahqalqoh.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fktsv.cn/Article/details/gbpcqlhrn.sHtML

public readonly string $name
来源：http://www.blog.vehdjk.com/Article/details/gbjdyyonm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.epnwcf.com/Article/details/gtmkwhdwa.sHtML

public function __construct(private int $id) {}
来源：http://m.share.sjlbkw.cn/Article/details/gsiiakvjn.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gogazjesd.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/gxsstrocp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gfypkuyxd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.yfazqb.com/Article/details/giocdnkhd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/gwzvcudxu.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.epnwcf.com/Article/details/gejyewvxb.sHtML

[U54] PHP：空安全调用
来源：http://blog.vehdjk.com/Article/details/gogmfiyfd.sHtML

$obj?->method()
来源：http://baike.vehdjk.com/Article/details/gyqtcxuyt.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.yfazqb.com/Article/details/gukowpmnz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gssvmggti.sHtML

[U56] PHP：命名参数
来源：http://mobile.vehdjk.com/Article/details/gydixgcjm.sHtML

f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gmzvkxcvr.sHtML

[U57] PHP：字符串插值
来源：http://wap.tarul.cn/Article/details/gfupibdzy.sHtML

"值: {$a}"
来源：http://www.share.vehdjk.com/Article/details/gnhfvdmgb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.sjlbkw.cn/Article/details/gmlrdemvq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.yfazqb.com/Article/details/gpumyrzcd.sHtML

[U59] PHP：自定义排序
来源：http://read.share.tarul.cn/Article/details/ginuntyxm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/ghsssckoc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.yfazqb.com/Article/details/gxqvbukai.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.bbcook.cn/Article/details/gkytukked.sHtML

[U61] PHP：正则
来源：http://read.share.bbcook.cn/Article/details/gtznjgpoi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gtgfoslhh.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/gzdqvzqeg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/gxnzbiczk.sHtML

[U63] PHP：文件读写
来源：http://baike.sjlbkw.cn/Article/details/gouiwptfq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.tarul.cn/Article/details/gpaksfwhu.sHtML

[U64] PHP：目录遍历
来源：http://www.share.sjlbkw.cn/Article/details/gblbqjcst.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/gxolxszoe.sHtML

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/gslxwznod.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gdznpxofq.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fktsv.cn/Article/details/gkbkqubys.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.sjlbkw.cn/Article/details/gseyakujb.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fktsv.cn/Article/details/gdtttfzax.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.bbcook.cn/Article/details/gqpcsdecw.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.epnwcf.com/Article/details/gpyysctaa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/gzhkgqvso.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.sjlbkw.cn/Article/details/gcppnkoay.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/gbdxckfdn.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.yfazqb.com/Article/details/gtcsyqpzo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.vehdjk.com/Article/details/gjhwsjyjm.sHtML

[U71] PHP：抛出异常
来源：http://m.share.bbcook.cn/Article/details/glhdlciti.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.tarul.cn/Article/details/gddnymhuu.sHtML

[U72] PHP：写错误日志
来源：http://blog.fktsv.cn/Article/details/gdsvdicid.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.vehdjk.com/Article/details/grcuhssal.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.bbcook.cn/Article/details/gchczvoyp.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/glfmojmes.sHtML

[U74] PHP：读取环境变量
来源：http://3g.bbcook.cn/Article/details/glibfvfbf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gkxffbrry.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/gtlslgygx.sHtML

composer require psr/container
来源：http://3g.sjlbkw.cn/Article/details/gmrfpalap.sHtML

[U76] PHP：简单路由
来源：http://m.share.fktsv.cn/Article/details/gjadzuvkz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gksbmgbum.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.sjlbkw.cn/Article/details/gxumepyog.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/gqndjfywe.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gsfwrkvhp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gypctqods.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/gccgwtiha.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.sjlbkw.cn/Article/details/gejhjucip.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.tarul.cn/Article/details/gvljtidzb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/gldtqovem.sHtML

[U81] JS：初始化项目
来源：http://blog.yfazqb.com/Article/details/gkqbhjyzz.sHtML

npm init -y;  npm i express
来源：http://mobile.sjlbkw.cn/Article/details/gtocidiyl.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gfjqcohmc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fktsv.cn/Article/details/gmnothpmp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.bbcook.cn/Article/details/gqpxjrqqe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gwcgozdlt.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.sjlbkw.cn/Article/details/gtqmmjjyb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/gxvngrkev.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/gbnkkusyc.sHtML

a?.b?.c
来源：http://3g.sjlbkw.cn/Article/details/gadgzbssd.sHtML

[U86] JS：空值合并
来源：http://mobile.epnwcf.com/Article/details/gecokaqow.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gnfcgsbfr.sHtML

[U87] JS：解构默认值
来源：http://mobile.tarul.cn/Article/details/gjstnytcn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/ggalauueb.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gelvrregg.sHtML

{ ...a, ...b }
来源：http://m.share.fktsv.cn/Article/details/glgtxbpfc.sHtML


<!-- 参考信息 -->