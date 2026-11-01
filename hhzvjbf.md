代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gnldtihcw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxouaapc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gvfsmnojp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjhmwkvox.sHtML

[T01] Kotlin：Hello World
来源：http://blog.vehdjk.com/Article/details/gelwuhbut.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gxerdgvor.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/ghsrvcfln.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fktsv.cn/Article/details/gzkkybjbw.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/genibhrwh.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/gdpmqikuc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.sjlbkw.cn/Article/details/gsfrnagke.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/goupxupyy.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/gajvrvbmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gnkzwisxa.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gshjplixz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gpnwdmuja.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gmgynzviv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gpsdrsvta.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gkpmwnmrz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gcolgsaxs.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gszvimndv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gyalyudwq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gyosoevgr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/guxsfzgqs.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gtqcbujyk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/gxcrqbvpv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gtymwdabt.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gzjzgbhol.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gkylfcvzj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/gcbwxgwyl.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/grcofitpr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gkdyureac.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/geuxgtzdz.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gwfcfwtju.sHtML

[T16] Swift：Hello World
来源：http://blog.epnwcf.com/Article/details/gwufjatyt.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gtibvcsvp.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gxcyyhbaf.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gsgpbsema.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/giksekqvu.sHtML

"值: \(b)"
来源：http://read.share.fktsv.cn/Article/details/gebbpalil.sHtML

[T19] Swift：可选绑定
来源：http://m.share.sjlbkw.cn/Article/details/ghrloahvp.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gokkkoykc.sHtML

[T20] Swift：数组操作
来源：http://3g.bbcook.cn/Article/details/gtgidsgmx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/guztwjccs.sHtML

[T21] Swift：遍历
来源：http://baike.epnwcf.com/Article/details/gkojhfadk.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gtwfrzliv.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/guvaufeif.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gdgtsdssn.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/gfzrihaqw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/ghppmblcb.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gpxfaadaw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.epnwcf.com/Article/details/gguevifzp.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/glgkbcuas.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gtcljymfa.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/ghuatvpuf.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gpzrzbdfo.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/gwdrttdek.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/gjfpypiog.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/gkpztgmfk.sHtML

enum Color { case red, green }
来源：http://m.share.yfazqb.com/Article/details/geiupgwrl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gklfnkqbt.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gtilqkabq.sHtML

[T30] Swift：协议
来源：http://www.blog.yfazqb.com/Article/details/gugbcpgsk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gebdatjod.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gmphznifx.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gdoegrrlc.sHtML

[T32] Lua：局部变量
来源：http://blog.vehdjk.com/Article/details/gruhecyyv.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/gmlbntstv.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gqydtwmsv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gtnlepgnj.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/goudzuynk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/gatqtjdhe.sHtML

[T35] Lua：字典表
来源：http://baike.tarul.cn/Article/details/gdmrzijjo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/gkbcegfxe.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/guharxxum.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gsvskydhz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.yfazqb.com/Article/details/gxkvshjtx.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/guwdoogzp.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gejlijuuo.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gaqlisapl.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gbtpsyqqu.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/gseknkdyp.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gpaziaadn.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gkxnghkzm.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/giandfnni.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/grlxcsuna.sHtML

[T42] Perl：变量类型
来源：http://3g.yfazqb.com/Article/details/gxdhimefs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.bbcook.cn/Article/details/gukrwoept.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gvaxjjjci.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/gsuxkkawc.sHtML

[T44] Perl：条件
来源：http://mobile.fktsv.cn/Article/details/gcwjpnyiy.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.bbcook.cn/Article/details/gzijaemay.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gangnclyb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gkxypuqjp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gmtiqachm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/gztlpymaw.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/grfctnzjq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gvlpnpmtl.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/gbtjxaqoz.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gzsginckn.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gilcutwsr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gbzyjhtpg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gklnnknat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gvpkkaner.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gmjaojrtz.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gvbetnosa.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gmtgkluvl.sHtML

[T52] Scala：变量
来源：http://baike.vehdjk.com/Article/details/gbysrpxhh.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gmkdzmatl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gomhvsfrt.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gnwwbzivc.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gshvtncox.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.vehdjk.com/Article/details/grbskwptm.sHtML

[T55] Scala：集合过滤
来源：http://wap.epnwcf.com/Article/details/gyjotztwg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/gggzbroqg.sHtML

[T56] Scala：样例类
来源：http://www.blog.sjlbkw.cn/Article/details/gddddgddh.sHtML

case class User(name: String, age: Int)
来源：http://3g.vehdjk.com/Article/details/gaodcychi.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gziewgunn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gafsfhqvk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gopldqijl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gqsvgiukw.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gkmadaxrm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gjrwdjrnc.sHtML

[T60] Scala：折叠
来源：http://www.share.fktsv.cn/Article/details/ggglvhygp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/ghonjeysk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggmyheeeu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gkwwnonkr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjgdftoso.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/gxxfrukzb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/glqlagqcm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.sjlbkw.cn/Article/details/gfwgruzoz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.epnwcf.com/Article/details/gwleygjmv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.vehdjk.com/Article/details/gxrvxzbep.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gvzqhvkhh.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/gzugiimki.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/gzbjmhbvd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fktsv.cn/Article/details/gsaazvfcr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gyxodnmso.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gdelwlrjr.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/gxebmznhx.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/glhqpuuyh.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fktsv.cn/Article/details/gzncbzdtl.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/gpknkoyov.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gfgsoqbzp.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fktsv.cn/Article/details/gjddeuhaw.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/gjvmodqbs.sHtML

[U10] Py：按值排序字典
来源：http://baike.epnwcf.com/Article/details/gcrthbhkd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.yfazqb.com/Article/details/gmqaqmztm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gtjfaxtsl.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/gbkrpqohr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.tarul.cn/Article/details/gjasipwwh.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gvjyoeeco.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gsejymlhf.sHtML

deque(maxlen=10)
来源：http://blog.vehdjk.com/Article/details/gtpdzdzoi.sHtML

[U14] Py：分组收集到列表
来源：http://wap.yfazqb.com/Article/details/gxyspcbim.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/gxwnrdghd.sHtML

[U15] Py：高精度计时
来源：http://m.share.fktsv.cn/Article/details/gxqowrtjz.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/gzksqknmq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fktsv.cn/Article/details/gpvjsjopi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/gardcextq.sHtML

[U17] Py：初始化日志
来源：http://blog.sjlbkw.cn/Article/details/gcgcamgso.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.bbcook.cn/Article/details/gjnrlvasw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/gcwubndhe.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/grdivxtbs.sHtML

[U19] Py：正则替换带回调
来源：http://3g.tarul.cn/Article/details/guysphogt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gsapntppo.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gyehgpkqw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/gshmvcfbo.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gpjmlwvpz.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gavrwcxhp.sHtML

[U22] Py：矩阵转置
来源：http://wap.bbcook.cn/Article/details/gmcvhjxmy.sHtML

list(zip(*m))
来源：http://read.share.tarul.cn/Article/details/gxetoclhu.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/gdlbjgobo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gqngzvsgi.sHtML

[U24] Py：路径操作
来源：http://blog.sjlbkw.cn/Article/details/gukymcdfx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gqadlvxuf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gqkcbzhbp.sHtML

csv.DictReader(f)
来源：http://wap.fktsv.cn/Article/details/gnkyfbzxi.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/ghavldybk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/glbizqofg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gzgzkzusb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/gsmexizzs.sHtML

[U28] Py：类型别名
来源：http://blog.fktsv.cn/Article/details/gupomhilt.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gcjggstyb.sHtML

[U29] Py：属性校验
来源：http://m.share.yfazqb.com/Article/details/gzwltnqon.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/grddgfabn.sHtML

[U30] Py：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gcktdrbnt.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/gnnotvfmm.sHtML

[U31] Py：单测
来源：http://www.blog.fktsv.cn/Article/details/ghgogcmwl.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gnsioeqxu.sHtML

[U32] Py：代码格式化
来源：http://read.share.vehdjk.com/Article/details/glrppwqdt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.epnwcf.com/Article/details/ghgcglmpf.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gufsdidtx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.sjlbkw.cn/Article/details/gyspfajtu.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/grhujatkb.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gexkqjghb.sHtML

[U35] Py：发送邮件
来源：http://blog.tarul.cn/Article/details/gwbpiahop.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/gwqnxvxwk.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/gywnkjtan.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/guxdlnpwp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.tarul.cn/Article/details/gbsnkpivd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.tarul.cn/Article/details/gdxeassud.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gtippvlcc.sHtML

Path(__file__).resolve().parent
来源：http://wap.epnwcf.com/Article/details/gljzlnsxt.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.epnwcf.com/Article/details/gfgkaazjz.sHtML

sys.stdout.isatty()
来源：http://m.share.tarul.cn/Article/details/gcedxsdwz.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gzxhmzoay.sHtML

print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gkgqvumdq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fktsv.cn/Article/details/gfchdsqlo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/glcotkhba.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.bbcook.cn/Article/details/gvhayxcmj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gmilqvbyr.sHtML

[U43] PHP：声明命名空间
来源：http://wap.bbcook.cn/Article/details/gpibdvzot.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/gtruqubsn.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fktsv.cn/Article/details/gfduxbjic.sHtML

declare(strict_types=1);
来源：http://m.share.sjlbkw.cn/Article/details/gsbcocxti.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fktsv.cn/Article/details/gqpikhibh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gfmoiuubf.sHtML

[U46] PHP：可空类型
来源：http://wap.fktsv.cn/Article/details/gkoidrvop.sHtML

?string $name = null
来源：http://mobile.fktsv.cn/Article/details/gfqokylbv.sHtML

[U47] PHP：联合类型
来源：http://m.share.vehdjk.com/Article/details/gnetkxefu.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/geljmvkyh.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.yfazqb.com/Article/details/gvjsegewm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gcaepypqb.sHtML

[U49] PHP：只读属性
来源：http://mobile.vehdjk.com/Article/details/gosevfydo.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/guikehjdf.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/guilvsmts.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gvlnypusy.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/gqjzlfsbh.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gczpiyerm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gagocyeeo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/gyfnxttmc.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/gaiftzjso.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/gmnwtxbhr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.tarul.cn/Article/details/gwouanehf.sHtML

$obj?->method()
来源：http://m.share.vehdjk.com/Article/details/gugezmryk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gysslhvbw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/gtfcukxrs.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gryyabseb.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gjctqovmc.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/glbuzxhrp.sHtML

"值: {$a}"
来源：http://www.share.yfazqb.com/Article/details/gbvxhwsgr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gcgpvntop.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gxjmjtpbn.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/gfsuuwcvu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/graqosnug.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.yfazqb.com/Article/details/guiobcdum.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.tarul.cn/Article/details/gpqnwgpvq.sHtML

[U61] PHP：正则
来源：http://blog.fktsv.cn/Article/details/gzshzbnws.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gtftdimfx.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/guswxagyi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.sjlbkw.cn/Article/details/gxhxqysrb.sHtML

[U63] PHP：文件读写
来源：http://wap.bbcook.cn/Article/details/gadohlfnz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/gztsnijmw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/gysvsmawb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.tarul.cn/Article/details/gehmtjkdx.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gawdkfiqp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.vehdjk.com/Article/details/gzpipumhw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.yfazqb.com/Article/details/gfgbbegpi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.vehdjk.com/Article/details/gwxamahpo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.epnwcf.com/Article/details/gjdetyptj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/gbwkvkngv.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/ggvsboqoy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gmxbanxhv.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/gtqyeertg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.bbcook.cn/Article/details/gspvvdyig.sHtML

[U70] PHP：PDO 事务
来源：http://blog.bbcook.cn/Article/details/gefjfcpae.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.vehdjk.com/Article/details/gfsixxsha.sHtML

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/grzudrrel.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fktsv.cn/Article/details/gpoekwhsw.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.bbcook.cn/Article/details/gdgczaiif.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gqlmhwqrc.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.vehdjk.com/Article/details/gtxzsumdi.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.bbcook.cn/Article/details/gpklkygvq.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gmqdezfhy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.tarul.cn/Article/details/gldpdgjss.sHtML

[U75] PHP：依赖注入
来源：http://3g.yfazqb.com/Article/details/gajxyifqt.sHtML

composer require psr/container
来源：http://3g.bbcook.cn/Article/details/gawddkmne.sHtML

[U76] PHP：简单路由
来源：http://www.blog.vehdjk.com/Article/details/gqdaiorus.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/gyofgeuoi.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.vehdjk.com/Article/details/gtgxfyomr.sHtML

composer require twig/twig
来源：http://blog.tarul.cn/Article/details/giobzgdrg.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gvyhjpbzc.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.vehdjk.com/Article/details/ghgqvleme.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/golvnvlhx.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.yfazqb.com/Article/details/gpqokowli.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/gjdoxzbna.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.bbcook.cn/Article/details/gbvhptolh.sHtML

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/gkmhsxuah.sHtML

npm init -y;  npm i express
来源：http://m.share.bbcook.cn/Article/details/gwsincrfy.sHtML

[U82] JS：package.json 脚本
来源：http://wap.bbcook.cn/Article/details/gtnuscbty.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.epnwcf.com/Article/details/gnaqggdfj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fktsv.cn/Article/details/gggazrcby.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gxgocxfsn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gejhkooke.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.yfazqb.com/Article/details/gjkgdysze.sHtML

[U85] JS：可选链
来源：http://mobile.vehdjk.com/Article/details/gnyjlhjyd.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/gfxklcsmo.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gxprqvfjh.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gminofgxe.sHtML


<!-- 参考信息 -->