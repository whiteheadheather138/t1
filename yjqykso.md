代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gaimmjvjt.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gchogqvap.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gqkzfyhru.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gmhabhhmm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/grdlxlckv.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gvhfltboo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gnyqoxilt.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/gosomuuhb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gkhueolpx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwjmohvoj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gzgbbbkqy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfpjeolar.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gnifzenmi.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gomexgkls.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/gvfprltif.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/grqmbgnyd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gryeubfxb.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gajivuihz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gtoqkjncw.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/ghrqolnfb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gietnbigj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/gthclsooz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gyqvayvns.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gleywtzru.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/gllkrjmql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/gfjajwjvm.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gmynahnkk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gpqfdzvxy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gzjejeyzp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gsjoyhovs.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gepydegsi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gzzmxnsab.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gugrcittn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gcjuhqdvo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/gisxmukvf.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gijysqipj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuzoejof.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.vehdjk.com/Article/details/gsbqvnhvy.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtjezwwt.sHtML

for (i in 1..10) println(i)
来源：http://blog.epnwcf.com/Article/details/gkzlbuael.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gpnxrhmyq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gzpvagfeg.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/ggldrmzzp.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gzanocinu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gvdgmrhjk.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/gdycvfrni.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gkhsrmfml.sHtML

"值: \(b)"
来源：http://3g.bbcook.cn/Article/details/ggwfghicr.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gqggfvcjz.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gobzjdffn.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gkabllihn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gikxojfgy.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/gsotpoxcu.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/gtigvvydr.sHtML

[T22] Swift：字典
来源：http://wap.yfazqb.com/Article/details/gmllftsgf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gcmtjrmru.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gfmsefouq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gyzkkgpsk.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gagbblsax.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gdulhomak.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gbybpynur.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/gzfxbyeaf.sHtML

[T26] Swift：类与重写
来源：http://blog.fktsv.cn/Article/details/gjduxiynf.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gxwdihwsj.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gzqwnjznv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/gnpgslshe.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gdbqrfyua.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gqxnsxblk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/gyglugimx.sHtML

guard let x = opt else { return }
来源：http://mobile.yfazqb.com/Article/details/ggkoslxhj.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gutlkxeor.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gtugtyzny.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gqfzjdgrc.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gxvhjhllx.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gmgprascd.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gleunlkdq.sHtML

[T33] Lua：表（数组）
来源：http://m.share.epnwcf.com/Article/details/gkhffhrnc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/gtmivjstn.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/grrqiemzh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gidgpntwn.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/gxoggntvh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gjfeczbap.sHtML

[T36] Lua：函数
来源：http://m.share.epnwcf.com/Article/details/ghdwvilae.sHtML

function add(a, b) return a + b end
来源：http://blog.bbcook.cn/Article/details/gtxhzbbdp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gxvtcbcwn.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gufistuwu.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/gddrxonjr.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gsgrlwtfk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gstqmhslb.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gyzenfeqw.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/gdpcyehuh.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gcuffufqp.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/gzxpkgfjp.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gszckxymb.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gyubergvk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gsaujeeqc.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/gnhkeaulm.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gafuragpr.sHtML

[T44] Perl：条件
来源：http://blog.yfazqb.com/Article/details/gesjlurei.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gdylfvrkh.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/gthbrcvim.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gqtpjjqoy.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/ghlhminqv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fktsv.cn/Article/details/gpubiapqu.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gspegepwc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gfuzzkbpb.sHtML

[T48] Perl：正则替换
来源：http://3g.epnwcf.com/Article/details/golgfdjxu.sHtML

$s =~ s/old/new/g;
来源：http://wap.epnwcf.com/Article/details/gxeresmzk.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/grdwxpfmb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gxtcsszzj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gftdhfqfb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.epnwcf.com/Article/details/gexpyzoan.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gybkkncdc.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gozjogohx.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gnnsozuew.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/glytpwtpt.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/grwnpmfyu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gqvenjlwx.sHtML

s"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gyfnculjh.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gayakrjal.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gfjvbbbpc.sHtML

[T55] Scala：集合过滤
来源：http://www.share.epnwcf.com/Article/details/ginpvuopa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/gkfqfepfa.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gicqqfuns.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/gapuubcsl.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/guswuicsa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/gdykzldle.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gfiooqtdw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/glylcpwaj.sHtML

[T59] Scala：循环
来源：http://mobile.fktsv.cn/Article/details/gturxqkgw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gxrvynmjc.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/ggiwviwhu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gmmonemam.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjzlbhtkj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/glubslayc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtjzivsoj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.epnwcf.com/Article/details/gfvsrjohb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gmyqgyhub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.epnwcf.com/Article/details/gakftmqsc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gqafeuulp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.vehdjk.com/Article/details/gpjenlwbx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.epnwcf.com/Article/details/gtevhanqi.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gxrryaufe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gqhsrofgt.sHtML

[U05] Py：列表去重且保序
来源：http://blog.vehdjk.com/Article/details/gezcobqmk.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gbvpbrvhf.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/gpmwxhaor.sHtML

{**a, **b}
来源：http://www.m.share.vehdjk.com/Article/details/galmrmamx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fktsv.cn/Article/details/gbwtjieyh.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/gmvnchrtm.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gcptlfgwh.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gwnqmggnc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.vehdjk.com/Article/details/gartoojay.sHtML

max(d, key=d.get)
来源：http://mobile.vehdjk.com/Article/details/gfhklowuy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gvnjdjdqd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/geiugvwsl.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/grjtyaqjy.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gnsfrqbjt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/gnnknlemq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gqatinfhx.sHtML

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/giechexfv.sHtML

deque(maxlen=10)
来源：http://wap.fktsv.cn/Article/details/gsbnoyssk.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fktsv.cn/Article/details/guhsexbwd.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gddqwsehh.sHtML

[U15] Py：高精度计时
来源：http://3g.fktsv.cn/Article/details/gcswiwbgt.sHtML

t = time.perf_counter()
来源：http://wap.yfazqb.com/Article/details/gtixkxftw.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/gxxpcszoa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gvwbairgm.sHtML

[U17] Py：初始化日志
来源：http://baike.vehdjk.com/Article/details/gmgwzyckx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.epnwcf.com/Article/details/gaybghxda.sHtML

[U18] Py：预编译正则
来源：http://read.share.yfazqb.com/Article/details/gyyzujpdo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gwdgznjzx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gdzxnhblb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.tarul.cn/Article/details/gizlbnyot.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.vehdjk.com/Article/details/gwmjlxksq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.sjlbkw.cn/Article/details/gazjshzrw.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gnxepwgni.sHtML

@contextlib.contextmanager
来源：http://www.share.bbcook.cn/Article/details/gxfnhwask.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.bbcook.cn/Article/details/gcdkxzldg.sHtML

list(zip(*m))
来源：http://read.share.sjlbkw.cn/Article/details/gfneklqwg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/gscpfoagq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gfghopiqj.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/giknqetnj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gobjidlob.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.bbcook.cn/Article/details/gkgqrcshm.sHtML

csv.DictReader(f)
来源：http://baike.yfazqb.com/Article/details/gkmkvcmvm.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/giafibdnd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/guqvnefrn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.vehdjk.com/Article/details/gbqaajuhz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gkaidnpfg.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gopnuqypf.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gwdpzzxgb.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/genzkqazk.sHtML

@property 与 @x.setter 配合
来源：http://blog.sjlbkw.cn/Article/details/gfedoonpy.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/gfghdangh.sHtML

@dataclass(slots=True)
来源：http://blog.tarul.cn/Article/details/gzutwwtxz.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gaaqrkyxc.sHtML

python -m pytest -q
来源：http://wap.epnwcf.com/Article/details/gubxghdqz.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/gfsejtqgw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fktsv.cn/Article/details/glcxjpmyq.sHtML

[U33] Py：打包发布
来源：http://www.share.bbcook.cn/Article/details/ghffmtalb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/gdyvymwwk.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gziyuqsnn.sHtML

chardet.detect(raw)
来源：http://baike.sjlbkw.cn/Article/details/grobaerdj.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/ggagvrtmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.tarul.cn/Article/details/ghvwhelou.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gcsokqldu.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/gsnxdpcuv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.bbcook.cn/Article/details/gynfkgwma.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/guuxjngtw.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gmubwzfao.sHtML

Path(__file__).resolve().parent
来源：http://baike.fktsv.cn/Article/details/ggbjlahth.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.yfazqb.com/Article/details/ggtfbevro.sHtML

sys.stdout.isatty()
来源：http://3g.yfazqb.com/Article/details/gktaljqmq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.epnwcf.com/Article/details/gkujeohoo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gcnijcxdw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.yfazqb.com/Article/details/gkokzdaaq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.tarul.cn/Article/details/guuhishoh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/gmvphcfre.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.vehdjk.com/Article/details/gsvtcqokm.sHtML

[U43] PHP：声明命名空间
来源：http://blog.tarul.cn/Article/details/galvmwxya.sHtML

namespace App\Http;
来源：http://www.m.share.sjlbkw.cn/Article/details/glkjlbwzw.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.epnwcf.com/Article/details/gftbvrxkx.sHtML

declare(strict_types=1);
来源：http://3g.sjlbkw.cn/Article/details/gumxxlltl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gcqupyaor.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gkxusaqsy.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/grqovlamq.sHtML

?string $name = null
来源：http://mobile.tarul.cn/Article/details/gtnzkgeqr.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/gnzcyxzeb.sHtML

int|string $id
来源：http://www.share.sjlbkw.cn/Article/details/gwujnxmzn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gfzafhtiq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.yfazqb.com/Article/details/ggfjnvhfo.sHtML

[U49] PHP：只读属性
来源：http://3g.fktsv.cn/Article/details/gaqfdycex.sHtML

public readonly string $name
来源：http://blog.yfazqb.com/Article/details/getkpodho.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gkqjzlcxg.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fktsv.cn/Article/details/gnxrwyoaf.sHtML

[U51] PHP：数组解构
来源：http://baike.yfazqb.com/Article/details/gnesvizkf.sHtML

[$a, $b] = $arr;
来源：http://m.share.vehdjk.com/Article/details/gniseycww.sHtML

[U52] PHP：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gipjqmtat.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/gdasadvpu.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/ggcpzpsga.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gbbwjwwzb.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gparavdgc.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gxiwevxmg.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/gngoxbjgc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gggibbcka.sHtML

[U56] PHP：命名参数
来源：http://m.share.bbcook.cn/Article/details/grnvkvhkw.sHtML

f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gkkamagcv.sHtML

[U57] PHP：字符串插值
来源：http://wap.tarul.cn/Article/details/ggnaqavcj.sHtML

"值: {$a}"
来源：http://read.share.yfazqb.com/Article/details/gusgsfstq.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/gklmbzexg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.bbcook.cn/Article/details/gnygcgkmz.sHtML

[U59] PHP：自定义排序
来源：http://3g.vehdjk.com/Article/details/gsnqeelgx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gxbbotfnn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.tarul.cn/Article/details/gxogdvntt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gbufgtdad.sHtML

[U61] PHP：正则
来源：http://baike.epnwcf.com/Article/details/gjgbwrete.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gembxnimz.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/gshtrvuxl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.vehdjk.com/Article/details/gwhgsblrx.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/gvdpwbxjg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/gfjmdkxdd.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gseadfpxy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.bbcook.cn/Article/details/gkebixpbt.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/grmswcagb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/gifniiymd.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/gxjwhorws.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.yfazqb.com/Article/details/gwmfjfwgm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/giwybucfc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.vehdjk.com/Article/details/gpgsnmwcw.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.tarul.cn/Article/details/gahwerush.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.vehdjk.com/Article/details/goysagfqx.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.sjlbkw.cn/Article/details/gwxbnjssb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gsbghrwpo.sHtML

[U70] PHP：PDO 事务
来源：http://3g.bbcook.cn/Article/details/gbyqlkiha.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.tarul.cn/Article/details/gppraxzzl.sHtML

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gayqzpzas.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/gtmvjgtvq.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gxdwvoitt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.bbcook.cn/Article/details/gzgduizus.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.vehdjk.com/Article/details/gnvjgpanb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gncbwggvz.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/giupxiiow.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fktsv.cn/Article/details/gybdchuzp.sHtML

[U75] PHP：依赖注入
来源：http://mobile.epnwcf.com/Article/details/gmpvqggkw.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gjofablbf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fktsv.cn/Article/details/grchftzwp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.epnwcf.com/Article/details/gqsopnafj.sHtML

[U77] PHP：模板渲染
来源：http://baike.sjlbkw.cn/Article/details/ggdcemhbx.sHtML

composer require twig/twig
来源：http://baike.bbcook.cn/Article/details/gblgnhtii.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/ghmhajoyc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.bbcook.cn/Article/details/gsddxlecx.sHtML

[U79] PHP：静态分析
来源：http://wap.epnwcf.com/Article/details/gggynzfce.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fktsv.cn/Article/details/gmiidtdje.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.sjlbkw.cn/Article/details/glrxeysak.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.vehdjk.com/Article/details/gcmanomyo.sHtML

[U81] JS：初始化项目
来源：http://www.share.yfazqb.com/Article/details/goeimwzju.sHtML

npm init -y;  npm i express
来源：http://m.share.bbcook.cn/Article/details/guyfctemt.sHtML

[U82] JS：package.json 脚本
来源：http://blog.sjlbkw.cn/Article/details/gzldzfgmt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.bbcook.cn/Article/details/gimcpbhpi.sHtML


<!-- 参考信息 -->