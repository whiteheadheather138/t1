代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gyjzdkyjh.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gegosqvip.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/geifgyemc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gftdypitj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gjaomozob.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnmpqkmkv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/guwtizyrj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goiniesft.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/ggksizfal.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/ggewbzhnf.sHtML

[T02] Kotlin：变量
来源：http://mobile.epnwcf.com/Article/details/gxzmfpafk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gkkuczmgk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/guwlbschc.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/giojourfl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fktsv.cn/Article/details/gvfdygshz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gnqeuofgi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gocftyatv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/gtpfefbvm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gzappngov.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gjusocsiy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/glcnxpipd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gxlwypjuv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gfehlitrl.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gncgmkqoa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/gztpaxgyi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gebbybwcr.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gaxctboru.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/glxpkqkhx.sHtML

[T11] Kotlin：协程
来源：http://m.share.sjlbkw.cn/Article/details/gdjycffko.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/gablesich.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/gcbbzbmsm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gpqlfsqge.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/gzznfrnuv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gvafhjvia.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gqtxjwztw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gfzmvocpp.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/ghcxulrrx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.bbcook.cn/Article/details/gtdbtosvf.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gjwfwoopb.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gprzgveqe.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/glnizvcxr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.tarul.cn/Article/details/gqqnoatdj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gtsldsinx.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gpagxypoe.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/gmbmqobbq.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/ggyiciygz.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/gtafwkogo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/gchcaavdv.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/gugbvvcsd.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/guzchivwn.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/grgiwaauu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gguodfdbi.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gsqsmqquu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.tarul.cn/Article/details/glfyhocrx.sHtML

[T24] Swift：闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gnlllypju.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gvvzeplzs.sHtML

[T25] Swift：结构体
来源：http://blog.vehdjk.com/Article/details/giumhfekm.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gdcswybef.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/gxoohvwqp.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/gvjwesbsn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.yfazqb.com/Article/details/gpxlcgbeu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.sjlbkw.cn/Article/details/geftyxini.sHtML

[T28] Swift：枚举
来源：http://read.share.yfazqb.com/Article/details/gtfmxvehy.sHtML

enum Color { case red, green }
来源：http://www.blog.tarul.cn/Article/details/ghtwthutw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gqwfioimb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmwyudyn.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gujhrqxpg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/gtscjvaxn.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/gfmbfsvdf.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gpuwionon.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gfezqwvxz.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gfghmsqoe.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gdzbqonkz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gmqjgdthw.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/grnuwhije.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/gkbbqfekh.sHtML

[T35] Lua：字典表
来源：http://3g.fktsv.cn/Article/details/gpxxkyhaa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gtjbizoly.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gdasplqgr.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/ggrisqyhq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gaizgiogo.sHtML

"a" .. "b"
来源：http://read.share.epnwcf.com/Article/details/gtwxgyiry.sHtML

[T38] Lua：条件
来源：http://blog.bbcook.cn/Article/details/gogqpobmk.sHtML

if x > 0 then print("正") end
来源：http://3g.vehdjk.com/Article/details/gdtbecvev.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gyfqakiiy.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/ghyyktmlc.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/gixrfqomd.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gamczvbrc.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/gedtoboyo.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gjzjympvn.sHtML

[T42] Perl：变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gxkaukjcp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/ghvvkjvjj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gdllbpntu.sHtML

"值: $a"
来源：http://mobile.vehdjk.com/Article/details/gtlfhsaeg.sHtML

[T44] Perl：条件
来源：http://m.share.sjlbkw.cn/Article/details/gmtfxvthz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/galwotwim.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/glzlencyy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbwebnqcg.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/gjhotbnwc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/gmiugkdnj.sHtML

[T47] Perl：正则捕获
来源：http://blog.vehdjk.com/Article/details/ggpdysoxe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gxmuztuvy.sHtML

[T48] Perl：正则替换
来源：http://blog.yfazqb.com/Article/details/gyqtdmcqm.sHtML

$s =~ s/old/new/g;
来源：http://baike.yfazqb.com/Article/details/gatzvvygy.sHtML

[T49] Perl：函数
来源：http://www.m.share.epnwcf.com/Article/details/gjlltanzh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gcvxgnzgs.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gskrzmozn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.yfazqb.com/Article/details/ggmspekvm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gpqasqvuf.sHtML

[T51] Scala：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gsctpzghp.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gohztbcvm.sHtML

[T52] Scala：变量
来源：http://3g.bbcook.cn/Article/details/guhbrhxtu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/gyhfmzwuj.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnjqzkos.sHtML

s"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/giygpyfjf.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/gsukwnsxy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gulequcqw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/gvzjwtzxa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/gzieovuqs.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/gvjtiiccd.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/grsjvkclk.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gsxhwadsp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.yfazqb.com/Article/details/glezcmqxb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/grasnlpdm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fktsv.cn/Article/details/gfltdfmcg.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gkmumaadb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gmfcowjyj.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/grmwecnwb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gsyhjiiwc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvcecrech.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gqpogmzqy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giqijmskj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/gituhdcxq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.bbcook.cn/Article/details/gchzjrejd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/gctwuuklu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fktsv.cn/Article/details/guipvlwbm.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.tarul.cn/Article/details/gnvulyyxd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/goestspeg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gmtessusc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gwjshthsn.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gkdfaosao.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gnbijbzzb.sHtML

[U06] Py：合并两个字典
来源：http://wap.sjlbkw.cn/Article/details/geltvzjok.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gylgiafbr.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gqrqxjcfq.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gbypishbr.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gzeycbzsz.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/gxhhedmba.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/gdmtfoncm.sHtML

max(d, key=d.get)
来源：http://3g.vehdjk.com/Article/details/gspibogzm.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gsfgkqcdl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gkltegyyd.sHtML

[U11] Py：生成器表达式
来源：http://m.share.tarul.cn/Article/details/gcrbbottt.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/ghmsmfrgn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.yfazqb.com/Article/details/gmzukzini.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/gctmaruao.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gtmzqqqbz.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/guwcoefhs.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gvbdwfrit.sHtML

defaultdict(list)
来源：http://mobile.epnwcf.com/Article/details/gagqgxmth.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/ghmjexifd.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/gbfouxzek.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gsuuujskf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gztwhiner.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/glbjrjfgn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.vehdjk.com/Article/details/gibhjohey.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.sjlbkw.cn/Article/details/graaataui.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gmhimrusd.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.yfazqb.com/Article/details/glokuqupu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gntuiwhqy.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/geezwlvjm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.sjlbkw.cn/Article/details/gvaobkawl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gmvhsslou.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gsyupvcug.sHtML

[U22] Py：矩阵转置
来源：http://mobile.yfazqb.com/Article/details/gdvmhyzch.sHtML

list(zip(*m))
来源：http://baike.epnwcf.com/Article/details/gievcwapk.sHtML

[U23] Py：分块读取大文件
来源：http://3g.vehdjk.com/Article/details/glimbvzlz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.vehdjk.com/Article/details/gjnsmrech.sHtML

[U24] Py：路径操作
来源：http://m.share.vehdjk.com/Article/details/gznjecdkj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gqhixzfdt.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/gdtxwznba.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gqkehyhuj.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/gilvrtyub.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gnckvrdqh.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/gibhsccni.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.tarul.cn/Article/details/gxfotwexw.sHtML

[U28] Py：类型别名
来源：http://www.m.share.tarul.cn/Article/details/gmhtpbkak.sHtML

UserId = int
来源：http://www.m.share.fktsv.cn/Article/details/gonohlsho.sHtML

[U29] Py：属性校验
来源：http://baike.sjlbkw.cn/Article/details/gyffmgeia.sHtML

@property 与 @x.setter 配合
来源：http://mobile.sjlbkw.cn/Article/details/gzefrtvfd.sHtML

[U30] Py：数据类
来源：http://m.share.bbcook.cn/Article/details/gzmnpuhmg.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gyhdzrxjk.sHtML

[U31] Py：单测
来源：http://mobile.vehdjk.com/Article/details/gvgbwarwi.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gomtsncef.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/gipeglxea.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fktsv.cn/Article/details/gyfsmapjo.sHtML

[U33] Py：打包发布
来源：http://baike.epnwcf.com/Article/details/gfvussvwv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.tarul.cn/Article/details/gzilxawnd.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gerigjczl.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/gnispfagw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.bbcook.cn/Article/details/gycusgnpw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/goxqphkxo.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gznnqflvr.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fktsv.cn/Article/details/gthlqkhxy.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/gedxyacen.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.vehdjk.com/Article/details/gtfuihklz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gzkhjcmom.sHtML

Path(__file__).resolve().parent
来源：http://3g.tarul.cn/Article/details/gibhpwfdu.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.sjlbkw.cn/Article/details/gfjxpllnz.sHtML

sys.stdout.isatty()
来源：http://wap.yfazqb.com/Article/details/gfnfxwkbj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/gnuhqrypa.sHtML

print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/gtlbhitmy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/gawkaobhj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/guycpdnia.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.yfazqb.com/Article/details/gjlzlwwfp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.epnwcf.com/Article/details/gzlkqladd.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gxrcthpmp.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/guerpifiz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.bbcook.cn/Article/details/gdgvmrjnr.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/ghwqfxgxo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.yfazqb.com/Article/details/gdzganhtr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gasxgrxto.sHtML

[U46] PHP：可空类型
来源：http://baike.bbcook.cn/Article/details/gniycbrgs.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gyzwajmko.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/gbfyvzkbn.sHtML

int|string $id
来源：http://baike.sjlbkw.cn/Article/details/gfixxuhhy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.epnwcf.com/Article/details/ggmlboyro.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/goyrxylpb.sHtML

[U49] PHP：只读属性
来源：http://mobile.fktsv.cn/Article/details/gszjrtmtp.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/gukewkasa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.bbcook.cn/Article/details/gngnqgufh.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzkkvuyzh.sHtML

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gpnoqutok.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/ghlhhmosd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.tarul.cn/Article/details/gixlxiufn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.vehdjk.com/Article/details/gckdsnaga.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gbdujiipe.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/glaaywdqu.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/gylrghgcw.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/gsnonyhap.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/gnydfgpzf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gnvdqface.sHtML

[U56] PHP：命名参数
来源：http://3g.fktsv.cn/Article/details/gsjenhbiz.sHtML

f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gpumhqipv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gmjbmlfxw.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/guzptasyd.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/grgocpgon.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.bbcook.cn/Article/details/gzfpesmer.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gulsykszo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gviidqqfr.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.vehdjk.com/Article/details/gvodjxbtv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fktsv.cn/Article/details/goekiyppm.sHtML

[U61] PHP：正则
来源：http://baike.bbcook.cn/Article/details/ghiqsebap.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gsrezzhzp.sHtML

[U62] PHP：日期对象
来源：http://read.share.fktsv.cn/Article/details/gnmbgokht.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gebbsbagn.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/gchiuvhes.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/gpclicofb.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.bbcook.cn/Article/details/gbadixekp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/gcxtchdxn.sHtML

[U65] PHP：会话
来源：http://baike.epnwcf.com/Article/details/gsrnkyjvk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/gnfiwwrpt.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/gynmcllzp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.vehdjk.com/Article/details/gdywqurip.sHtML

[U67] PHP：处理文件上传
来源：http://baike.yfazqb.com/Article/details/gnskxdyck.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/groejbelz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/gyetjjuuw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gankijqws.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.sjlbkw.cn/Article/details/glzvrgcwl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.sjlbkw.cn/Article/details/gbmheltxg.sHtML

[U70] PHP：PDO 事务
来源：http://3g.epnwcf.com/Article/details/gdcxwaagj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/ggqdveebf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gqwcmfniv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/grtsebqkz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gmjhlbple.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.vehdjk.com/Article/details/gnnpgllne.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.bbcook.cn/Article/details/gtetndmig.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.sjlbkw.cn/Article/details/grqavzzfg.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.vehdjk.com/Article/details/ghstlgrqo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.tarul.cn/Article/details/gtujxllvm.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.epnwcf.com/Article/details/gdxnscnpt.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gsztyxdsp.sHtML

[U76] PHP：简单路由
来源：http://www.blog.epnwcf.com/Article/details/gakbairzw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gxbacyjdk.sHtML

[U77] PHP：模板渲染
来源：http://3g.tarul.cn/Article/details/gkchjljwa.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/gsozrevgv.sHtML

[U78] PHP：单元测试
来源：http://3g.sjlbkw.cn/Article/details/ghyeucdmq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/ghwiygcsf.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gqqahqlkb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gslzzhqee.sHtML

[U80] PHP：代码规范修复
来源：http://wap.bbcook.cn/Article/details/geihdehjc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.tarul.cn/Article/details/giexoknwo.sHtML

[U81] JS：初始化项目
来源：http://3g.vehdjk.com/Article/details/gfplqqmcr.sHtML

npm init -y;  npm i express
来源：http://wap.bbcook.cn/Article/details/ggmhrupqi.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fktsv.cn/Article/details/grhzvytyf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fktsv.cn/Article/details/ggrwuixxh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fktsv.cn/Article/details/gfrrfbquw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gmwcuadyh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.epnwcf.com/Article/details/gdtzvfpkn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gvqolnzvk.sHtML


<!-- 参考信息 -->