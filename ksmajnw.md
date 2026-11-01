代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gwcevpcdx.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gyxhdwvkp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/giqwkgetf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/gyrtzlrkc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.vehdjk.com/Article/details/gccovenrv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxhckjvcq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/geuxfdusr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmbllqyzr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gdmefzjkk.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gyjxmjtlv.sHtML

[T02] Kotlin：变量
来源：http://mobile.bbcook.cn/Article/details/godeaabcq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gqstvjwpd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gdyiwvxnk.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/govmjuwbz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.yfazqb.com/Article/details/grmvcmmzc.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/gqvudhisr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gtfgawaeg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gwxatelek.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/gxlmsbimm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gwnzlthet.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gchmjavku.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gmtuumkwg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gqjxcdouv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gxapxnmqv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gachvkxbz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/gbtgcydkt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gluxptuqn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gtubgmyde.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/gtdqidtic.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/guyvhencw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gbvznaqwk.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gvfzatkuy.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gutslrdqm.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gmicibiak.sHtML

[T14] Kotlin：循环
来源：http://baike.epnwcf.com/Article/details/gqulqomfc.sHtML

for (i in 1..10) println(i)
来源：http://wap.vehdjk.com/Article/details/gmsvkrflc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gewyaqctf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gxqbhrlgg.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gnezxicix.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/grvsljpsd.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/gkpddwgfr.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/gwrgdjxjv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gfizaibrj.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gincszahp.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gnxznrign.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/guascwdzu.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/goqtplnvq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/grjrmbkqc.sHtML

[T21] Swift：遍历
来源：http://mobile.epnwcf.com/Article/details/gzpgefacn.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/gkdavfccy.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/gqjercjds.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gouyxxchi.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/ghevbcwwk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.yfazqb.com/Article/details/gkqltyghz.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/gmkjgyqwt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gzktmypuj.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/gptxpjxxd.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gbxqumegh.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gcxypcfko.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gccrpeoai.sHtML

[T27] Swift：错误处理
来源：http://mobile.bbcook.cn/Article/details/gpahernvs.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/grxtxwnut.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/godprbhym.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gvjwstlrq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gjdjblumn.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gguynusid.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/gzwygzbtu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gxrsdqfcm.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gbaohlaou.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/giidzhnpk.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gydorfwbm.sHtML

local a = 1
来源：http://read.share.epnwcf.com/Article/details/gmjmvvday.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gmstauccs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/gisoegtfk.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/gkgccnyam.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/gzoscvtha.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/ggzjzcyyw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gvmtvukuz.sHtML

[T36] Lua：函数
来源：http://blog.epnwcf.com/Article/details/gsnmbkbbe.sHtML

function add(a, b) return a + b end
来源：http://baike.fktsv.cn/Article/details/gililpjlb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gxlphfuhe.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gcmlgkgma.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gankxekuz.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gxowtuhwp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gdadjncig.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/guhsbogxc.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gjwrqadcu.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fktsv.cn/Article/details/gcmlmbjjd.sHtML

[T41] Perl：Hello World
来源：http://mobile.epnwcf.com/Article/details/gnpmunzlm.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gznijbfha.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gvnmstznr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.yfazqb.com/Article/details/gjzpgazpz.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gjsrgvgly.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/ggetzvdol.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/gzfzirdke.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.sjlbkw.cn/Article/details/gspgomayh.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gzslaqirm.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/gxukpsfsq.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gjaitctio.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gyxzxdewl.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.yfazqb.com/Article/details/gvdozckqo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gddnqaaqs.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/gkieactry.sHtML

$s =~ s/old/new/g;
来源：http://blog.epnwcf.com/Article/details/gybntzigp.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gmrsuedzu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gownpjbtr.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gpwgdaxsh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.sjlbkw.cn/Article/details/gxyqohvec.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.vehdjk.com/Article/details/gnsiibhkm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gpxwxgfph.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gfkqsxqgp.sHtML

[T52] Scala：变量
来源：http://read.share.tarul.cn/Article/details/goukcvkhp.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/gudymhpun.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gxwsjilfx.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/guxcscixl.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gdikwddjz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gdgofvkkz.sHtML

[T55] Scala：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gtgqgtnel.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/gskgijtwx.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/gntsbuetz.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gianyrzmo.sHtML

[T57] Scala：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gdrkltrjw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fktsv.cn/Article/details/gubngluyd.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/gtzzdedqu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/grvovzjgp.sHtML

[T59] Scala：循环
来源：http://mobile.fktsv.cn/Article/details/gajhtbhfq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gydlyrsxs.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gnilytpbh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gcpmcecve.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjactfzwl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/ggixvdqpk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gscysioop.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/gztriwbis.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.bbcook.cn/Article/details/gdonqlooj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.yfazqb.com/Article/details/gupzkvyga.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/gvlsgfvhr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gglkipufq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/giauggjgs.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/ggedfxnty.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.yfazqb.com/Article/details/gietshwvm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gpsiuftfn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gavbshqeq.sHtML

[U06] Py：合并两个字典
来源：http://baike.yfazqb.com/Article/details/garctoqib.sHtML

{**a, **b}
来源：http://read.share.vehdjk.com/Article/details/gebnrmemi.sHtML

[U07] Py：反转字典键值
来源：http://www.share.vehdjk.com/Article/details/gledgwahu.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gvwwcdafq.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/gkiynvnvk.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gqtmxlvvj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/govrynyrc.sHtML

max(d, key=d.get)
来源：http://wap.bbcook.cn/Article/details/gzbpjlmtu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.sjlbkw.cn/Article/details/gjsefwmgv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/gclhimaho.sHtML

[U11] Py：生成器表达式
来源：http://read.share.vehdjk.com/Article/details/gfttupbnp.sHtML

(x * 2 for x in arr)
来源：http://read.share.fktsv.cn/Article/details/gxflqxbek.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.bbcook.cn/Article/details/geagphkcd.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gsfhzkbaa.sHtML

[U13] Py：固定长度队列
来源：http://wap.sjlbkw.cn/Article/details/gzxgdmotu.sHtML

deque(maxlen=10)
来源：http://baike.bbcook.cn/Article/details/gewckoybc.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.epnwcf.com/Article/details/gkcudayeh.sHtML

defaultdict(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gawmnqvzo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/gbqoyylxq.sHtML

t = time.perf_counter()
来源：http://www.blog.sjlbkw.cn/Article/details/gdbyriyaz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.yfazqb.com/Article/details/gqohcgulf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/gzytjftnl.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gvblxwxtu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.tarul.cn/Article/details/ggryhmxyr.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.vehdjk.com/Article/details/grfljqcru.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/groiryquy.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gdiuwomhz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.vehdjk.com/Article/details/gwegpuvvl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fktsv.cn/Article/details/gupwqcrup.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gdlxnqhfm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/ghnismvwp.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/gmxdrzuxn.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/grigpcgls.sHtML

list(zip(*m))
来源：http://baike.tarul.cn/Article/details/gjzlqxysu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gjlfqazks.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/gcgidbvpa.sHtML

[U24] Py：路径操作
来源：http://www.blog.tarul.cn/Article/details/ghdvjccov.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gdbwrxdkv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.sjlbkw.cn/Article/details/gbcmpdlmo.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gsbmfrezs.sHtML

[U26] Py：并发下载
来源：http://www.blog.tarul.cn/Article/details/gnlehjjgy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.bbcook.cn/Article/details/gjaglbqxp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.epnwcf.com/Article/details/gtugvnrph.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/gdsmgpcno.sHtML

[U28] Py：类型别名
来源：http://3g.epnwcf.com/Article/details/gdjjwivis.sHtML

UserId = int
来源：http://www.share.bbcook.cn/Article/details/gvhbmkzpm.sHtML

[U29] Py：属性校验
来源：http://3g.tarul.cn/Article/details/gxxfqeddf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fktsv.cn/Article/details/gyckettsr.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gvmgzrwkn.sHtML

@dataclass(slots=True)
来源：http://3g.sjlbkw.cn/Article/details/gnxesfiux.sHtML

[U31] Py：单测
来源：http://mobile.sjlbkw.cn/Article/details/gedbkgeej.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gcitbyncc.sHtML

[U32] Py：代码格式化
来源：http://wap.bbcook.cn/Article/details/gqtbikylg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/ghqzgybef.sHtML

[U33] Py：打包发布
来源：http://read.share.yfazqb.com/Article/details/gyevopmfs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.bbcook.cn/Article/details/grxoaylge.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gvalsoxvo.sHtML

chardet.detect(raw)
来源：http://mobile.yfazqb.com/Article/details/gmjgttheu.sHtML

[U35] Py：发送邮件
来源：http://www.share.bbcook.cn/Article/details/govrfwfdm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/gjsmlejqa.sHtML

[U36] Py：定时任务
来源：http://3g.tarul.cn/Article/details/gtrgjimjw.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gkgsjjvhk.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/gkkarfhkg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gzwcrojve.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/gjspgqniy.sHtML

Path(__file__).resolve().parent
来源：http://blog.epnwcf.com/Article/details/gomhofvlg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/gcvrbkvkc.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/geagwrthx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gddlhcobd.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/guvlqgxci.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.yfazqb.com/Article/details/gvppoymbb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fktsv.cn/Article/details/gtbieobog.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/ginoyuyzk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gjeagrbzc.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fktsv.cn/Article/details/gpexbyhdv.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gzunwyyqp.sHtML

[U44] PHP：开启严格类型
来源：http://blog.bbcook.cn/Article/details/gkemjvncf.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/gvxzknapj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/gkogiosiv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gvcvshbgp.sHtML

[U46] PHP：可空类型
来源：http://baike.bbcook.cn/Article/details/goadrojwn.sHtML

?string $name = null
来源：http://m.share.bbcook.cn/Article/details/gavmotwot.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gqnlasric.sHtML

int|string $id
来源：http://read.share.yfazqb.com/Article/details/gbiafzdkd.sHtML

[U48] PHP：纯枚举
来源：http://read.share.yfazqb.com/Article/details/gfpuhutzh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fktsv.cn/Article/details/gnntjukge.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/giqbxpufd.sHtML

public readonly string $name
来源：http://mobile.bbcook.cn/Article/details/gdkvoclsz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/gyrsyrmxw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/gtzhzjnin.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gushutqvn.sHtML

[$a, $b] = $arr;
来源：http://blog.epnwcf.com/Article/details/gfwizrqpv.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gwhtxkjnr.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.tarul.cn/Article/details/gnzfkrtxy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gxrrmtarf.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.epnwcf.com/Article/details/gxcqrcoln.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/gmdrcuxpb.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gijzxodoi.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gtjuybmgw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.tarul.cn/Article/details/ghqmnktrz.sHtML

[U56] PHP：命名参数
来源：http://mobile.vehdjk.com/Article/details/geiaehkfo.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gsqbzjyzf.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/ghotfqzhd.sHtML

"值: {$a}"
来源：http://www.blog.sjlbkw.cn/Article/details/gcnhfypoz.sHtML

[U58] PHP：数组三件套
来源：http://wap.tarul.cn/Article/details/gfmvknbae.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.vehdjk.com/Article/details/gajzviufy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.tarul.cn/Article/details/gdoetwyyo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gufgobwkd.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fktsv.cn/Article/details/gvibmmvrq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.vehdjk.com/Article/details/ghlbxrddb.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/ggnafxbsk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gergebeji.sHtML

[U62] PHP：日期对象
来源：http://www.blog.bbcook.cn/Article/details/giivhtbly.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.tarul.cn/Article/details/gazrioilc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/glncxkfeb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.sjlbkw.cn/Article/details/gshhwnjtc.sHtML

[U64] PHP：目录遍历
来源：http://mobile.vehdjk.com/Article/details/gixcpoude.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/grvkvfcnn.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/glunglzsv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gmxameljs.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/gwykgupfx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.bbcook.cn/Article/details/gfgbxskqd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/godhhvclq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.vehdjk.com/Article/details/gotbpaesy.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/ggddwdfro.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.vehdjk.com/Article/details/gmsrosvyl.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.tarul.cn/Article/details/gonnvsfoh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.bbcook.cn/Article/details/gtowhrcyj.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/gipcxsyac.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.bbcook.cn/Article/details/gckhtejkz.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/gbjopwerq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.vehdjk.com/Article/details/gwsrmhodw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gxcdfbind.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.sjlbkw.cn/Article/details/gqidteyns.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.vehdjk.com/Article/details/gwatwulxc.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gnsshomlm.sHtML

[U74] PHP：读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gjlqwrphf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gkkrusmpp.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.bbcook.cn/Article/details/gtttuvkqd.sHtML

composer require psr/container
来源：http://3g.tarul.cn/Article/details/gqlqwbfap.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.yfazqb.com/Article/details/guogvwxtt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fktsv.cn/Article/details/gbndtkwfs.sHtML

[U77] PHP：模板渲染
来源：http://blog.tarul.cn/Article/details/gwxrdhoti.sHtML

composer require twig/twig
来源：http://3g.yfazqb.com/Article/details/ggagmlucw.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/gcymxbpsw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/guofbndbf.sHtML

[U79] PHP：静态分析
来源：http://www.blog.tarul.cn/Article/details/grusztjef.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/ghlatenzs.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.yfazqb.com/Article/details/gwihwaxus.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.sjlbkw.cn/Article/details/gwyhiwyas.sHtML

[U81] JS：初始化项目
来源：http://baike.epnwcf.com/Article/details/gvcdexrao.sHtML

npm init -y;  npm i express
来源：http://baike.vehdjk.com/Article/details/gemxophyv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.yfazqb.com/Article/details/ggwuygora.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.epnwcf.com/Article/details/gokqjphzw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.sjlbkw.cn/Article/details/gayqpvpwx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gtwsduzps.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/gzfgwbfrw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.vehdjk.com/Article/details/grdmgtzzx.sHtML


<!-- 参考信息 -->