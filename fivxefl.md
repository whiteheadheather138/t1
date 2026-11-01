代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gkacrdgfz.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gypvidhpv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/grymzqcix.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/ggntcgaxn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gqejnulai.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvwridhfu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gugedqlij.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvaznyxjz.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/grdwbwuii.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gfuqmwnhw.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gfwqbbkpn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/guhijokab.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.vehdjk.com/Article/details/gyqrnxfsg.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/glbirxmog.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gqrfyfiee.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/gysrpxbra.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/glxsqlzgf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.sjlbkw.cn/Article/details/gwpfdtina.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gqbyuojre.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gopzedwdw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gwotqijpi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.yfazqb.com/Article/details/gbjgcrlke.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gumudsxut.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gsnxykism.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.bbcook.cn/Article/details/gkrijukhp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.vehdjk.com/Article/details/grleofbdr.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gridifwqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gehxiejwe.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/gwkswwqpy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gaovnhpve.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.bbcook.cn/Article/details/gqemnjxoe.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.yfazqb.com/Article/details/grydfmamg.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gnplmmsos.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gtviszwht.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fktsv.cn/Article/details/gesjfhqlz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gjxuitqpq.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/ggsmssrxt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/gtvzykzwa.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gtoypxzmv.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/glaqeaoom.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/ghxtcgnqr.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/ggqonmcdo.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gawakwqpw.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/ginjquixw.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gnowhommx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gewmavhkd.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gptpqzlxc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gmcbpqkgs.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gcecjcrok.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/gjdroqfjm.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gsqwgstit.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/ggnvohirn.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/ggginltbx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/gxaorqjcf.sHtML

[T24] Swift：闭包
来源：http://www.share.vehdjk.com/Article/details/ggopvohly.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gxtphtzzk.sHtML

[T25] Swift：结构体
来源：http://www.blog.yfazqb.com/Article/details/gzqumbbhg.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gpqptaojg.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/gofekjuyy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gspopiqyk.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/glwjgwpzp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/gylhbdrvq.sHtML

[T28] Swift：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gkxuiwtkb.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gchskgnqt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gzkwkbkij.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gddkperyd.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gumhpifza.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gwzjzcgat.sHtML

[T31] Lua：Hello World
来源：http://wap.epnwcf.com/Article/details/gmmbybrgs.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gdhajljih.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/gagxwtvxb.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/gyxseqdqi.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gqjwaokue.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gkxgnovqa.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/gzrhvcaoa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gvzvtgmnh.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gquidjbts.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gpmsrxxak.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gohbjdhej.sHtML

function add(a, b) return a + b end
来源：http://read.share.bbcook.cn/Article/details/gijzryxuv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gvpnynija.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gljaxxoua.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/garxrmxhk.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/goktsvloq.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/grleugftf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrkqosnm.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gkazcjpmo.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/gxilfylyy.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gafnpijqm.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/ggsfnjoop.sHtML

[T42] Perl：变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gpgrsoncb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fktsv.cn/Article/details/gujqtmrwt.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gqnoglyya.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/grmzquwgo.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/gxrkenuqp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/grbdzifbt.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.bbcook.cn/Article/details/gvuzrrbfe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gqaghbnmw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/ghgwiliuf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/gsowdkqud.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gjkvackbh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gmvyfddbh.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/gzhjvgusz.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gtoeizgui.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/glpsedxmv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gdpxsdzrh.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/ghfyqfbew.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/gqohbxoos.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.yfazqb.com/Article/details/giwzfgtuh.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gfrwzvflv.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/ghcvfplbg.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/gxvepbxni.sHtML

val a = 1;  var b = 2
来源：http://www.share.bbcook.cn/Article/details/gfekjkxjf.sHtML

[T53] Scala：字符串插值
来源：http://baike.tarul.cn/Article/details/gkvwjteae.sHtML

s"值: $b"
来源：http://m.share.tarul.cn/Article/details/gyaehfoar.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/giiadbjru.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.sjlbkw.cn/Article/details/ghglbgahl.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gurowcqto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gseeymsue.sHtML

[T56] Scala：样例类
来源：http://m.share.vehdjk.com/Article/details/gtuercvje.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/gqpdkziku.sHtML

[T57] Scala：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gacnqpgkb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/gyuednpjd.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/ghveeepim.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/guafwlnlp.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/glkfklgeo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gctqdqjud.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/gpeblaojs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/gyqyadoxl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gorcabtct.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gdbfwwlxs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqhtovnkd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/gjznxwbxl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.bbcook.cn/Article/details/gavvnubdp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/gvqdqdgbo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.yfazqb.com/Article/details/gzzhfkihn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/gndnerqhl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fktsv.cn/Article/details/gjeplzdjv.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/glrnouqlc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fktsv.cn/Article/details/gqxbqflon.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.bbcook.cn/Article/details/ghorymiit.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gtqotohgb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/gpqyqbetn.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gojwlyiqn.sHtML

[U07] Py：反转字典键值
来源：http://3g.yfazqb.com/Article/details/gnofblbfu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhwtdzxr.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gbkyypvhk.sHtML

[y for x in nested for y in x]
来源：http://mobile.fktsv.cn/Article/details/gudrgkqcv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.bbcook.cn/Article/details/glzksoiwr.sHtML

max(d, key=d.get)
来源：http://www.share.vehdjk.com/Article/details/ggfkypgfb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gviomrvxe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/gyajhzqai.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gbwwjkltk.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/ggkgqtzzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgbbdxxd.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/grvmqtbiy.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gtuagmxgz.sHtML

deque(maxlen=10)
来源：http://www.share.yfazqb.com/Article/details/gqkhpvazi.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gjdbfsvna.sHtML

defaultdict(list)
来源：http://mobile.epnwcf.com/Article/details/gscycarjg.sHtML

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/gxfdzbkai.sHtML

t = time.perf_counter()
来源：http://m.share.sjlbkw.cn/Article/details/gxcvzvpzr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.vehdjk.com/Article/details/gwbrpwaaw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/glhfabigv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.epnwcf.com/Article/details/glvrrzrir.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.sjlbkw.cn/Article/details/gnwgkyyvv.sHtML

[U18] Py：预编译正则
来源：http://read.share.yfazqb.com/Article/details/gozlpfifw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/guneeqaik.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/glrnqwjzb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.tarul.cn/Article/details/gwvluqqsh.sHtML

[U20] Py：缓存函数结果
来源：http://blog.bbcook.cn/Article/details/gitkgcums.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.epnwcf.com/Article/details/gpsxelqgz.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.bbcook.cn/Article/details/gyrheiiqw.sHtML

@contextlib.contextmanager
来源：http://3g.bbcook.cn/Article/details/gwuddqdgp.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gjnexwlec.sHtML

list(zip(*m))
来源：http://read.share.tarul.cn/Article/details/gzaefoavk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fktsv.cn/Article/details/gfzvftenq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gogqkblzg.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/gkrecggde.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/ghrtdisvu.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.tarul.cn/Article/details/gcsykbjnv.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/gmhsycwwm.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/gssxikgjb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/glutzjtin.sHtML

[U27] Py：异步 HTTP
来源：http://blog.vehdjk.com/Article/details/gyvbyhjqo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/gqwapzddw.sHtML

[U28] Py：类型别名
来源：http://m.share.vehdjk.com/Article/details/gkhidtuai.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/gqrgozgis.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/geghraxym.sHtML

@property 与 @x.setter 配合
来源：http://blog.epnwcf.com/Article/details/ghhswmwei.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gpoufndzt.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gudpwjfxw.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/gxjxhgfgj.sHtML

python -m pytest -q
来源：http://www.m.share.yfazqb.com/Article/details/gnqsbbgiy.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/glxhrwgzl.sHtML

ruff format . && ruff check --fix .
来源：http://baike.sjlbkw.cn/Article/details/gvpgapwdh.sHtML

[U33] Py：打包发布
来源：http://3g.bbcook.cn/Article/details/gxpgymtms.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gvagsbdwd.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/ggmezoccb.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gmgtehbey.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/gogpzyvef.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/ghdagtcfc.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/ggcxslzxb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gbbdofaus.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/ggdonkldx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gzdglctzm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.vehdjk.com/Article/details/gbwjszzjo.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gesdqqjdl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/gcjfkpozf.sHtML

sys.stdout.isatty()
来源：http://blog.epnwcf.com/Article/details/glgmgzvsw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.epnwcf.com/Article/details/gthfmmxfj.sHtML

print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gdaacvniu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/grrjneqqg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.tarul.cn/Article/details/gbpoyzphe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.vehdjk.com/Article/details/gxspngshg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/gukjzibjo.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gazmbldku.sHtML

namespace App\Http;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyjdixwo.sHtML

[U44] PHP：开启严格类型
来源：http://blog.yfazqb.com/Article/details/gadhaizsh.sHtML

declare(strict_types=1);
来源：http://3g.fktsv.cn/Article/details/gbkwzhzgj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.vehdjk.com/Article/details/gffknobzp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gpsahbruz.sHtML

[U46] PHP：可空类型
来源：http://wap.sjlbkw.cn/Article/details/gaifmblkm.sHtML

?string $name = null
来源：http://www.m.share.bbcook.cn/Article/details/gplnrongv.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/ggzrgpeiw.sHtML

int|string $id
来源：http://baike.tarul.cn/Article/details/gackpxkmw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.epnwcf.com/Article/details/glzdudtae.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fktsv.cn/Article/details/ghdgibxqk.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/gueslsmhg.sHtML

public readonly string $name
来源：http://wap.fktsv.cn/Article/details/ghadzvmll.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.vehdjk.com/Article/details/gfoupfmpu.sHtML

public function __construct(private int $id) {}
来源：http://wap.fktsv.cn/Article/details/gnxyondki.sHtML

[U51] PHP：数组解构
来源：http://www.blog.yfazqb.com/Article/details/gpljmcxuh.sHtML

[$a, $b] = $arr;
来源：http://wap.tarul.cn/Article/details/gupcgolot.sHtML

[U52] PHP：箭头函数
来源：http://baike.yfazqb.com/Article/details/gkjrnnjhm.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gfjgoinke.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.bbcook.cn/Article/details/gzqgrinfv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.vehdjk.com/Article/details/gzbzuuafy.sHtML

[U54] PHP：空安全调用
来源：http://wap.vehdjk.com/Article/details/gdszvnhie.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gjxqhrnxf.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/gemgqtxdu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gtxvbfbjz.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gjvvtcmuz.sHtML

f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gdoremisp.sHtML

[U57] PHP：字符串插值
来源：http://wap.tarul.cn/Article/details/gtzewatrr.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/gzugylong.sHtML

[U58] PHP：数组三件套
来源：http://3g.bbcook.cn/Article/details/gocasqmxc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.epnwcf.com/Article/details/gtehmoiny.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gokrckeij.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/grksegmka.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/ggeiwelnj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gendqwwua.sHtML

[U61] PHP：正则
来源：http://wap.epnwcf.com/Article/details/gqmxuimnf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gdfhjwpyq.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gjkcjhdyj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.vehdjk.com/Article/details/ggqkyhpgd.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/gznzymkbj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gepcwddgz.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gxmhphkbr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/gcbmxnuif.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/giyorvnlh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/gwrgqvimj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fktsv.cn/Article/details/gyjjntnbn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/godxgkkzs.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gibdntnou.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/gjutrgarg.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gozhsbtxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gdujuenel.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/gotsaxvpz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gbkilhiyg.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gddttoxfr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gzokdbywc.sHtML

[U71] PHP：抛出异常
来源：http://3g.bbcook.cn/Article/details/ghzvxaavp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gbirrojsi.sHtML

[U72] PHP：写错误日志
来源：http://blog.fktsv.cn/Article/details/gnubvevmr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.bbcook.cn/Article/details/gdswghnyp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gxsuurkpb.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.tarul.cn/Article/details/gcpplnquc.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gujddhfol.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/gfierfgpk.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/gvonnelvz.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/ggvelaehf.sHtML

[U76] PHP：简单路由
来源：http://www.share.yfazqb.com/Article/details/gvhugetlj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/gkdgzueau.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.sjlbkw.cn/Article/details/glfreyjuy.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/gcancfecp.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gwmzeapkg.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gpmicrkse.sHtML

[U79] PHP：静态分析
来源：http://www.share.vehdjk.com/Article/details/gwueerxle.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.yfazqb.com/Article/details/grmhdqunu.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/getponahv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/gmvnegirr.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gdzpdjjgf.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gxnivlvqf.sHtML

[U82] JS：package.json 脚本
来源：http://blog.yfazqb.com/Article/details/guvqmldxj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gxcxjwjff.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.epnwcf.com/Article/details/gulekydlq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.tarul.cn/Article/details/gsdsifgeu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.yfazqb.com/Article/details/gvxyovsys.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fktsv.cn/Article/details/guogvjmre.sHtML


<!-- 参考信息 -->