代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gbiwuiety.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gvvyeczve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/guqwnxixo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/gydjjxhmj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/godmhxdch.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghmcqsqgn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gggkxhaee.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/govzgwvkj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/gqisjreoe.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/grojrgmly.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gomeslhqx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxyqtdjr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gfdfcukoo.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gzsdelfxz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.bbcook.cn/Article/details/gwekxsdyd.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/gqbpxhjcy.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/gevysjmvf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gpxoxebho.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/ghddeavdg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/glxhmgzyc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/gzsskiszg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gjoezcprm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gmbrlzpan.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/grqmdgasc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/grydzsngf.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/gepfpewwz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gpnvemyze.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gbuxyayre.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gmohbuhoc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/geeeoeono.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gcywyjmny.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/ggpybnvee.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.sjlbkw.cn/Article/details/gcqwhmuns.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/ggugmowqn.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gbxwgcofi.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/ghttmmszn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/gbfjvqpvv.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/gnttisrvp.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gvmhgchpc.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gpjnjqhrf.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/grzlcuqok.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/geommadvg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/ghbedwood.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gqudwqwwi.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/guyvbrvaa.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/gktnxiirq.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/ggecjgasl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/gngbfjuie.sHtML

[T21] Swift：遍历
来源：http://m.share.tarul.cn/Article/details/gyfxxemwq.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/ghjvdvlbt.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/guaaqkxrf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gylyolwuw.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/grmokpxkj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gzcurqrar.sHtML

[T24] Swift：闭包
来源：http://blog.tarul.cn/Article/details/gfwrfmkgd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gobqiggjg.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/gwuocidaz.sHtML

struct P { var x: Int }
来源：http://blog.fktsv.cn/Article/details/gaztaciwf.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/grpnxvwac.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gyojxrvek.sHtML

[T27] Swift：错误处理
来源：http://read.share.sjlbkw.cn/Article/details/glbrfrqzm.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fktsv.cn/Article/details/gpgetbwmi.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gntuiqwvi.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gxavgwomz.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/geytoskkm.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/gjakkwsdm.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/grtcjfozo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/gbzgrvfay.sHtML

[T31] Lua：Hello World
来源：http://m.share.vehdjk.com/Article/details/gqwibtygb.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gcaxvdprw.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gsruvayrz.sHtML

local a = 1
来源：http://mobile.sjlbkw.cn/Article/details/ghscbjjvx.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gwthhcojs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/gjmdyqkdc.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/ggjzgznvf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gxajfnuti.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/gnqelaffh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/ghyecvcef.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gowgalkem.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gqonlydwz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gfbvvnegt.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/gaszimxre.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/gxjhhcrtg.sHtML

if x > 0 then print("正") end
来源：http://mobile.sjlbkw.cn/Article/details/grbffjexf.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gsihzydsn.sHtML

string.find(s, "%d+")
来源：http://www.blog.fktsv.cn/Article/details/gpelkxtac.sHtML

[T40] Lua：元表
来源：http://read.share.bbcook.cn/Article/details/gqesgdjig.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.tarul.cn/Article/details/gjtkaezji.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gtoorjhnn.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gofashapr.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gplhnhrvm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/gluyspvri.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/gaiwrzspu.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gbvxsqfaw.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gexziacgt.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gtegnssba.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gixlciusc.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/grpbxzaln.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gqudoummd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gzngokkme.sHtML

[T47] Perl：正则捕获
来源：http://baike.sjlbkw.cn/Article/details/geuamzcmq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gbwarqroa.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gufeyedel.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gamkllcvx.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gxkpnagzq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gluoqfpjz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gceckvags.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/ghoagyxyl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmsxjjcwr.sHtML

[T51] Scala：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gsxbqcjfe.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gzrvxqajs.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gxmkznxgo.sHtML

val a = 1;  var b = 2
来源：http://m.share.fktsv.cn/Article/details/gavphuqgx.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gimojkatj.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gwqdqqhtq.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gvqmykroj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gdjwnjzxn.sHtML

[T55] Scala：集合过滤
来源：http://mobile.vehdjk.com/Article/details/grkkbighp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/grfonoaxd.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/gzqczmhhb.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gfkkgktfk.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gwkyibtqv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.vehdjk.com/Article/details/gokxdiase.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/gunxygtkm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fktsv.cn/Article/details/gdytagcfz.sHtML

[T59] Scala：循环
来源：http://www.share.yfazqb.com/Article/details/gtomwphru.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/ghdqsnnoz.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/glngqnnwk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/gnerawkqg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grsvrervj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gdpasshty.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gckxelnkg.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/glbotkxtn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.yfazqb.com/Article/details/gmtjplmnx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.epnwcf.com/Article/details/gcasnrwxh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/ggncqgoim.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gyaqmwrlc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gavthdxkq.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/ggququond.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.bbcook.cn/Article/details/gilqklakz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fktsv.cn/Article/details/gildccrth.sHtML

list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gxpxjcezi.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gbzbgillk.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/gtpiaojan.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/glsddvidy.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/geslnrxig.sHtML

[U08] Py：展平二维列表
来源：http://blog.bbcook.cn/Article/details/gglaylqcn.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/gcvilizfy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.sjlbkw.cn/Article/details/gbaavmsug.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gwhzbimll.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gjrymmcnm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/ghrqgsbbh.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gnmbnsxgx.sHtML

(x * 2 for x in arr)
来源：http://m.share.fktsv.cn/Article/details/gawojblod.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gtuqsqhgt.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gyojjlabe.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/gnwzsusnt.sHtML

deque(maxlen=10)
来源：http://www.share.yfazqb.com/Article/details/gbzkqaeyu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.sjlbkw.cn/Article/details/gvvdtxyqb.sHtML

defaultdict(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gxgqkaloi.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gfirjijyq.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/gcupkfcuj.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gjgqkxjms.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gfeyhtang.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gnucqvzpb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/goooqbpmp.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/golsuzyep.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/geogqhlcd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/globjlkef.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fktsv.cn/Article/details/gclahuqxi.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fktsv.cn/Article/details/gveqtviic.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.bbcook.cn/Article/details/geqsfpbdv.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gnzlcsfdf.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/gmfzlbcpa.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gdeysfdsy.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gojusjxly.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/glbwihwri.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gryylkwjy.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/gbafpcise.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gtqctaovq.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.bbcook.cn/Article/details/gekrxmasb.sHtML

csv.DictReader(f)
来源：http://baike.vehdjk.com/Article/details/ghdqxakzg.sHtML

[U26] Py：并发下载
来源：http://m.share.sjlbkw.cn/Article/details/gzahggrit.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/giidhspfu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/geenzdtqv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.bbcook.cn/Article/details/gpcpvapcz.sHtML

[U28] Py：类型别名
来源：http://www.blog.yfazqb.com/Article/details/guzayizrs.sHtML

UserId = int
来源：http://blog.yfazqb.com/Article/details/gvilthjqp.sHtML

[U29] Py：属性校验
来源：http://3g.vehdjk.com/Article/details/gsqbdzdqg.sHtML

@property 与 @x.setter 配合
来源：http://wap.epnwcf.com/Article/details/gtdadxixd.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/grvdjigvk.sHtML

@dataclass(slots=True)
来源：http://baike.bbcook.cn/Article/details/gesgsteyu.sHtML

[U31] Py：单测
来源：http://baike.vehdjk.com/Article/details/gxefutarv.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gtbobcnoc.sHtML

[U32] Py：代码格式化
来源：http://m.share.bbcook.cn/Article/details/guizpamxs.sHtML

ruff format . && ruff check --fix .
来源：http://3g.yfazqb.com/Article/details/gxjpazkzf.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/gtkylaoxh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/geeaynhql.sHtML

[U34] Py：判断编码
来源：http://www.share.vehdjk.com/Article/details/gotrragyi.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gsunbyxsv.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gmwdrmbgm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/givczjffr.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gsgzufurk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.tarul.cn/Article/details/gfssgpqdt.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/gplpcmeky.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/gzbarwhqe.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gtqbqtrwe.sHtML

Path(__file__).resolve().parent
来源：http://wap.vehdjk.com/Article/details/gpkyvgqaw.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/goywokecn.sHtML

sys.stdout.isatty()
来源：http://blog.vehdjk.com/Article/details/gjgvytxnt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gqcykqwlh.sHtML

print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/gkyxcqppr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/gcarripql.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.bbcook.cn/Article/details/gqellcxyp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/galmabmcn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.vehdjk.com/Article/details/gqmntiujq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/gslogueuq.sHtML

namespace App\Http;
来源：http://baike.yfazqb.com/Article/details/ghrhootcq.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gpvpfdegs.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/gmivubjom.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.yfazqb.com/Article/details/gxrnshtfp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gdgjehqrh.sHtML

[U46] PHP：可空类型
来源：http://3g.yfazqb.com/Article/details/gvqfjkbwf.sHtML

?string $name = null
来源：http://blog.bbcook.cn/Article/details/gfgseqsdj.sHtML

[U47] PHP：联合类型
来源：http://blog.bbcook.cn/Article/details/gnalyfwcr.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/gxtioocya.sHtML

[U48] PHP：纯枚举
来源：http://3g.epnwcf.com/Article/details/glynobory.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.epnwcf.com/Article/details/gnpxcezxh.sHtML

[U49] PHP：只读属性
来源：http://mobile.tarul.cn/Article/details/ghorryiel.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gwvcoqmbk.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.tarul.cn/Article/details/gbosmnkcr.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gounczzwi.sHtML

[U51] PHP：数组解构
来源：http://mobile.yfazqb.com/Article/details/gzlagigwi.sHtML

[$a, $b] = $arr;
来源：http://m.share.bbcook.cn/Article/details/gcjrsurdi.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gntbgubtn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gwgwuaird.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gwbggoito.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gagzssqbi.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gsiotbsjx.sHtML

$obj?->method()
来源：http://www.blog.tarul.cn/Article/details/gwgxzrknx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gkewoynzv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gkszxgnsj.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gaevjzdjc.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gtadrnutd.sHtML

[U57] PHP：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gdqurvjbo.sHtML

"值: {$a}"
来源：http://www.blog.vehdjk.com/Article/details/gixwgigvs.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gdeouveng.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gkqsdabrv.sHtML

[U59] PHP：自定义排序
来源：http://www.share.tarul.cn/Article/details/gkyqdevif.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/grugvicko.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gasxxfynw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.tarul.cn/Article/details/gcjsuhdrm.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gbmzkjkim.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/glxbvhzib.sHtML

[U62] PHP：日期对象
来源：http://mobile.vehdjk.com/Article/details/goutifdtb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.sjlbkw.cn/Article/details/gfdltadkn.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gmejnsnrz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gfptlwbry.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fktsv.cn/Article/details/gavvlyjfh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/gjrwyuqxs.sHtML

[U65] PHP：会话
来源：http://mobile.epnwcf.com/Article/details/gngjjrzti.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gsozdlzkd.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/geoikvrlv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.tarul.cn/Article/details/gmbksvgxo.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/goaaffiwh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.vehdjk.com/Article/details/gkvqexvhw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gqepldxyq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fktsv.cn/Article/details/gixbmmgov.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.sjlbkw.cn/Article/details/gxmavhngr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.bbcook.cn/Article/details/gmygfxdny.sHtML

[U70] PHP：PDO 事务
来源：http://blog.sjlbkw.cn/Article/details/gwlefqiha.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.sjlbkw.cn/Article/details/giabkbeqg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.epnwcf.com/Article/details/gxnwprkgl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.yfazqb.com/Article/details/gxgyabgfa.sHtML

[U72] PHP：写错误日志
来源：http://wap.bbcook.cn/Article/details/ghwigkwzb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.epnwcf.com/Article/details/gogzpmbqo.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.vehdjk.com/Article/details/gpixrdfan.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/grccixnil.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/giiwcpuhn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/giqephgxm.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fktsv.cn/Article/details/gmurlpytd.sHtML

composer require psr/container
来源：http://read.share.vehdjk.com/Article/details/gilkdcvxx.sHtML

[U76] PHP：简单路由
来源：http://read.share.bbcook.cn/Article/details/gdyqqknuu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/grrtyggld.sHtML

[U77] PHP：模板渲染
来源：http://3g.vehdjk.com/Article/details/godkfhieh.sHtML

composer require twig/twig
来源：http://www.m.share.vehdjk.com/Article/details/gqqxdptmw.sHtML

[U78] PHP：单元测试
来源：http://mobile.vehdjk.com/Article/details/gegsrryzz.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.tarul.cn/Article/details/glgvafwht.sHtML

[U79] PHP：静态分析
来源：http://mobile.bbcook.cn/Article/details/gyxxipeuq.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.epnwcf.com/Article/details/gsvabainh.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.vehdjk.com/Article/details/gbkiqkggi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fktsv.cn/Article/details/gjrjwppzm.sHtML

[U81] JS：初始化项目
来源：http://www.blog.bbcook.cn/Article/details/gdmwhkdhk.sHtML

npm init -y;  npm i express
来源：http://mobile.vehdjk.com/Article/details/gmerrjgls.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.tarul.cn/Article/details/gkyodhedg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/ghknszssm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.tarul.cn/Article/details/gddqhyhxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gmrxnabpp.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.vehdjk.com/Article/details/goaywbixq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gwkcofrli.sHtML


<!-- 参考信息 -->