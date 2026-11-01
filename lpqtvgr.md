代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://read.share.sjlbkw.cn/Article/details/grxmolojk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gltgnenhy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gsqvvlokt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gdnxplbuo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/googlheig.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggbjnqlue.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gsgbhvyky.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsxezvqzc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/gygurwxoo.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gcnmdjmig.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gohiptcts.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/gllwxmvbr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/goixiruwr.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gwbkxbyrv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gaoiopkmz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gojkashnz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/gygueyfam.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/ggrooblci.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/glkjmpswp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gtxydinjg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/gfthkaklz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/ggflnhzaw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gjsfwcphn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/gwaheswdy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/gpuhdayss.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gsbxveoff.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/gmzjfkoto.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gyesksapr.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/grebifiqb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gfitjkgtm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gfjgpjlbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/grbpsnulr.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gfcsyaqgh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/gzffaxbox.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/ggziddsrp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gionazngv.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gsfjvwktl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gbedrpvut.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/gvfqpbrge.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/godoxzcep.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/gcpxhvxxr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gpltfihfa.sHtML

[T18] Swift：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gtldcnlqg.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gzsmqbsxk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gjmywrvez.sHtML

if let n = opt { print(n) }
来源：http://baike.epnwcf.com/Article/details/gozqixuao.sHtML

[T20] Swift：数组操作
来源：http://3g.bbcook.cn/Article/details/gluffmxgf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gnzlnjiyy.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/ghbxoawbh.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gijjxigpy.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gelehfggx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gdsofixgj.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/ghsmwscdr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/goymecoca.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gvjwfpotm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gatbxrqtn.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gtzdfddkp.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gldctcqku.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gjyozbzlq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.vehdjk.com/Article/details/gkxlwvhvx.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/gzjfvrykc.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/gmonktuby.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gcynjrhpk.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/gxptnknrk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/ghuccdesh.sHtML

guard let x = opt else { return }
来源：http://m.share.yfazqb.com/Article/details/ghftvnevt.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gwmrrvkyn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/ggzpchgaq.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ghtlvdgix.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gwmvowddw.sHtML

[T32] Lua：局部变量
来源：http://3g.sjlbkw.cn/Article/details/gwpzggzof.sHtML

local a = 1
来源：http://www.blog.yfazqb.com/Article/details/gqvoioyvf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.vehdjk.com/Article/details/guvgwliuv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gihsozyat.sHtML

[T34] Lua：遍历表
来源：http://3g.bbcook.cn/Article/details/gjxgjktdb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gfeqtmqst.sHtML

[T35] Lua：字典表
来源：http://wap.sjlbkw.cn/Article/details/gtznmzaxq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/ghgxkakhk.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/gkcuwzvrt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/ggbromogn.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gpkyrtpnt.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gddnpezbs.sHtML

[T38] Lua：条件
来源：http://www.blog.epnwcf.com/Article/details/gzywtafdz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/gjvybjzon.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gqsfrefni.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/glfqfmiec.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gycndilac.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/glwjsqahi.sHtML

[T41] Perl：Hello World
来源：http://wap.vehdjk.com/Article/details/gnpyugpnb.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/gythrcqzu.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbgvzcib.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.epnwcf.com/Article/details/gfzkjvygm.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/ghwqsfizh.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gocyocbeq.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gityyljwy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.sjlbkw.cn/Article/details/ggpaauxzs.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/gbbmjkhot.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.sjlbkw.cn/Article/details/gqawxrewq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/giqehqwyb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/gvdvcwege.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/grpbddork.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/gadiaoknn.sHtML

[T48] Perl：正则替换
来源：http://mobile.vehdjk.com/Article/details/gdwhizesn.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gdglhmwww.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/gjdozulql.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gpwshmgwh.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gqcbaudgl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/givlsuvra.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/grpojhzru.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gqbvwxawo.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/ggkwgykds.sHtML

[T52] Scala：变量
来源：http://wap.yfazqb.com/Article/details/ghsixjibr.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gluqqtxtp.sHtML

[T53] Scala：字符串插值
来源：http://baike.tarul.cn/Article/details/gexphxtjl.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gdsncgvxo.sHtML

[T54] Scala：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gexdskkwh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fktsv.cn/Article/details/gmpbjsrbj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gzcgbkyij.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gqofhejat.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/gxvtqpkjl.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gaoywtkev.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gyapxzwzj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/grfjptpfv.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gspxwdhey.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.vehdjk.com/Article/details/gntprvcyi.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gvpljssnc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/gwqphvrfe.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gjhpexsio.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/gybfvvsbd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwtutsvst.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gwkjavkxi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfnvxdmgb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/ghdvsqaia.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.bbcook.cn/Article/details/glmogdyoj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gsiwtrauu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fktsv.cn/Article/details/ghnmkxvlk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fktsv.cn/Article/details/geziscfnh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/grejqlhnz.sHtML

[U04] Py：变量调试打印
来源：http://blog.yfazqb.com/Article/details/gbmjclpgy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gstlavyag.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gtcvvjecs.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gqkooqkkm.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gdciuvmpy.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gzozszqrg.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/ggxipbgyu.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/gagnofkmb.sHtML

[U08] Py：展平二维列表
来源：http://blog.vehdjk.com/Article/details/gmunzgmik.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/gfkeskkts.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.vehdjk.com/Article/details/gwzkctoox.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gzacdxrge.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/gvebrwqln.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/guxmxkdiy.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gbmqnyowt.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gxixfzmzj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/goyrfijuu.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gjhaoqvyg.sHtML

[U13] Py：固定长度队列
来源：http://3g.fktsv.cn/Article/details/gxiwgzmix.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gunywrqnt.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/gfdfsapux.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gajnoccmg.sHtML

[U15] Py：高精度计时
来源：http://3g.epnwcf.com/Article/details/gomrldndn.sHtML

t = time.perf_counter()
来源：http://mobile.fktsv.cn/Article/details/gcbkqfzyq.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gatucttuh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gvllbqsin.sHtML

[U17] Py：初始化日志
来源：http://wap.yfazqb.com/Article/details/goyafqxoh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/ghlgrnnyt.sHtML

[U18] Py：预编译正则
来源：http://m.share.sjlbkw.cn/Article/details/gzlbzqmxp.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/guapwcgbl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.vehdjk.com/Article/details/ggmsupful.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gtmyzaroc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.yfazqb.com/Article/details/ggsxwlynq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gqmlhvfgq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.bbcook.cn/Article/details/grqoawpmo.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/gdnqnwuon.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.bbcook.cn/Article/details/gbhbxxior.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gruihznjm.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gzdcklivn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.vehdjk.com/Article/details/gszblphbh.sHtML

[U24] Py：路径操作
来源：http://wap.fktsv.cn/Article/details/gmqclhjml.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gimgofrxv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/grtwdmqse.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gcxlqaxpe.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fktsv.cn/Article/details/gyhdltfxa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.vehdjk.com/Article/details/gsggqyrza.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/gtfygcwum.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.epnwcf.com/Article/details/gyrzakozu.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/gkxyldhal.sHtML

UserId = int
来源：http://www.m.share.vehdjk.com/Article/details/gntmwcdvl.sHtML

[U29] Py：属性校验
来源：http://blog.fktsv.cn/Article/details/grdvixfqj.sHtML

@property 与 @x.setter 配合
来源：http://blog.vehdjk.com/Article/details/gbydqnbds.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/gnhtgyjgh.sHtML

@dataclass(slots=True)
来源：http://baike.yfazqb.com/Article/details/gmdoiqtqz.sHtML

[U31] Py：单测
来源：http://baike.bbcook.cn/Article/details/ghhskajjf.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gdnirhwku.sHtML

[U32] Py：代码格式化
来源：http://baike.fktsv.cn/Article/details/ggjchewze.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.vehdjk.com/Article/details/glmtxwrwv.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gnvlqvxek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.tarul.cn/Article/details/guxrcjgat.sHtML

[U34] Py：判断编码
来源：http://mobile.yfazqb.com/Article/details/glmnzyasp.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/gfkzyvufa.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gswcrwwkq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gurhgevoy.sHtML

[U36] Py：定时任务
来源：http://www.m.share.vehdjk.com/Article/details/ghpmajyvt.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.yfazqb.com/Article/details/gkzkkjxsw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.vehdjk.com/Article/details/gadnnqyhz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/gxhcumnmm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fktsv.cn/Article/details/gataznadn.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuwikdiz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/ggzkapimi.sHtML

sys.stdout.isatty()
来源：http://3g.yfazqb.com/Article/details/guhpbobnk.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gwsvliwjg.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/guncffdso.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gltkcrccg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gcirmhogz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/goaxmqnuz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gqqpxwgin.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gkazjogzp.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/glmvvogro.sHtML

[U44] PHP：开启严格类型
来源：http://3g.tarul.cn/Article/details/gxpveymqg.sHtML

declare(strict_types=1);
来源：http://3g.tarul.cn/Article/details/gbhoxvdim.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.epnwcf.com/Article/details/grjnjiomx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gdchaarjo.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gxpurgqqf.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/gnzoexsnr.sHtML

[U47] PHP：联合类型
来源：http://www.share.epnwcf.com/Article/details/gatuspiqq.sHtML

int|string $id
来源：http://www.blog.vehdjk.com/Article/details/gzrcotaoz.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gizlnquoq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gzmhugeza.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/gzgooaudx.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gktwrwpxv.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fktsv.cn/Article/details/gtsunnpny.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/gltzlxpkq.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gstetqxvd.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gdfwswebv.sHtML

[U52] PHP：箭头函数
来源：http://3g.bbcook.cn/Article/details/gsdjbytlp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.yfazqb.com/Article/details/gtstiodgc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.yfazqb.com/Article/details/gyjdsczdt.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/ggdhndtiu.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/grcsbjkqq.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gpgrhobgl.sHtML

[U55] PHP：match 表达式
来源：http://wap.vehdjk.com/Article/details/gxkskcfex.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gwlrhazyh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fktsv.cn/Article/details/gnrkrlwhb.sHtML

f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gpslcwjhu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gzarabiqd.sHtML

"值: {$a}"
来源：http://www.share.tarul.cn/Article/details/gqjmrjies.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gdvzdbmin.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.tarul.cn/Article/details/giggfocyx.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gykuukwzf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/ghimkrube.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.epnwcf.com/Article/details/gagydiljt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gnmwaqxdo.sHtML

[U61] PHP：正则
来源：http://read.share.sjlbkw.cn/Article/details/gdxwkvjqa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/grxfzypnl.sHtML

[U62] PHP：日期对象
来源：http://blog.fktsv.cn/Article/details/gupxzrcgw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.yfazqb.com/Article/details/garnkzlib.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/gcuxmwdie.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.sjlbkw.cn/Article/details/gpfqurgtj.sHtML

[U64] PHP：目录遍历
来源：http://3g.fktsv.cn/Article/details/grieuxajs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.vehdjk.com/Article/details/glmbhryti.sHtML

[U65] PHP：会话
来源：http://www.blog.sjlbkw.cn/Article/details/ggweiyney.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.tarul.cn/Article/details/gidqsbjey.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.tarul.cn/Article/details/glnvcnmxb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.vehdjk.com/Article/details/gudpalkqj.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/glvktsftq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/grwtrgcyi.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.tarul.cn/Article/details/guqafpjdl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.yfazqb.com/Article/details/guhtdhmxv.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.bbcook.cn/Article/details/gydikbwwh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/gubgdnlsl.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fktsv.cn/Article/details/gknhzzlkn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.bbcook.cn/Article/details/ggbrughed.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fktsv.cn/Article/details/gsvcgrflb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gkalrftlj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/gtlvmnaji.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/grozhwogx.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.yfazqb.com/Article/details/gldqbmogt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/gvpipgvln.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/gnytlhhok.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.bbcook.cn/Article/details/ghlpskyzb.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/gsspxariz.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/gdamypzft.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/guztjqbjz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.epnwcf.com/Article/details/gmsurbhra.sHtML

[U77] PHP：模板渲染
来源：http://wap.tarul.cn/Article/details/gwpfombsr.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/glkqnfsvd.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyeogntb.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.vehdjk.com/Article/details/gpekedgoe.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/guysglqql.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.sjlbkw.cn/Article/details/grkjosnjv.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gcqunluaf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gzxpohjuz.sHtML

[U81] JS：初始化项目
来源：http://blog.tarul.cn/Article/details/gupunsmry.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/gpiqkbdof.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gdwlrbkpo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.epnwcf.com/Article/details/gzugsbosv.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gpsbhpbie.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gqgayqdfv.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/guekqtofi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/gfkosbcvj.sHtML


<!-- 参考信息 -->