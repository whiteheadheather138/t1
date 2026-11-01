代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gftjoxpbd.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gozizhrvl.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/guiyenzak.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gfjtdyccd.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gfqhabaud.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/ghadxxvie.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/gxhvngkxa.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gdkwtofol.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/glsyhtbwo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gucspvhdw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gvsvglqdi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gygiqntnd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.epnwcf.com/Article/details/gbzewaswt.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gelhgzord.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/grjubykan.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gyapjvcbf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gwyuuvxpl.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gqfvxmwop.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gtcsqxbyi.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/guiazrxzy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.epnwcf.com/Article/details/gunjbfhud.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/gqcmsbtjb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gvitssaft.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gcvoxtcwc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/gbvofneom.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gmhsrkgvs.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/glejitvxh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gqmncvawl.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gaycsfart.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/grgqpzmah.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gogjwazhr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/gaualrusp.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/genkyjuqy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.sjlbkw.cn/Article/details/gfvxvnfog.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.epnwcf.com/Article/details/grdqumuhy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gvbouhxuq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/glanheozo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gxfilfeng.sHtML

[T14] Kotlin：循环
来源：http://wap.sjlbkw.cn/Article/details/gnrdwfmps.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gurjmewnq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.tarul.cn/Article/details/gegdershx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gwmjtakxk.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gdwqydjxb.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gixlzbtiv.sHtML

[T17] Swift：变量与常量
来源：http://wap.sjlbkw.cn/Article/details/gviukjdkc.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/gwistabhm.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gndzxdesd.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/gyevfilvb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gskdwhwac.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/gwofzlwpr.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/guarxcfjl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gjmvnquuw.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gyjpgnaqq.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/gkcxvmlve.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/guhfavckl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gqsitlcnz.sHtML

[T23] Swift：函数
来源：http://baike.yfazqb.com/Article/details/gngbymkqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gztnsvpob.sHtML

[T24] Swift：闭包
来源：http://www.share.bbcook.cn/Article/details/ghqsvrjia.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gsomnjpbd.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gnvkmkjam.sHtML

struct P { var x: Int }
来源：http://www.blog.yfazqb.com/Article/details/graiefrjq.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/gknercfmh.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gybidrjtr.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gzchjugvv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/garfkngmq.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gwglvlbck.sHtML

enum Color { case red, green }
来源：http://www.share.fktsv.cn/Article/details/gektlwqmb.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/guzdgqwfj.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gqqwbzxew.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gkhxbqbhb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.vehdjk.com/Article/details/gsokkfumi.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gcawlvlbb.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/glmhfjmjl.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/ggveqhijx.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gkugiciyu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/ghsupfcdu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/gldggwqnu.sHtML

[T34] Lua：遍历表
来源：http://3g.sjlbkw.cn/Article/details/glsveiqxo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/gpptutbvj.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/goxvwxvey.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/gfwtcbgbj.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gccqqqsah.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/gyojqvmcv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gydmbuksa.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/gmwaldror.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gtstktfsi.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/grjkvbwrg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gbijdfzex.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gjqmetmfi.sHtML

[T40] Lua：元表
来源：http://blog.epnwcf.com/Article/details/gebakswxf.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/grwefstgo.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gwgqpyhtz.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gttfvummx.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/gzemzfdvc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gqrmklazc.sHtML

[T43] Perl：字符串插值
来源：http://blog.tarul.cn/Article/details/gvlmqpdqb.sHtML

"值: $a"
来源：http://m.share.yfazqb.com/Article/details/gqggrezvn.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/gxttjobya.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.epnwcf.com/Article/details/gpmolztaj.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/gccwihjkp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.tarul.cn/Article/details/gxsnaauio.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gabnpmpzl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/ggmphkpqm.sHtML

[T47] Perl：正则捕获
来源：http://m.share.tarul.cn/Article/details/gjpgdgbyc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gvtabfkis.sHtML

[T48] Perl：正则替换
来源：http://3g.bbcook.cn/Article/details/gsgenrkvn.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gazroktih.sHtML

[T49] Perl：函数
来源：http://3g.tarul.cn/Article/details/gsaembmia.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gzohahlfg.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gbczmouqp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.epnwcf.com/Article/details/gweqmqcps.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gqbcntntn.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/gvchcuvok.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gikfxsjjc.sHtML

[T52] Scala：变量
来源：http://baike.vehdjk.com/Article/details/gntvxsoty.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gzlcadwqy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.tarul.cn/Article/details/gcxjxxvsa.sHtML

s"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gxqqpfklp.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gxxymchta.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.epnwcf.com/Article/details/ggjofqchn.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/geaqdrsfp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gggkjhdeh.sHtML

[T56] Scala：样例类
来源：http://www.share.bbcook.cn/Article/details/gihmdiphy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gdbdhekmv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gbygwbqdi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gpkxgtnfh.sHtML

[T58] Scala：函数定义
来源：http://wap.epnwcf.com/Article/details/gvnztvjhi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.bbcook.cn/Article/details/gglnzjucs.sHtML

[T59] Scala：循环
来源：http://read.share.yfazqb.com/Article/details/gpsisxsjn.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/grjapglye.sHtML

[T60] Scala：折叠
来源：http://read.share.bbcook.cn/Article/details/gybfriwzd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/gtdwfygvp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gapvujmbw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gtwqetftx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjwmagoin.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.yfazqb.com/Article/details/gyhmwsnsn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/gxmftozcc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.epnwcf.com/Article/details/gyxewoppb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/gwahecara.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.yfazqb.com/Article/details/ghyvoighp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.vehdjk.com/Article/details/gpazleedj.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gxxwyhyqd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.bbcook.cn/Article/details/gphvgkkfs.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/geyblndnn.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsskfsto.sHtML

[U06] Py：合并两个字典
来源：http://blog.sjlbkw.cn/Article/details/gwctvlnca.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gqzwhfswa.sHtML

[U07] Py：反转字典键值
来源：http://www.share.epnwcf.com/Article/details/gxnqtjrjn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.vehdjk.com/Article/details/gypibvqne.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/gmwbbrjqp.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/gvabkbvzj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.bbcook.cn/Article/details/gbfaaqepz.sHtML

max(d, key=d.get)
来源：http://blog.tarul.cn/Article/details/gxdppnmaf.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gqocpzixc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gdmnkoywz.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.vehdjk.com/Article/details/gvbgumwig.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/gxzglsbwv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.epnwcf.com/Article/details/gdjunbpsk.sHtML

Counter(arr).most_common(3)
来源：http://www.share.vehdjk.com/Article/details/gagfkfotg.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/ggwszjrgj.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gfoqwdjmv.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.bbcook.cn/Article/details/gwxeoxgqf.sHtML

defaultdict(list)
来源：http://wap.epnwcf.com/Article/details/gxrwhlcjt.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gykosvbtl.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/gjvlkqimo.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gloicfqrz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gsndrkhaf.sHtML

[U17] Py：初始化日志
来源：http://www.blog.sjlbkw.cn/Article/details/gprbvwjei.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.sjlbkw.cn/Article/details/gmxzlhpvc.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gdlqynpqa.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fktsv.cn/Article/details/gkwjzotgj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fktsv.cn/Article/details/gmoduxbfm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.sjlbkw.cn/Article/details/gskkpqzto.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/grzbqxckk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gtsjzehjj.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gfmppxwzl.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gpumrzsjn.sHtML

[U22] Py：矩阵转置
来源：http://mobile.sjlbkw.cn/Article/details/gnvsuwsit.sHtML

list(zip(*m))
来源：http://m.share.bbcook.cn/Article/details/gzquuexso.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.sjlbkw.cn/Article/details/gorpbreqr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.bbcook.cn/Article/details/gdxnpuzke.sHtML

[U24] Py：路径操作
来源：http://m.share.vehdjk.com/Article/details/gratdhuln.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/ghxrxoeba.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.epnwcf.com/Article/details/gftupfvdg.sHtML

csv.DictReader(f)
来源：http://m.share.vehdjk.com/Article/details/gcyurcxwi.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fktsv.cn/Article/details/gqswupaps.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.bbcook.cn/Article/details/gtfedjize.sHtML

[U27] Py：异步 HTTP
来源：http://blog.yfazqb.com/Article/details/guufegfxw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.sjlbkw.cn/Article/details/gabuylecb.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/gyerotlun.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gdmillscp.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/gbuqyzvwr.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gnackzfdv.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/glllolxpt.sHtML

@dataclass(slots=True)
来源：http://m.share.bbcook.cn/Article/details/gmjvyeabg.sHtML

[U31] Py：单测
来源：http://blog.yfazqb.com/Article/details/gktcaaese.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/ghfoykcli.sHtML

[U32] Py：代码格式化
来源：http://mobile.bbcook.cn/Article/details/geofjjtlj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.yfazqb.com/Article/details/gpxaznaym.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/grapcmtyz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/gtjnwbbkl.sHtML

[U34] Py：判断编码
来源：http://m.share.vehdjk.com/Article/details/gxtymdcup.sHtML

chardet.detect(raw)
来源：http://3g.yfazqb.com/Article/details/guhicgxoy.sHtML

[U35] Py：发送邮件
来源：http://wap.tarul.cn/Article/details/gpvgivyzl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.sjlbkw.cn/Article/details/getfeclki.sHtML

[U36] Py：定时任务
来源：http://wap.epnwcf.com/Article/details/gioyzucqr.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.bbcook.cn/Article/details/gpxkdenca.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/gzqtzkyxy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.sjlbkw.cn/Article/details/gutkuivui.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/gzmwdlvgk.sHtML

Path(__file__).resolve().parent
来源：http://3g.epnwcf.com/Article/details/glghtvzhy.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/grxicunxi.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/gblzkinfz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.epnwcf.com/Article/details/gxcfyqbic.sHtML

print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gymchnjnq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.sjlbkw.cn/Article/details/ghuzdmrrg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.bbcook.cn/Article/details/gjpqtmbzo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gmhnwsppi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.bbcook.cn/Article/details/gpzamvmin.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.epnwcf.com/Article/details/gmsxmtisu.sHtML

namespace App\Http;
来源：http://www.share.yfazqb.com/Article/details/gmkkjqffu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gqmseenej.sHtML

declare(strict_types=1);
来源：http://baike.sjlbkw.cn/Article/details/gjczbzskz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.vehdjk.com/Article/details/gplukdfcl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gvowalvmi.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.tarul.cn/Article/details/gjcfyunft.sHtML

?string $name = null
来源：http://read.share.tarul.cn/Article/details/gnylbizhy.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/grmouxdnj.sHtML

int|string $id
来源：http://www.share.vehdjk.com/Article/details/ghaijessj.sHtML

[U48] PHP：纯枚举
来源：http://mobile.yfazqb.com/Article/details/gqdwwaitu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcaazgfg.sHtML

[U49] PHP：只读属性
来源：http://m.share.bbcook.cn/Article/details/gcbehdbwr.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gvcimxhks.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/geygjurqs.sHtML

public function __construct(private int $id) {}
来源：http://baike.fktsv.cn/Article/details/grpiqrgpa.sHtML

[U51] PHP：数组解构
来源：http://3g.fktsv.cn/Article/details/gekadgnbe.sHtML

[$a, $b] = $arr;
来源：http://baike.fktsv.cn/Article/details/gpwaksyfy.sHtML

[U52] PHP：箭头函数
来源：http://m.share.tarul.cn/Article/details/gvfnjxira.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.tarul.cn/Article/details/gzuhbiqrw.sHtML

[U53] PHP：空合并运算符
来源：http://wap.epnwcf.com/Article/details/gtyzbrtoa.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.vehdjk.com/Article/details/grujuysth.sHtML

[U54] PHP：空安全调用
来源：http://wap.vehdjk.com/Article/details/ghidigkcb.sHtML

$obj?->method()
来源：http://3g.vehdjk.com/Article/details/gepiowqjw.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/gqqnyoqtn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gfqccrnok.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gpwusaceg.sHtML

f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gkiqgjzho.sHtML

[U57] PHP：字符串插值
来源：http://mobile.bbcook.cn/Article/details/guwxvczgy.sHtML

"值: {$a}"
来源：http://blog.tarul.cn/Article/details/gstrrkcxe.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/goeakksxw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gifejajrs.sHtML

[U59] PHP：自定义排序
来源：http://blog.yfazqb.com/Article/details/gqjoymlhe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gdiuzevtq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/gjzuvftgi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/goejddiil.sHtML

[U61] PHP：正则
来源：http://www.m.share.yfazqb.com/Article/details/gvynsaxje.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/ghpqhttym.sHtML

[U62] PHP：日期对象
来源：http://3g.tarul.cn/Article/details/ggnkcfjnw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.vehdjk.com/Article/details/geqhusajw.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gixyoplhf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/gcfqmpcuy.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fktsv.cn/Article/details/gtsrejoze.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.sjlbkw.cn/Article/details/ggqquywyv.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gznlloqwl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gmyejrbcl.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fktsv.cn/Article/details/gxshbvthq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/ghhihskgm.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fktsv.cn/Article/details/gxbyqlozu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.vehdjk.com/Article/details/gxoshmaci.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gmnhlbrot.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.tarul.cn/Article/details/gfmgsuryn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.bbcook.cn/Article/details/gulmtsybe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gpborfxxs.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/gbjaebqvc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.sjlbkw.cn/Article/details/gqunfseis.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gyeznjbju.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/gilodsojv.sHtML

[U72] PHP：写错误日志
来源：http://wap.fktsv.cn/Article/details/grjbmkozd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.tarul.cn/Article/details/gaxmrcjzj.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.tarul.cn/Article/details/gymqocgkt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/goeaifodc.sHtML

[U74] PHP：读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/gbdeoyjdn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.yfazqb.com/Article/details/gdsaepugh.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/gkarmsjuz.sHtML

composer require psr/container
来源：http://3g.bbcook.cn/Article/details/gvnnhlrdu.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gscjcjogb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/gvdspouvo.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gscuvbnjz.sHtML

composer require twig/twig
来源：http://m.share.tarul.cn/Article/details/gyxelwjwq.sHtML

[U78] PHP：单元测试
来源：http://baike.fktsv.cn/Article/details/gzfmiziug.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.vehdjk.com/Article/details/ggckdjcqy.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gtlrroddv.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/gjblgedjx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.epnwcf.com/Article/details/gquvpdjbe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.tarul.cn/Article/details/gnjfbaoze.sHtML

[U81] JS：初始化项目
来源：http://3g.epnwcf.com/Article/details/gwxfhibfw.sHtML

npm init -y;  npm i express
来源：http://mobile.epnwcf.com/Article/details/gudkeksub.sHtML

[U82] JS：package.json 脚本
来源：http://baike.tarul.cn/Article/details/gkwtsouex.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/gpgnotfur.sHtML


<!-- 参考信息 -->