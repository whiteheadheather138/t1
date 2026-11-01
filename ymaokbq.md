代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gcljebihz.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gjgjiblsn.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gjudvkacm.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gabsxiugt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/glwoekabv.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gdukjklkt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/gaufvmbtu.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/grqsupazq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gxsnyeyys.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gpyxtwflz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gwlmxcqga.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/giatljfnx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gcatzudux.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gfexqpmpt.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gcmqdvwgs.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/glmzhiosq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gatdndsez.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gmlgcvram.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/grddsnmsq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.tarul.cn/Article/details/gethdcfks.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/ggbexsgsl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grblrjbzj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/gailrlwlk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmkhuvwxk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/grrqxykvo.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gktwhefyt.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/guywbpgzt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fktsv.cn/Article/details/gzwsazois.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gvuupoyfc.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gjmsdwyyp.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gjphjxlor.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gjlthzjmx.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gfqvaotxg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gkvuaqbkt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gwwdhzqhi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gbmqlpelq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gqegygilf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.sjlbkw.cn/Article/details/gbjyqulws.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/ggmcwncrr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gxhkwcgiq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gpybvfrjf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gumtqtpok.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/glurqweoa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gvsqdvnjn.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gnprdfbam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gayqyyjnz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gmbbhasgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gkqnmeuim.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/geggbqprn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/guhumxjvd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gigvfrsyl.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gsiqvwvig.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/ghwgckozo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.vehdjk.com/Article/details/grgluqcfv.sHtML

[T16] Swift：Hello World
来源：http://mobile.yfazqb.com/Article/details/gqlhedivf.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gnepyeyra.sHtML

[T17] Swift：变量与常量
来源：http://mobile.epnwcf.com/Article/details/gtbflqhxc.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/gmxmiprpp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gbuhhhyje.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gyivmffzn.sHtML

[T19] Swift：可选绑定
来源：http://mobile.sjlbkw.cn/Article/details/gsfdxtjyj.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gfzwcfnjw.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/getmvgfwz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/gliyorgbp.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/gmjzoaalh.sHtML

for x in a { print(x) }
来源：http://read.share.yfazqb.com/Article/details/grxdixywc.sHtML

[T22] Swift：字典
来源：http://www.share.fktsv.cn/Article/details/ggblmyaos.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gnxhozsde.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gewesbxif.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/getagjglu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gnclxhwui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gamtgxzap.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gppqsrzgo.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/grglpouez.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/giitfuryu.sHtML

class A: Base { override func f() {} }
来源：http://baike.epnwcf.com/Article/details/gmqevwwfn.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/ggrlgmwev.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/geiooxwwg.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gkuclloza.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gextsinbm.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gmjbujkmr.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gzrkrujob.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/gyzzbrcmg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.epnwcf.com/Article/details/gqftzhnvx.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gzrxpdcsq.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gnjojoqni.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gjzxousfy.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gdkzupjkj.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fktsv.cn/Article/details/glrrzzhfm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gnsqjwmkj.sHtML

[T34] Lua：遍历表
来源：http://wap.tarul.cn/Article/details/gppduihwc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/glebqyusy.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/gophwjfru.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gosdollrt.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gshnzzfct.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gmtvvumkv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gqsxcmvzx.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gzrijuzno.sHtML

[T38] Lua：条件
来源：http://www.m.share.tarul.cn/Article/details/gohzdhjtp.sHtML

if x > 0 then print("正") end
来源：http://www.blog.epnwcf.com/Article/details/gaxmokxtr.sHtML

[T39] Lua：模式匹配
来源：http://3g.bbcook.cn/Article/details/gnwunhhzm.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/ghknvawkg.sHtML

[T40] Lua：元表
来源：http://www.share.yfazqb.com/Article/details/gnbxiftvg.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gnlrhsibj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/geumbsazk.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gxhhuevvv.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gvkgotzdh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/girveszzz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gbcnwnjtp.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gnhkgadar.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/giwwingvt.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gohjdqzja.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/ganmgjmsn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.bbcook.cn/Article/details/gjjvagbjw.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gngaxbwlo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/grneleolz.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/gewqjfudg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gydkeqzqj.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/gkofyrjsk.sHtML

$s =~ s/old/new/g;
来源：http://blog.bbcook.cn/Article/details/gvnwjwunr.sHtML

[T49] Perl：函数
来源：http://mobile.vehdjk.com/Article/details/gwkcfhher.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gxsrezsdc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gfhdisggm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/giqisqjpy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.bbcook.cn/Article/details/grkoyyqpg.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/guzcutale.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gmikxxolh.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/gkticfbwj.sHtML

val a = 1;  var b = 2
来源：http://www.share.fktsv.cn/Article/details/gcdhpfyns.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/guqhepasz.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gwcitmdlv.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gylfkkaxs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.tarul.cn/Article/details/gsntzeqbh.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gmdoplngw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gsybmeree.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gkesbavas.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gxzlizbka.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/ghuqedmsk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gxdyggpar.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gpxrjqnyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.bbcook.cn/Article/details/glpualrpz.sHtML

[T59] Scala：循环
来源：http://www.blog.fktsv.cn/Article/details/gydgjsttd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gdjpmndkf.sHtML

[T60] Scala：折叠
来源：http://www.share.vehdjk.com/Article/details/grawmveqc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gnlldlxsb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwttwphxr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/getcprlwx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmbllwayi.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/gthdqmfii.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gpjbejogv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.sjlbkw.cn/Article/details/gldzokatv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/gtjjkxypq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.yfazqb.com/Article/details/gnztsnhoe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.tarul.cn/Article/details/gpvbjfcln.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gbihrginx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/gmxzdqasg.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gflcktyfz.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gvqecphaq.sHtML

[U06] Py：合并两个字典
来源：http://wap.sjlbkw.cn/Article/details/gdakacgtx.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gvtfaxvdd.sHtML

[U07] Py：反转字典键值
来源：http://www.share.tarul.cn/Article/details/gdicjimok.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/gdazhhjfm.sHtML

[U08] Py：展平二维列表
来源：http://blog.epnwcf.com/Article/details/gdghlgoyv.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/ghdsgzjbx.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/gzrefmcmk.sHtML

max(d, key=d.get)
来源：http://wap.tarul.cn/Article/details/ggxiilyvz.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gstlefvfp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gojaikukb.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gvqemzuef.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/glabfwuso.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gqesjorem.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gtxluvvmn.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gobfsdxgs.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/gvpiahrve.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gtlzdxzbq.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gnmnjazzd.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/ghjeaabvl.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gwmxribqr.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fktsv.cn/Article/details/gtykhlipu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/gqjftrawc.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gucargleo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fktsv.cn/Article/details/gtxmgcyqw.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gdozxvjym.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gsnhseuyc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.yfazqb.com/Article/details/gyzhxqxqy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.sjlbkw.cn/Article/details/gjwuqalsp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gmezcwcey.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/gjoswfyak.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.sjlbkw.cn/Article/details/gxcgwudfi.sHtML

@contextlib.contextmanager
来源：http://blog.fktsv.cn/Article/details/ggxmzcdde.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.vehdjk.com/Article/details/gmrykenlm.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gmldxktpr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fktsv.cn/Article/details/gxirdyqsx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/guueztidk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.bbcook.cn/Article/details/gxcwfmixr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gwpegozvd.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/gpkrhlfsk.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gggvfdqrk.sHtML

[U26] Py：并发下载
来源：http://wap.vehdjk.com/Article/details/gziaxsbcb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.epnwcf.com/Article/details/gclzzbpbx.sHtML

[U27] Py：异步 HTTP
来源：http://3g.yfazqb.com/Article/details/gwynqugmh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/ggbxxkejo.sHtML

[U28] Py：类型别名
来源：http://3g.sjlbkw.cn/Article/details/gzdtycpxa.sHtML

UserId = int
来源：http://m.share.sjlbkw.cn/Article/details/ggxtalgwh.sHtML

[U29] Py：属性校验
来源：http://3g.fktsv.cn/Article/details/gjolzoigl.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/gmeqozefz.sHtML

[U30] Py：数据类
来源：http://3g.yfazqb.com/Article/details/gbtmznfxo.sHtML

@dataclass(slots=True)
来源：http://read.share.vehdjk.com/Article/details/gzoowaklm.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gcyzfhuxk.sHtML

python -m pytest -q
来源：http://read.share.sjlbkw.cn/Article/details/gzcqlhhjr.sHtML

[U32] Py：代码格式化
来源：http://m.share.fktsv.cn/Article/details/glgbuobzz.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.vehdjk.com/Article/details/gonxnfnna.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/gwogozrrr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gynjowwhr.sHtML

[U34] Py：判断编码
来源：http://mobile.yfazqb.com/Article/details/ghvrdgubf.sHtML

chardet.detect(raw)
来源：http://blog.tarul.cn/Article/details/gfryipuoc.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/grsjnyuhi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gwvvpnddd.sHtML

[U36] Py：定时任务
来源：http://wap.tarul.cn/Article/details/gaborajti.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gqqjjbgmi.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.yfazqb.com/Article/details/glxjykkrp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gouhivwjs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.sjlbkw.cn/Article/details/gotpnmdbp.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gkrlgsstj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.sjlbkw.cn/Article/details/gqfuqfgbc.sHtML

sys.stdout.isatty()
来源：http://read.share.sjlbkw.cn/Article/details/gxnzibrhj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.vehdjk.com/Article/details/gnogidkff.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gncaghgwh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/gudeusoej.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/gpvwqehlh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.tarul.cn/Article/details/gbdcprcvg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.sjlbkw.cn/Article/details/gfolketok.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gnqzmdjoy.sHtML

namespace App\Http;
来源：http://blog.bbcook.cn/Article/details/gcxfyvgok.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/glciyqmmc.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/gflkaojmb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.tarul.cn/Article/details/grxljqvde.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gqbxoshkp.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gfvegbkpw.sHtML

?string $name = null
来源：http://m.share.fktsv.cn/Article/details/gsiwuwhew.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gpidfqkbz.sHtML

int|string $id
来源：http://blog.vehdjk.com/Article/details/giuqpfalq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.yfazqb.com/Article/details/gtgygpxec.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.sjlbkw.cn/Article/details/gfvmvdvzt.sHtML

[U49] PHP：只读属性
来源：http://mobile.vehdjk.com/Article/details/glnfhhfui.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gwbncziwl.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fktsv.cn/Article/details/gsalfnphl.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/glxiioqxs.sHtML

[U51] PHP：数组解构
来源：http://read.share.fktsv.cn/Article/details/gsprnrnlo.sHtML

[$a, $b] = $arr;
来源：http://blog.fktsv.cn/Article/details/gucawnuir.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/genzskytj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gbvihgeuq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.vehdjk.com/Article/details/gfhnsduoz.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.yfazqb.com/Article/details/gplemsive.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/guqfdqtzi.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gzipvhxtk.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.yfazqb.com/Article/details/geizhwezw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/gipvsifmd.sHtML

[U56] PHP：命名参数
来源：http://m.share.vehdjk.com/Article/details/gsygtgxmt.sHtML

f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gzhbjtxpo.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gunoklwem.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/guvmimgbo.sHtML

[U58] PHP：数组三件套
来源：http://3g.epnwcf.com/Article/details/gkeqbgjzy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gaxskzdey.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gyqhptyyk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gkxlbfwon.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/gsksqonvo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.epnwcf.com/Article/details/gwgsbbeit.sHtML

[U61] PHP：正则
来源：http://mobile.bbcook.cn/Article/details/gkrcnbydf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gihymhkxa.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gzetmaumu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.epnwcf.com/Article/details/gieekxzjz.sHtML

[U63] PHP：文件读写
来源：http://baike.bbcook.cn/Article/details/gyuiincvw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.bbcook.cn/Article/details/giiddhbcn.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fktsv.cn/Article/details/gcmgxlfrj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.tarul.cn/Article/details/glgqfozao.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gclejfwbt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gbzpvwnvg.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.epnwcf.com/Article/details/gkhdgkhkm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.bbcook.cn/Article/details/gjxiarexc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/gjgdujdar.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fktsv.cn/Article/details/gcnwkcddr.sHtML

[U68] PHP：PDO 连接
来源：http://wap.tarul.cn/Article/details/gfkdxtvjw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.bbcook.cn/Article/details/gfirqtcbb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.bbcook.cn/Article/details/gqowxaqid.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.vehdjk.com/Article/details/gquwwyisk.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.yfazqb.com/Article/details/gsoihrytr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmqrxile.sHtML

[U71] PHP：抛出异常
来源：http://mobile.epnwcf.com/Article/details/gaojwphgb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fktsv.cn/Article/details/gfdexfvyj.sHtML

[U72] PHP：写错误日志
来源：http://wap.fktsv.cn/Article/details/gvssdlkon.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/ghkliqcrt.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.bbcook.cn/Article/details/gvrkegpib.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.vehdjk.com/Article/details/gtvapqqwj.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gsnnokyzz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gdnqbkgyy.sHtML

[U75] PHP：依赖注入
来源：http://m.share.epnwcf.com/Article/details/grfhtdcky.sHtML

composer require psr/container
来源：http://read.share.vehdjk.com/Article/details/glulgrlva.sHtML

[U76] PHP：简单路由
来源：http://read.share.bbcook.cn/Article/details/gzvpovwod.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gdxqympaz.sHtML


<!-- 参考信息 -->