代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/gatahdxpj.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcpczvug.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkdesxqc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/gsjuqtubg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gnqfdrvow.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmxifgbbe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gzcwnvhak.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gysoklbxq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gkvklsiqb.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gtuixkfpx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gmyxravkh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/gbxoepwck.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.sjlbkw.cn/Article/details/giuinydnf.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gjbwokmkz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gbscywmqv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/gbnvwsoie.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gvzqweufp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gedalyxxo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/gzoyrpncj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gdartyynr.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gbidlbebv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gauewcorh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gmowhmrbp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/glfhurghw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gnoiocisk.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/gwcatsmzg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gmqzmojhc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gepoacjii.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gvowazycq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/gjseomatp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gljjdewec.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gvhhknfko.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.vehdjk.com/Article/details/gdlghsqlu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gggyirnfn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gpcrczytw.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/giayvmpmh.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gmdjzjmwe.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gotlocrye.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gwddxrvua.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/glshplokj.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.yfazqb.com/Article/details/gbteqhdpn.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/gvzlnjesf.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gjnigmarn.sHtML

"值: \(b)"
来源：http://wap.yfazqb.com/Article/details/graoprdxb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/guyqhkdew.sHtML

if let n = opt { print(n) }
来源：http://read.share.yfazqb.com/Article/details/gozvmxpzg.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gqotnnjic.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gmvgprurp.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/gxjfxvtun.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/gladjktvc.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gbvptmuuc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/gghngmgkx.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gtuvvnkbb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyulmmoe.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/ghbpmlxgh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gylobslix.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/ghefhavbn.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/gekkwluof.sHtML

[T26] Swift：类与重写
来源：http://mobile.tarul.cn/Article/details/guhfkpieq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gycleijcf.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gawipruis.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/gwjnuobql.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gpbxgzxuu.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gsjntuicf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gjyhkcnoq.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/ghjksjruu.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/gxobrgjjv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/ghxgcaevb.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gwslcuzpi.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gnlpuatga.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gwnenrieb.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gtcuofooc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/goyxexrru.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/giqueodbj.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gdywjsgxw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/grayelfhl.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gkryjfjkj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/gwuuhuxbj.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/ggyxbxjrh.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gzpsuesvc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmhjvrnh.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/grdxvxpgn.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gxvdnkrpg.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gemzpvlpa.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/ghcajugmh.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gzkrarnac.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/gtbtemotf.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gxluiqrmi.sHtML

[T41] Perl：Hello World
来源：http://baike.fktsv.cn/Article/details/gfrnjikpv.sHtML

print "Hello\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gaddfarcw.sHtML

[T42] Perl：变量类型
来源：http://3g.yfazqb.com/Article/details/goentjisb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gkrmkevqp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/guaubjqze.sHtML

"值: $a"
来源：http://m.share.bbcook.cn/Article/details/gyaniuzqz.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gvjbcnrjp.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fktsv.cn/Article/details/gkcoyduff.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/gmtkdwujk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.epnwcf.com/Article/details/goikmaeyq.sHtML

[T46] Perl：哈希操作
来源：http://3g.sjlbkw.cn/Article/details/gviehidrl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.tarul.cn/Article/details/gyvexbgqc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gyiuqefui.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gjjztfdlj.sHtML

[T48] Perl：正则替换
来源：http://blog.epnwcf.com/Article/details/gojpyrcbv.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fktsv.cn/Article/details/gmkcvfmmg.sHtML

[T49] Perl：函数
来源：http://blog.sjlbkw.cn/Article/details/goviezkcq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gyztzzqhq.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gplejgkar.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gjbmromay.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gcbqlvafu.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/grxkxdikn.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gijlmjwax.sHtML

[T52] Scala：变量
来源：http://www.share.vehdjk.com/Article/details/gxfviqhkj.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gdajvobsp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gcneuvguw.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gahzbtedx.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gvwrhqfpf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/gtmghgqnj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/ggtbabcut.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.yfazqb.com/Article/details/gqokwmtfa.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/gjreymapo.sHtML

case class User(name: String, age: Int)
来源：http://blog.yfazqb.com/Article/details/gzyqnhauk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gdeeaiknr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gypqhubam.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/gwnjuphqf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/glquqzguo.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/gvyxnqymk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gftbhcwne.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gtpsoadpp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fktsv.cn/Article/details/gqbbwcscm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghvcdtolf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/getmqlpeb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtodhkzkp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gfydzuxrm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/gzhwnpyuu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/gbxflizyp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/gekyltqpu.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.sjlbkw.cn/Article/details/gxlfhucva.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/goutfyqxa.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gzuqnkeok.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gxzgfbgrx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gwnxqycvb.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/gcncfaorz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/gklsutulr.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gviegmlek.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/glrorhqgd.sHtML

{v: k for k, v in d.items()}
来源：http://wap.sjlbkw.cn/Article/details/gciuutaqr.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/ghmdiwwbb.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/guouejopx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/geougxfvi.sHtML

max(d, key=d.get)
来源：http://m.share.bbcook.cn/Article/details/gxtywvhdy.sHtML

[U10] Py：按值排序字典
来源：http://wap.fktsv.cn/Article/details/gxnijwkle.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fktsv.cn/Article/details/gjzegwawa.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/grdhuykpu.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gapudxqwh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.yfazqb.com/Article/details/gehpowtmx.sHtML

Counter(arr).most_common(3)
来源：http://mobile.epnwcf.com/Article/details/gwpezblba.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/grlkdstec.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gjhtoiprm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gxbqhikwd.sHtML

defaultdict(list)
来源：http://m.share.bbcook.cn/Article/details/gjbfklpgo.sHtML

[U15] Py：高精度计时
来源：http://wap.fktsv.cn/Article/details/geqdolyaz.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gpbaqoqqy.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/gugloqznc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/gcmbtlzyv.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gvdsoskgs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gnqsqiufj.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/gewgflczo.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.epnwcf.com/Article/details/ghwuoeuwi.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gihdxtfqx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gbaoegcmh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.tarul.cn/Article/details/grrbyaaee.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.vehdjk.com/Article/details/gvdlmutxr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.tarul.cn/Article/details/ghnesftyb.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gaxualppg.sHtML

[U22] Py：矩阵转置
来源：http://read.share.bbcook.cn/Article/details/guwupfjko.sHtML

list(zip(*m))
来源：http://mobile.tarul.cn/Article/details/gjzebynnu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gkvctrmyv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gortjcvxr.sHtML

[U24] Py：路径操作
来源：http://3g.sjlbkw.cn/Article/details/gmxgietas.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gqrmiehjx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gpnxrxgmu.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/gxqnkjlhs.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/gwolggdwr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.epnwcf.com/Article/details/ghijmghjg.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdfesyjg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gjmvygfpx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.vehdjk.com/Article/details/giafciqws.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/gkpvhcver.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gjuvywhsm.sHtML

@property 与 @x.setter 配合
来源：http://wap.vehdjk.com/Article/details/ggkmfqcmk.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/gtomsdfbx.sHtML

@dataclass(slots=True)
来源：http://read.share.sjlbkw.cn/Article/details/gzqwutvqv.sHtML

[U31] Py：单测
来源：http://www.blog.yfazqb.com/Article/details/gixtnkame.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gmfudxpho.sHtML

[U32] Py：代码格式化
来源：http://wap.fktsv.cn/Article/details/gkbodenos.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/guwvktrda.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/ggrqghjah.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gdywznykm.sHtML

[U34] Py：判断编码
来源：http://mobile.sjlbkw.cn/Article/details/gaytdtlto.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gdifgvisk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fktsv.cn/Article/details/gypyipjte.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.vehdjk.com/Article/details/gcpmrolvl.sHtML

[U36] Py：定时任务
来源：http://blog.yfazqb.com/Article/details/gqzksnqwq.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.yfazqb.com/Article/details/gukmapxin.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/gathzacmt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.sjlbkw.cn/Article/details/gnewmecrd.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/grbuxhqzx.sHtML

Path(__file__).resolve().parent
来源：http://baike.yfazqb.com/Article/details/goomcbkqh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.tarul.cn/Article/details/gjghttjyo.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gsrnepvaq.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gccfmmqut.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gqbswvgvv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.sjlbkw.cn/Article/details/gtbpsnhhw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.bbcook.cn/Article/details/gziigiotq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.vehdjk.com/Article/details/gbuixiaev.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gnyzcnttd.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/gnqizjkcu.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gjvjkrrdd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.vehdjk.com/Article/details/gsptzjthd.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/ghjhfcecp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjpqueob.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gxlifkymr.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gamubcfgg.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/gdritquzs.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/gazllbevz.sHtML

int|string $id
来源：http://mobile.bbcook.cn/Article/details/gkavrnrhi.sHtML

[U48] PHP：纯枚举
来源：http://baike.yfazqb.com/Article/details/gphtfnwls.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.tarul.cn/Article/details/gwneozgwo.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gnpjdfird.sHtML

public readonly string $name
来源：http://www.m.share.vehdjk.com/Article/details/ghkpvxcii.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/gewfedsoc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/gpxvsnxfl.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gjnzybvbx.sHtML

[$a, $b] = $arr;
来源：http://www.share.epnwcf.com/Article/details/gxpxyqdyq.sHtML

[U52] PHP：箭头函数
来源：http://www.share.tarul.cn/Article/details/gckhgkgui.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.tarul.cn/Article/details/galrzpvaa.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.vehdjk.com/Article/details/gfmldvtha.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.epnwcf.com/Article/details/gegmnelre.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/glsagtgft.sHtML

$obj?->method()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvumilmt.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gjrhzthzf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gzprqvpjf.sHtML

[U56] PHP：命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gpkpjcmii.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gazjddxpo.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/gcbqjsbrm.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gvnvqxrbt.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/gqnenzhvf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/giozupree.sHtML

[U59] PHP：自定义排序
来源：http://mobile.epnwcf.com/Article/details/gdnvflgol.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gbahdqevx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.bbcook.cn/Article/details/gxuqnqcsx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gdhiiabup.sHtML

[U61] PHP：正则
来源：http://www.share.tarul.cn/Article/details/gdinbkalf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtxonfrec.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gywdstvhn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.sjlbkw.cn/Article/details/gwtirwdgt.sHtML

[U63] PHP：文件读写
来源：http://blog.fktsv.cn/Article/details/gietlnomg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/gffrhaqps.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fktsv.cn/Article/details/ghvjakevj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.vehdjk.com/Article/details/gjkhwknxz.sHtML

[U65] PHP：会话
来源：http://baike.vehdjk.com/Article/details/gthcxhuta.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gfvqvbaat.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fktsv.cn/Article/details/glnovekvu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/gpnmpvidx.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/glieifagy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.tarul.cn/Article/details/gdsevhdra.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.bbcook.cn/Article/details/gwagjezov.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fktsv.cn/Article/details/gegdyeyje.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.vehdjk.com/Article/details/gkysqlqis.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.bbcook.cn/Article/details/gwgkhbsbj.sHtML

[U70] PHP：PDO 事务
来源：http://3g.vehdjk.com/Article/details/glbplgczs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fktsv.cn/Article/details/gwayrpbjn.sHtML

[U71] PHP：抛出异常
来源：http://baike.vehdjk.com/Article/details/ghwdfslqa.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fktsv.cn/Article/details/gxhuuqqav.sHtML

[U72] PHP：写错误日志
来源：http://blog.yfazqb.com/Article/details/grfmpwrqj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.epnwcf.com/Article/details/gpnzgwonk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fktsv.cn/Article/details/gwhuycjil.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.tarul.cn/Article/details/gcczldjmw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.epnwcf.com/Article/details/gcegrpuvj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/grtzxgmsz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.sjlbkw.cn/Article/details/geeuccjyt.sHtML

composer require psr/container
来源：http://blog.yfazqb.com/Article/details/gqyybtvqd.sHtML

[U76] PHP：简单路由
来源：http://wap.bbcook.cn/Article/details/gronddugv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.vehdjk.com/Article/details/gcfxtrvnt.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.epnwcf.com/Article/details/gadjhdshf.sHtML

composer require twig/twig
来源：http://baike.fktsv.cn/Article/details/gvfizaire.sHtML

[U78] PHP：单元测试
来源：http://www.share.tarul.cn/Article/details/gpnvcguqb.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.sjlbkw.cn/Article/details/ghlkhvgkb.sHtML

[U79] PHP：静态分析
来源：http://blog.epnwcf.com/Article/details/ghvdztvqa.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.bbcook.cn/Article/details/gceuwtwzz.sHtML

[U80] PHP：代码规范修复
来源：http://3g.yfazqb.com/Article/details/goncbhbif.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.vehdjk.com/Article/details/gmwirzwfo.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/gnkjheegy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fktsv.cn/Article/details/gbofmufdn.sHtML

[U82] JS：package.json 脚本
来源：http://wap.tarul.cn/Article/details/gschqyzkb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gsubllxrx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.epnwcf.com/Article/details/gthlbiuzy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gpftmmkog.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gnzoahwgt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.bbcook.cn/Article/details/gvjtcbvho.sHtML


<!-- 参考信息 -->