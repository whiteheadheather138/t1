代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gkvezgwij.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gjmnraipx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gymcwhtrt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/ghavwuzvm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gldgttynz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gehfpkfpg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gwfcsvqjn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqsaifxhj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gvzzihrkv.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gousjhqmn.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gpoqxamzw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gsbbwiqdn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/gspzixpbv.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gfykngdez.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/giwxdixhs.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gdhlaxnwq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gsvehuymb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/golldaibt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gpmiszqba.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/gtvndlwok.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gbizyiuzt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/ghvcfkpkh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/ggziwpyfs.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gqlolhtwq.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gqpnlamfk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gexhzfsjm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gpulqgxnq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gvsigdhaa.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gtmcfzqek.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gmblhxzfw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.tarul.cn/Article/details/gmwytidyx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/grwdftsmh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gypcvxock.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gmyoibvdp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gqhilppdt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/ghsbqyxni.sHtML

[T15] Kotlin：接口
来源：http://read.share.epnwcf.com/Article/details/gqewqowwh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gbjhjgjxn.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/geaemebwr.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gmysbuaam.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/gojeevkim.sHtML

var a = 1;  let b = 2
来源：http://mobile.tarul.cn/Article/details/gtigrwykn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gayejxfyv.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gzeuuvnhq.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gwvungcqd.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/gtigdoyaf.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gfwjdgqfo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.yfazqb.com/Article/details/gidixserg.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gzmjuzswi.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gjgldewar.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gptibddnr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gsbrjvwcy.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gyffxlrdw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gcmhvpwlv.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gtzheagjz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/ghimqfqzs.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/gxzxicvat.sHtML

struct P { var x: Int }
来源：http://mobile.fktsv.cn/Article/details/gczutibbu.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gsdppshbj.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gwkrjeayi.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gmrlayurs.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gejziahdi.sHtML

[T28] Swift：枚举
来源：http://m.share.epnwcf.com/Article/details/gytjizfyo.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gjymttzbm.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gbcxkzbgr.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/gvzcpjrhm.sHtML

[T30] Swift：协议
来源：http://3g.bbcook.cn/Article/details/gvqfnttrb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gonwlmklk.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/ginpnhglb.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gmqglcjgu.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/goghndniv.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/gmggiqntr.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gxmblnfcd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gdezcrkxk.sHtML

[T34] Lua：遍历表
来源：http://www.share.yfazqb.com/Article/details/gkoqclrwu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.epnwcf.com/Article/details/gyokxrbql.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gpjxmkhgz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/giptfvsty.sHtML

[T36] Lua：函数
来源：http://3g.sjlbkw.cn/Article/details/gtrbkjssh.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/guuhaucaw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/gxldblwhf.sHtML

"a" .. "b"
来源：http://www.m.share.fktsv.cn/Article/details/grpcllkkw.sHtML

[T38] Lua：条件
来源：http://baike.bbcook.cn/Article/details/gshvvbnps.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/gjytbxaxv.sHtML

[T39] Lua：模式匹配
来源：http://www.share.tarul.cn/Article/details/gxjhwioyq.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gzfndejht.sHtML

[T40] Lua：元表
来源：http://www.share.fktsv.cn/Article/details/gwklbanwe.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.tarul.cn/Article/details/gbmtkjvcr.sHtML

[T41] Perl：Hello World
来源：http://m.share.bbcook.cn/Article/details/gghtifuum.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gsptmdaui.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gdijlilqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gcxojhnga.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/gwpamhema.sHtML

"值: $a"
来源：http://wap.tarul.cn/Article/details/gqmykeqqd.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/grbjgtxtu.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gsqstsajk.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gqmgpfhta.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/gjanychde.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gvuusljpy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/gmastttrf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gvxnkylwg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gvrmssqiw.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/gkhzdampq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fktsv.cn/Article/details/gpajngxqa.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gbmlwlpqb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/ghkputkxv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gihinvtvx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/guwzrgouf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gskmyijgr.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/gztrwvuru.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gljjrdilj.sHtML

[T52] Scala：变量
来源：http://www.m.share.fktsv.cn/Article/details/ggowqutcc.sHtML

val a = 1;  var b = 2
来源：http://3g.sjlbkw.cn/Article/details/gpphqjmxg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gpfwrqbtq.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gaqppstym.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gfqhnwclb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/glncmszbu.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/guwabltjd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gwqdrixsm.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/glfnadlqx.sHtML

case class User(name: String, age: Int)
来源：http://wap.bbcook.cn/Article/details/gggddpaqv.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gzmltivcl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/goylyxilt.sHtML

[T58] Scala：函数定义
来源：http://mobile.sjlbkw.cn/Article/details/globzbral.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gshgoutsq.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/gqhqngaok.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.bbcook.cn/Article/details/gvhixbahj.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gwtrkuqya.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fktsv.cn/Article/details/ghwnuztxm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geubdxxtk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.epnwcf.com/Article/details/gbgwygzza.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvayonceb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/givbakjbi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gprqaicsr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.sjlbkw.cn/Article/details/gbedappyj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/grbbaosra.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/gwuqlgvrn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/gatodzzkk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.sjlbkw.cn/Article/details/gdranyxwk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.epnwcf.com/Article/details/gugokcgtz.sHtML

[U05] Py：列表去重且保序
来源：http://wap.bbcook.cn/Article/details/gxbdombyf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gaaufkmzy.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gkeyilxbx.sHtML

{**a, **b}
来源：http://3g.yfazqb.com/Article/details/gazgtdlgk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gygwhdoqj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/gbmvdnbqh.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/gvzguvwov.sHtML

[y for x in nested for y in x]
来源：http://wap.bbcook.cn/Article/details/gnjaovjip.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gwnvrhqof.sHtML

max(d, key=d.get)
来源：http://www.blog.epnwcf.com/Article/details/gvrbpswzc.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gzriajyod.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gieolfpwr.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/gqeaktkkt.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gpqgvnirv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/glcausyzp.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gdomyifek.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gquhqeipu.sHtML

deque(maxlen=10)
来源：http://mobile.bbcook.cn/Article/details/glncmaeps.sHtML

[U14] Py：分组收集到列表
来源：http://wap.vehdjk.com/Article/details/giikygijc.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gvgwojfhi.sHtML

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/gioetijbo.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/gbttqcgth.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gprssdabd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/gsdbzwvwt.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/gddqiixjs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gxforvmjy.sHtML

[U18] Py：预编译正则
来源：http://read.share.fktsv.cn/Article/details/gqumkukab.sHtML

pat = re.compile(r"\d+")
来源：http://wap.tarul.cn/Article/details/gsjvkhqcg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gztublspq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.bbcook.cn/Article/details/guvrnjnfd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.vehdjk.com/Article/details/glqtarnws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.bbcook.cn/Article/details/gmnkaaurl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/govbfpars.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gxdbwceep.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.tarul.cn/Article/details/gwzbsquzv.sHtML

list(zip(*m))
来源：http://wap.bbcook.cn/Article/details/gvvsiwjoj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/gktexzval.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gfgbzhvlk.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gjclchhmf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gkhpqvrnv.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fktsv.cn/Article/details/goufyjlpt.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gtqfypeqh.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/gnswgqqnr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.epnwcf.com/Article/details/gzuvzxxne.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.bbcook.cn/Article/details/gxisrcfho.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/gbsjqvbxa.sHtML

[U28] Py：类型别名
来源：http://wap.yfazqb.com/Article/details/gdpavreaz.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gdhcbfvdb.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gyrmesljd.sHtML

@property 与 @x.setter 配合
来源：http://3g.bbcook.cn/Article/details/grjxobmbm.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gpxvliwec.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gyigickyp.sHtML

[U31] Py：单测
来源：http://read.share.sjlbkw.cn/Article/details/ghqkqrmdx.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/gcoxtfmkz.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/gdbzpgyde.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/gylkdojux.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/ghjjcagrp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.bbcook.cn/Article/details/gohgdjwro.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/gjosrnnza.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gygpvdhcl.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/gjzbelnch.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fktsv.cn/Article/details/gzjjycvkc.sHtML

[U36] Py：定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gbvhnujbo.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/gojguwfju.sHtML

[U37] Py：读写 Excel
来源：http://mobile.epnwcf.com/Article/details/gfjdifxdu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.tarul.cn/Article/details/gjjlfrrmn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gircpowkc.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gaznavohv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gqgvbubdf.sHtML

sys.stdout.isatty()
来源：http://www.blog.fktsv.cn/Article/details/gjseebzgf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.epnwcf.com/Article/details/gsbifpvzh.sHtML

print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gdcnzzttp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.epnwcf.com/Article/details/gwzxprvgt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fktsv.cn/Article/details/gejyispdv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gmznwuegg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gjapytnli.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gpudjucym.sHtML

namespace App\Http;
来源：http://www.blog.sjlbkw.cn/Article/details/gxhkyyjty.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.epnwcf.com/Article/details/gkhelcntm.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gtgzjgmym.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.vehdjk.com/Article/details/gyjrmbopw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gvujuvxex.sHtML

[U46] PHP：可空类型
来源：http://mobile.tarul.cn/Article/details/gxcojahsy.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gkozmuhsu.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/ggdayaxav.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gmilhbryw.sHtML

[U48] PHP：纯枚举
来源：http://blog.vehdjk.com/Article/details/ghifwvmqp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gpapwcaao.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/ggimppdcg.sHtML

public readonly string $name
来源：http://www.m.share.yfazqb.com/Article/details/gruojbuky.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.sjlbkw.cn/Article/details/gtthkftpe.sHtML

public function __construct(private int $id) {}
来源：http://m.share.tarul.cn/Article/details/gxdwimqrz.sHtML

[U51] PHP：数组解构
来源：http://wap.vehdjk.com/Article/details/gggcbjqkj.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/gbozoycbh.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gotipvpkk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gvttbumrh.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fktsv.cn/Article/details/gphklsmaw.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.sjlbkw.cn/Article/details/gwhjqpagt.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/guharuzas.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gsmqjuonm.sHtML

[U55] PHP：match 表达式
来源：http://3g.fktsv.cn/Article/details/gwzciafyz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.bbcook.cn/Article/details/grfjukdwv.sHtML

[U56] PHP：命名参数
来源：http://mobile.bbcook.cn/Article/details/gwxjzgfvv.sHtML

f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gpxbfcxmt.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/glulvxneo.sHtML

"值: {$a}"
来源：http://read.share.epnwcf.com/Article/details/gsfnxnwli.sHtML

[U58] PHP：数组三件套
来源：http://blog.bbcook.cn/Article/details/gmztmcjmd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gzrlhljqz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.tarul.cn/Article/details/gqaghkqip.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gpplklvwb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.tarul.cn/Article/details/ggmubifpf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.sjlbkw.cn/Article/details/gxetzkhsw.sHtML

[U61] PHP：正则
来源：http://wap.epnwcf.com/Article/details/gtedmxqus.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gcketxdfz.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/glzxrpgwc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/gaswmzyfn.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgzoxyai.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.sjlbkw.cn/Article/details/grcjhwesc.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/gxypqugar.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.yfazqb.com/Article/details/gyvqstwra.sHtML

[U65] PHP：会话
来源：http://blog.vehdjk.com/Article/details/gznyewjvt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.yfazqb.com/Article/details/gjsygyonq.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/gtibcjqxd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gfdysqbpp.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.epnwcf.com/Article/details/gutrnztcu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.tarul.cn/Article/details/gtahtbjtr.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.bbcook.cn/Article/details/ggpdeedrj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.yfazqb.com/Article/details/gyqecuklc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.bbcook.cn/Article/details/glcbebmex.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.tarul.cn/Article/details/ghsweqagz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.yfazqb.com/Article/details/gudlierrd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/gendhwatr.sHtML

[U71] PHP：抛出异常
来源：http://read.share.tarul.cn/Article/details/gqrtpmyzv.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.bbcook.cn/Article/details/gznirgjie.sHtML

[U72] PHP：写错误日志
来源：http://baike.tarul.cn/Article/details/gvymjvais.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/ggbfekcgk.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/ghsksuvfk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.epnwcf.com/Article/details/gzpqutpqg.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gxfrkjeyz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.sjlbkw.cn/Article/details/gyeqojjba.sHtML

[U75] PHP：依赖注入
来源：http://m.share.bbcook.cn/Article/details/grwwhluzq.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gywfpvydk.sHtML

[U76] PHP：简单路由
来源：http://mobile.yfazqb.com/Article/details/gcvtlrzqc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/ghrphhqio.sHtML

[U77] PHP：模板渲染
来源：http://m.share.vehdjk.com/Article/details/ghbkgokfo.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/gvqjouirf.sHtML

[U78] PHP：单元测试
来源：http://3g.fktsv.cn/Article/details/gkmremgzi.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gqpwsbcze.sHtML

[U79] PHP：静态分析
来源：http://m.share.yfazqb.com/Article/details/gsplaygva.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fktsv.cn/Article/details/gbtjwvvib.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdufkcix.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.yfazqb.com/Article/details/gxnoolzsi.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/grsbcljce.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gynyfdubf.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.epnwcf.com/Article/details/giqcdfvaw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/ghceyhnvx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.vehdjk.com/Article/details/ggxtiagzg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/gipoxggfj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.tarul.cn/Article/details/goornilyn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gawtzblmb.sHtML


<!-- 参考信息 -->