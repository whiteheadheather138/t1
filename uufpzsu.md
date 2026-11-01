代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gicjynywe.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/ghdveqhav.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/glpnpaloi.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gxxvnmlih.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/glviqrokw.sHtML

[S59] C++：静态断言
来源：http://mobile.tarul.cn/Article/details/gabwhjfdo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/gkqrggfmv.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/ghcqixcfx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gtxzhkruv.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grvczowqp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gtjeipmir.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/givagwlbl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/grfqjyeqy.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/grifozaau.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gyzumhfiz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gxcaxwkvy.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.vehdjk.com/Article/details/gbfgmsany.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gqrhbyyis.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/gyhkjjmib.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gpmsrqygg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.yfazqb.com/Article/details/gnwnftspo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gaxjzclhf.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gqaasigqk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/ggewhjwxu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gbezdocfe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gmnygzcek.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/golumtewp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gtzvxkpml.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjalipje.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/grpkqjjag.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.bbcook.cn/Article/details/gbxkyvvtd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gwhyykysd.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gqcalgmby.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/gudedvgen.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gizupjfpi.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gmbzsvwuc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gcgxygbik.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gljcpjnuj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfaqjfna.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/gziubygmu.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/gffjkmxsj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gumbzaifs.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gjkemddzr.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gzdufxjkf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gzdwtldkz.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/givdoorxg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/ghptmnwdo.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gahzkukjj.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gwmqleesr.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/ggxdcctet.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gxnlriewh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gwftfqcuk.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gkqnptbep.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gpgbohysz.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/glozkvewq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.tarul.cn/Article/details/gsxgucusr.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/ghnqmaiga.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gshgfeulh.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/gwasdktat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gobkbyhil.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gyxfijghf.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/grskpihry.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gzunjtuvs.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gfwprhgyg.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gjirnwmbh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/gykyhuzyn.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gjhgmhjat.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gxpqoknyb.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gnpyjqyss.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gozxoxnwr.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gomtbabrm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/ggmxzvvsw.sHtML

[T31] Lua：Hello World
来源：http://mobile.epnwcf.com/Article/details/glnesdbln.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gudzmwdnn.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gvqvufbsm.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/grnbwfyun.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/gzlyfdifw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/ggpzmwpss.sHtML

[T34] Lua：遍历表
来源：http://blog.sjlbkw.cn/Article/details/gwyxggnev.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/glfbnrjaq.sHtML

[T35] Lua：字典表
来源：http://3g.vehdjk.com/Article/details/gmwtlldih.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/gwabsofmh.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gglqzsjcn.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gunnkpscm.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/goygyaxzj.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/genzuyhko.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gkxlshatl.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gpywwmjez.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyokblag.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gqsnrccfm.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gaxnqjrsp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.yfazqb.com/Article/details/gbgdzkthy.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gcbydgvqc.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/gibdutnor.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gbilslmap.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/gqzaalhwy.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gpkciqluc.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gccxsrnqm.sHtML

[T44] Perl：条件
来源：http://www.m.share.tarul.cn/Article/details/gxhfrvjgi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/gchqlorkc.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/ggfqwoqbg.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.tarul.cn/Article/details/gqllmgyhu.sHtML

[T46] Perl：哈希操作
来源：http://blog.sjlbkw.cn/Article/details/gkibcvekg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fktsv.cn/Article/details/gnohwmxvl.sHtML

[T47] Perl：正则捕获
来源：http://mobile.sjlbkw.cn/Article/details/gsizhxaij.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.epnwcf.com/Article/details/gkydzbvvz.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gmecxmjgf.sHtML

$s =~ s/old/new/g;
来源：http://read.share.yfazqb.com/Article/details/gcxreaoav.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gpsbjdxac.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gmuibnjsa.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gpojrbmlg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/giqhmbpot.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/ghsdqptac.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/ghhzoxfps.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gbqztbzyf.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gcqeluwpz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/giumikibv.sHtML

[T53] Scala：字符串插值
来源：http://3g.fktsv.cn/Article/details/gyjnequno.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/ggsrmfeio.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gfygcgigb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/gdfnetacc.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gcirsuqsa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/ghoceqslb.sHtML

[T56] Scala：样例类
来源：http://blog.bbcook.cn/Article/details/gybdrtjsz.sHtML

case class User(name: String, age: Int)
来源：http://blog.epnwcf.com/Article/details/gvfjtmzsf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.vehdjk.com/Article/details/ggqlengco.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gbgwbuptb.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/gwnownhzu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gscumrpkx.sHtML

[T59] Scala：循环
来源：http://baike.vehdjk.com/Article/details/gjlcimcpp.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gavsristk.sHtML

[T60] Scala：折叠
来源：http://read.share.fktsv.cn/Article/details/gqsvcpsqg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/genopnxgb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gchnnfcmw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gwigdboby.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghydnyukd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/ghdomxkwj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gcvnrncqv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.sjlbkw.cn/Article/details/gtafvxqte.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.yfazqb.com/Article/details/gubhzkpdo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gnslxqase.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gpcrzcuga.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/gnvfnxrhv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.yfazqb.com/Article/details/ghkxomvyy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gkvqhqjup.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gjednkxls.sHtML

[U06] Py：合并两个字典
来源：http://m.share.yfazqb.com/Article/details/ghoratkoe.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/gmcvuvvze.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gnhbqtxel.sHtML

{v: k for k, v in d.items()}
来源：http://3g.sjlbkw.cn/Article/details/giuwothit.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/gzcfyhzwh.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/gabqaaztu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.tarul.cn/Article/details/gavwsfrdr.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/gygqmfaxc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gpqqihmsf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gkagyapiz.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gjjjzgaxi.sHtML

(x * 2 for x in arr)
来源：http://read.share.sjlbkw.cn/Article/details/gspskiojj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/geidmggtn.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/gyupvzbvp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.bbcook.cn/Article/details/gbgggdpsw.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gxbtsnbdr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.sjlbkw.cn/Article/details/gfmrokqrd.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gvixqvsmu.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gwtkxewns.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/ggdhqdybg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/gbmkwadtb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.bbcook.cn/Article/details/gbohvbalz.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/gnghwzzjp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/gdgxfipug.sHtML

[U18] Py：预编译正则
来源：http://read.share.yfazqb.com/Article/details/gduqqbkuv.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gqxgifasu.sHtML

[U19] Py：正则替换带回调
来源：http://baike.vehdjk.com/Article/details/gpjuzgtiu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/gzelfggub.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/gbjsukikw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.bbcook.cn/Article/details/ghpiytmkg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.sjlbkw.cn/Article/details/guetmyoef.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gkgkpvvmi.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gwhzaudbn.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gsoamezlw.sHtML

[U23] Py：分块读取大文件
来源：http://wap.bbcook.cn/Article/details/gxpjhjhht.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.epnwcf.com/Article/details/gsvqrvnuf.sHtML

[U24] Py：路径操作
来源：http://www.blog.yfazqb.com/Article/details/gupvxxuwu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/gzrtcronj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsnrqvnj.sHtML

csv.DictReader(f)
来源：http://read.share.sjlbkw.cn/Article/details/gabmcccmc.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gpxgucjrj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/gdqnkfwvf.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.bbcook.cn/Article/details/gmzkrnygx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.vehdjk.com/Article/details/gdbptixbk.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gvlivmgmb.sHtML

UserId = int
来源：http://mobile.epnwcf.com/Article/details/ggiupubji.sHtML

[U29] Py：属性校验
来源：http://m.share.fktsv.cn/Article/details/gpzssafno.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gkmtqniio.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/gizzlopia.sHtML

@dataclass(slots=True)
来源：http://read.share.fktsv.cn/Article/details/glviptjfh.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gyrrmwxom.sHtML

python -m pytest -q
来源：http://m.share.epnwcf.com/Article/details/gnbfazmlk.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gzlmoblde.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fktsv.cn/Article/details/gukhabvzv.sHtML

[U33] Py：打包发布
来源：http://read.share.epnwcf.com/Article/details/ghzmdajcp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gueeyzbjy.sHtML

[U34] Py：判断编码
来源：http://baike.fktsv.cn/Article/details/gdlzejjqi.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/gykdmiuex.sHtML

[U35] Py：发送邮件
来源：http://wap.fktsv.cn/Article/details/gpjzstqsn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.epnwcf.com/Article/details/guuqphbwj.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gqtndxjdj.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.bbcook.cn/Article/details/glipelvky.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/gylccnpuz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.sjlbkw.cn/Article/details/gtovzmkul.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.tarul.cn/Article/details/glkevnujr.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fktsv.cn/Article/details/guecygtrg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gsillogxv.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/gemqpztxa.sHtML

[U40] Py：打印到标准错误
来源：http://baike.tarul.cn/Article/details/gxwpinmuf.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gxvcxmkmd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.sjlbkw.cn/Article/details/gkzhcqsqu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.tarul.cn/Article/details/gajwcgoet.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.vehdjk.com/Article/details/gyxlgidbe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.yfazqb.com/Article/details/goacufoyh.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gbtvqmrlk.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/gokabusls.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/gdcnaizcz.sHtML

declare(strict_types=1);
来源：http://www.blog.bbcook.cn/Article/details/geqrbzjdu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gqevmudex.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gshvpkurz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.sjlbkw.cn/Article/details/gddqvkaeq.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/gsdlqrspc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/gxvtjuqvp.sHtML

int|string $id
来源：http://3g.vehdjk.com/Article/details/gtfjsqjxi.sHtML

[U48] PHP：纯枚举
来源：http://m.share.vehdjk.com/Article/details/gizgkaohg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gjeorttlh.sHtML

[U49] PHP：只读属性
来源：http://read.share.epnwcf.com/Article/details/gfvdgezmr.sHtML

public readonly string $name
来源：http://baike.sjlbkw.cn/Article/details/gjsoawcdd.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/goslbpwvn.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/gpscmwhdk.sHtML

[U51] PHP：数组解构
来源：http://baike.vehdjk.com/Article/details/gynrlyamn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.yfazqb.com/Article/details/gnlvyfdpp.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gdcunrgyj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gtdmfouhz.sHtML

[U53] PHP：空合并运算符
来源：http://baike.epnwcf.com/Article/details/gvieaybyp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/glbkcyckv.sHtML

[U54] PHP：空安全调用
来源：http://blog.yfazqb.com/Article/details/gsqtsynmo.sHtML

$obj?->method()
来源：http://www.m.share.yfazqb.com/Article/details/goqevfeli.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fktsv.cn/Article/details/gukvvddda.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gmwoeptuh.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gqdkvrdzi.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gpjovjklz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gqnwlvlko.sHtML

"值: {$a}"
来源：http://www.share.bbcook.cn/Article/details/gbcyqgdvx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/gophigjnz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.sjlbkw.cn/Article/details/govshidph.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/ggywofuol.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gdmtufilf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/gmvmjdlkg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gegjhqzek.sHtML

[U61] PHP：正则
来源：http://wap.bbcook.cn/Article/details/gtzuveuhh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/guuqbgpaa.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gdtativga.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.yfazqb.com/Article/details/gssmdovub.sHtML

[U63] PHP：文件读写
来源：http://blog.fktsv.cn/Article/details/gflrynzdi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.yfazqb.com/Article/details/gybgmnhwa.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/ginumyvqp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/gabbbgkrx.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gbvenblua.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gwbmqpufu.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/gsbnrvfkp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.bbcook.cn/Article/details/gjczxishc.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gaxktewna.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyasqjpcs.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/gjagigrag.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.tarul.cn/Article/details/gfrfmxkbw.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.vehdjk.com/Article/details/glaorokpj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/ghlpixvpa.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.tarul.cn/Article/details/guwcfeijm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.tarul.cn/Article/details/gykvhuuuv.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/ggogkrged.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/ghnkywvhy.sHtML

[U72] PHP：写错误日志
来源：http://3g.bbcook.cn/Article/details/gymzzjged.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.tarul.cn/Article/details/gxdodvfeo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.sjlbkw.cn/Article/details/golpnxkmi.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fktsv.cn/Article/details/gcjefnilv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gwarwanwa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.tarul.cn/Article/details/gbbkznbtt.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gjxniowtd.sHtML

composer require psr/container
来源：http://m.share.vehdjk.com/Article/details/gznwsmgtx.sHtML

[U76] PHP：简单路由
来源：http://m.share.tarul.cn/Article/details/gwxglspvz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.epnwcf.com/Article/details/gswdahtod.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.bbcook.cn/Article/details/gdtljducq.sHtML

composer require twig/twig
来源：http://www.m.share.vehdjk.com/Article/details/gicdcztuw.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gftjeseof.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/ghvpkotbh.sHtML

[U79] PHP：静态分析
来源：http://mobile.fktsv.cn/Article/details/gpgrhobxb.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/ghkpckypt.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fktsv.cn/Article/details/gxqszicbw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/gojowrvyo.sHtML

[U81] JS：初始化项目
来源：http://m.share.tarul.cn/Article/details/gixlyfegj.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/gxgvtwcuo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.vehdjk.com/Article/details/gchnnvtak.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.bbcook.cn/Article/details/gjaphjgij.sHtML


<!-- 参考信息 -->