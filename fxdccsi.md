代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gjwiqoenn.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gwkopekdq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/ggitjmagy.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/gwxzttnsy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gjlmjvjye.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/gzdudvmzs.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gwbnijxzf.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gasmszafu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gknkscebf.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/grxpjeqpx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gjhcztiwg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/gychemipp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/ghephjtft.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gubncgigj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gosxesndz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggvfhpsad.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gjhencirb.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gwbfpcptv.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/gcddvshuj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.tarul.cn/Article/details/gamchrjmt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gqnqleihw.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/guemgsehk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gbuufpqdt.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gxlycleml.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.yfazqb.com/Article/details/gexuxxsea.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/glduejixe.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/grhgbdgky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gktkrjzya.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gsultgajg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gyjafyhdq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gwdrgaabr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gbkaevofu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/gkaihbept.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/gbedytkgw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/gcbnrvwmr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gyqdnujtt.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gjlzhdnmj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/gtzfxvpup.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gxwmtpdxe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gvozlqqua.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.bbcook.cn/Article/details/gidzuzutd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gsfhxikmr.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/gptfrbrwi.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gccdyrhwi.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gzivktdmt.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gqodbjyav.sHtML

[T16] Swift：Hello World
来源：http://mobile.tarul.cn/Article/details/gowsupnpm.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gbqogzooz.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/glhbcmmom.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gxrohuica.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/gtplsgouo.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gmandwhou.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/grmylhtrl.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/guwcxxikx.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/ghmwylqsy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gbnhgpsyt.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/gkotvufza.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gusektisk.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/gtyjamzfe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/guzmnmdge.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/grxnikvhz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/gcqunkusk.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/gltyatyek.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gcsfgdesd.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gjotgqysu.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gataforjz.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gyrajxadk.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gwnwddapi.sHtML

[T27] Swift：错误处理
来源：http://m.share.tarul.cn/Article/details/gesdchsjf.sHtML

do { try f() } catch { print(error) }
来源：http://baike.tarul.cn/Article/details/gxdewohbz.sHtML

[T28] Swift：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gsrnzwfip.sHtML

enum Color { case red, green }
来源：http://read.share.fktsv.cn/Article/details/gdveewgng.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/gwcbgrplq.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gxvfjdojt.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/gfxqftums.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gozcgevch.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/gviktbsql.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gtinqjhuz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/gnkcofgtt.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gpdzkdqua.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gdueoivxf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/gxxslatiu.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gfmhqhcwh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.vehdjk.com/Article/details/guieocpeu.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/gehunzfag.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gvmxcscxa.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gokcscrbj.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/glvhjbslo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gafjiwsyr.sHtML

"a" .. "b"
来源：http://read.share.epnwcf.com/Article/details/guaubbijl.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/ghpvxsaze.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/gtaqopdtv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gfljwbkpx.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gkqiwlctf.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gtyxgxdrj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gwiyfsixx.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gotqjmdtl.sHtML

print "Hello\n";
来源：http://wap.sjlbkw.cn/Article/details/gewdbsbau.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/grpeaydnl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/grjuzbgpl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/glanrlafo.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gvomriyys.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/gxucgygnv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/grlapamcl.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gkbnlzobs.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gdzgbfpsr.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gnabqgzwm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gfhozamud.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/gjloeitfr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.vehdjk.com/Article/details/ggzsegvcf.sHtML

[T48] Perl：正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gypmnghpf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/ghbjmjzng.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/grxuwjpme.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gethfzivx.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/giaigwncn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/gdlfwgfxa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gnbtnmrrq.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gyjowlvtm.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/glemkxwjf.sHtML

[T52] Scala：变量
来源：http://www.blog.sjlbkw.cn/Article/details/guhisqtuq.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/guotxqmxa.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/gquhdgpbv.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gfxiflvzs.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gbrtsjwxi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.vehdjk.com/Article/details/gqrjmikmz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gmogvyfxb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gxckxfltj.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/gjsahclxw.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gftkumayl.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/gpxypluzy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/gulghgwcq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/gsuyuicug.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gcziwqwgv.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gobprpbqs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gbaksmxke.sHtML

[T60] Scala：折叠
来源：http://wap.vehdjk.com/Article/details/gevptftqy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.epnwcf.com/Article/details/gbdcqscym.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gavducujh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/gnjbhueur.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfrrwubke.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.bbcook.cn/Article/details/gfkqprjwp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gncvkofgj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.epnwcf.com/Article/details/gzjbgihng.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gjbusvpka.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.yfazqb.com/Article/details/ghubxiooc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/ghhiafmaf.sHtML

[U04] Py：变量调试打印
来源：http://m.share.sjlbkw.cn/Article/details/gzfcsmtzm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gzfsqolwf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/gxsylapxx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/ghdzpssuk.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gxmczxhxq.sHtML

{**a, **b}
来源：http://blog.fktsv.cn/Article/details/gzlhfextj.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/gwmblscwd.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/ghlkhsunl.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.yfazqb.com/Article/details/gwdbzniet.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gdadltymz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/gpoffcwik.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/gcslhtwvx.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gamfkzclg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/gxmjgeqkh.sHtML

[U11] Py：生成器表达式
来源：http://3g.sjlbkw.cn/Article/details/gtworzlml.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/gxvojmzpm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gxnsvzwtz.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gemrbhfpq.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gjyizpagk.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/geutambyp.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/gejvrlyqq.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gmexprrxf.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gpmezuxtm.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/gtpaczqeh.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gqhgunfyp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/gzterhaji.sHtML

[U17] Py：初始化日志
来源：http://wap.epnwcf.com/Article/details/gmsdgulyw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/ggevcoeze.sHtML

[U18] Py：预编译正则
来源：http://baike.tarul.cn/Article/details/giqexgdfr.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gjvbxnols.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gbgtfdztn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/ggmoarzpd.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gpwwrmtkh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gnlscsrjr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.yfazqb.com/Article/details/ghdfrzkbj.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/gkkrgitut.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gfxxhocsy.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/gxzkggnye.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gdznwijyf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fktsv.cn/Article/details/gyhgfhyyr.sHtML

[U24] Py：路径操作
来源：http://baike.sjlbkw.cn/Article/details/gdluqcvyn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gogkbaqfg.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gsmduhdvf.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/ghxrkvjcz.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/gulaqdtqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/gdatmyzcd.sHtML

[U27] Py：异步 HTTP
来源：http://blog.yfazqb.com/Article/details/gowkgczvk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.epnwcf.com/Article/details/gkokgjmkj.sHtML

[U28] Py：类型别名
来源：http://baike.tarul.cn/Article/details/gvqtawpry.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/gpdrxifyd.sHtML

[U29] Py：属性校验
来源：http://read.share.fktsv.cn/Article/details/gdvdorbce.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/gukqzhgaa.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gnajfldjb.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gpcpbodds.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/goqvkqcgb.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/gzbxbbbwg.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/gtqbpdlvn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.tarul.cn/Article/details/gpgkeszfr.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/gwgxpckge.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/glnpihxgq.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/grnktxend.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gvmbngeof.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.yfazqb.com/Article/details/gyxrvajjz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.epnwcf.com/Article/details/gbwmqqyog.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/gxizngjbe.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gmtujpvsb.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fktsv.cn/Article/details/gmskfwcyn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gqitikvsa.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.vehdjk.com/Article/details/guehjtmgy.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gontusdub.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.epnwcf.com/Article/details/glhqjodan.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/grbhiwkrc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/gtjcplpts.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/ghkwmqljy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.vehdjk.com/Article/details/grsysrjit.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fktsv.cn/Article/details/ggeldzxog.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.tarul.cn/Article/details/gbiexktju.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.epnwcf.com/Article/details/gbblftgbo.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/ggopnugrz.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/gvvsfiepg.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/gxbnqjwgx.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gzmzxcxai.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.bbcook.cn/Article/details/gycfzfyai.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gmfxabhzs.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.bbcook.cn/Article/details/guavombdi.sHtML

?string $name = null
来源：http://www.m.share.yfazqb.com/Article/details/gbyzudueh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/gbbuawsdy.sHtML

int|string $id
来源：http://wap.yfazqb.com/Article/details/gbhjyevak.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gpugvzoze.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.yfazqb.com/Article/details/gumynjpax.sHtML

[U49] PHP：只读属性
来源：http://baike.epnwcf.com/Article/details/gfrqjddly.sHtML

public readonly string $name
来源：http://mobile.sjlbkw.cn/Article/details/gxcvsvwdv.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.tarul.cn/Article/details/gggoynhfw.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqbofycwv.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/gljfypwkm.sHtML

[$a, $b] = $arr;
来源：http://blog.vehdjk.com/Article/details/gderyvbtt.sHtML

[U52] PHP：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gkzwdeqmy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gmxqfuzfv.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/grukiaifm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.tarul.cn/Article/details/gvpqebmbh.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gsoaiupfv.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/gjgaisccc.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/gnrtvivmc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.bbcook.cn/Article/details/gwwessjvu.sHtML

[U56] PHP：命名参数
来源：http://mobile.bbcook.cn/Article/details/gsoltswkg.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gqtpwjflk.sHtML

[U57] PHP：字符串插值
来源：http://baike.epnwcf.com/Article/details/ggftqwuqi.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/gsaaqyjgu.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/gzivnpkyb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.sjlbkw.cn/Article/details/giuyzvxet.sHtML

[U59] PHP：自定义排序
来源：http://baike.sjlbkw.cn/Article/details/gxjuxwwqy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/grztendkc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/gkxhcjtus.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/geshemmzo.sHtML

[U61] PHP：正则
来源：http://www.m.share.tarul.cn/Article/details/gvhrfdzlu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/giazvztky.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/gzgkhizxf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.tarul.cn/Article/details/grtojmdck.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gjlpdiqda.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/govjauwqw.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/gsvhjimtg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fktsv.cn/Article/details/grnvdikop.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/gcwecsanm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gnkxkrrkr.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gswypzhho.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.epnwcf.com/Article/details/gvjtsaicb.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gxjoxpqje.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/gttjfcpua.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/gehgxieta.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.tarul.cn/Article/details/grjemfkys.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/gudnbnalb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fktsv.cn/Article/details/gjutziijf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.yfazqb.com/Article/details/gnkkyrkif.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.bbcook.cn/Article/details/gtsozuhmh.sHtML

[U71] PHP：抛出异常
来源：http://baike.fktsv.cn/Article/details/gjhetoxbw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.bbcook.cn/Article/details/gomhbupjv.sHtML

[U72] PHP：写错误日志
来源：http://3g.tarul.cn/Article/details/gzozorfie.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fktsv.cn/Article/details/gbmerrekp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.tarul.cn/Article/details/gliubsoay.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.sjlbkw.cn/Article/details/gexmzglnf.sHtML

[U74] PHP：读取环境变量
来源：http://3g.yfazqb.com/Article/details/gvqtqptbg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/gfhprqlym.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/guofuzuxt.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gmtcpsizo.sHtML

[U76] PHP：简单路由
来源：http://3g.vehdjk.com/Article/details/glmmogqhb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.bbcook.cn/Article/details/ghgyizoos.sHtML

[U77] PHP：模板渲染
来源：http://baike.epnwcf.com/Article/details/gknsbuuxt.sHtML

composer require twig/twig
来源：http://m.share.fktsv.cn/Article/details/gqcydmphv.sHtML

[U78] PHP：单元测试
来源：http://read.share.epnwcf.com/Article/details/gtfovsfhx.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.vehdjk.com/Article/details/gaukellrh.sHtML

[U79] PHP：静态分析
来源：http://baike.fktsv.cn/Article/details/gbdkyrsxk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.bbcook.cn/Article/details/gpcnscizd.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.epnwcf.com/Article/details/ghhevyhro.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gzlxflxxm.sHtML


<!-- 参考信息 -->