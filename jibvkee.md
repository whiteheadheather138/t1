代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.vehdjk.com/Article/details/gxejviuds.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gccpstjdr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gekbiuipy.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/glqwxaazc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/ghkwppwjd.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gxiwjiili.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gesjoedvw.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gljxnurpp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gwcvrpwtc.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gtqwtxsrt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gnszwwrsu.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/grzpakjlo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gnyjqmzwg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glqbxdftr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gwzuevoai.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyomomnkd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.bbcook.cn/Article/details/gyjmvulgj.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gzdgivqsd.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/geesepawz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gokmnmzbj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gkiacsiqm.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gbqjmzyet.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gdofumpvn.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/gbfunvmqf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gqjbfzywj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gzlbaezmv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gqslpwddc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gpyprvbid.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gyyydwrqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/gxiwnyomh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/ggssivwjd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gsrdouhay.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gwwwqsufw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/glqtepoqm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gxwsxfgou.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gwatvvhec.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/giwbdknwc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/gbygnxxyc.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gwfsbhjxa.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/glqqnsgff.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gczzvbgpb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/gqoqywsej.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gjydobhzp.sHtML

for (i in 1..10) println(i)
来源：http://baike.tarul.cn/Article/details/grsifvkrg.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gpgclxpth.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gfvwvgfiq.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gbuicsywf.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/ghdhpmwnz.sHtML

[T17] Swift：变量与常量
来源：http://blog.fktsv.cn/Article/details/gznipexke.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/gmumryhtu.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/ggcpvnsnm.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/gbezgxcty.sHtML

[T19] Swift：可选绑定
来源：http://3g.bbcook.cn/Article/details/glphptxmb.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/guutnkakp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/geingukto.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gmckflpny.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsnmpikt.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gfvclvdgu.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gsexakiil.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/gzluegacd.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/govhqtxxs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/girobioab.sHtML

[T24] Swift：闭包
来源：http://wap.vehdjk.com/Article/details/gjhzipymn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gdmattniw.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gvirlkrph.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gfbzpfvih.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gznnaghmn.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gfimrpdia.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/gfssvmvrb.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gniagztjp.sHtML

[T28] Swift：枚举
来源：http://3g.epnwcf.com/Article/details/gdkklbyfr.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gqqysxirs.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gipqfwehe.sHtML

guard let x = opt else { return }
来源：http://m.share.tarul.cn/Article/details/gjbxotixq.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gxexsztua.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxtwbdsx.sHtML

[T31] Lua：Hello World
来源：http://m.share.tarul.cn/Article/details/gdrzbibul.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gqrsffriv.sHtML

[T32] Lua：局部变量
来源：http://mobile.fktsv.cn/Article/details/gbnrbidiy.sHtML

local a = 1
来源：http://mobile.sjlbkw.cn/Article/details/gaepgwsfq.sHtML

[T33] Lua：表（数组）
来源：http://m.share.yfazqb.com/Article/details/geyjortzt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/gymefupad.sHtML

[T34] Lua：遍历表
来源：http://wap.yfazqb.com/Article/details/gwdizgcto.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.yfazqb.com/Article/details/gwqenxpfs.sHtML

[T35] Lua：字典表
来源：http://read.share.vehdjk.com/Article/details/gwwhaiexs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/gdvvihfmz.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/gwlcdnven.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gtundsfvv.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fktsv.cn/Article/details/goivffajm.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/gdfislpzw.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gdgiunhgd.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gwfmcfzys.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gdkfgdxqc.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gdrjgempo.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/gaqigubyq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fktsv.cn/Article/details/ghfmegixs.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/gvlyzhaks.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/gplfjkxfz.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/gvvqhzqdy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.vehdjk.com/Article/details/glfdkijko.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gnuqvnntl.sHtML

"值: $a"
来源：http://blog.sjlbkw.cn/Article/details/gbqvethcu.sHtML

[T44] Perl：条件
来源：http://mobile.fktsv.cn/Article/details/gwqvmjsaw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.yfazqb.com/Article/details/gjjpjbmxf.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gljuaudka.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.vehdjk.com/Article/details/ggohnlwyq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.bbcook.cn/Article/details/gqhgrwqct.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/glytfrweb.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gjggbksgp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gtsvhwqil.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gnhnfcqqd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gaxvfesvf.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gkiijgxvg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gnkbkrfth.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/goslcducd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/gikybrrfq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.tarul.cn/Article/details/gfcgdjyol.sHtML

[T51] Scala：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gqtrdyqqa.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gwxfhbvne.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/ghvptohie.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gjibruxpl.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/gktbaokts.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gkoktvdvg.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gaesjfipm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gqdicmlrs.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gefnfoxvf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.epnwcf.com/Article/details/gqftlhsoc.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/gvopvwufa.sHtML

case class User(name: String, age: Int)
来源：http://wap.epnwcf.com/Article/details/gyahjhqdy.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/gcwmkjmsj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/gkbqznuvr.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/gbkqgdchv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fktsv.cn/Article/details/gevidovjh.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/ggvpkphaa.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gsojfhslv.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gtuddccyd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/glyyomamn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gscmbkvzq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/grkqhvuhn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gystptnbv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gcnxtyenx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gavscwozv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.bbcook.cn/Article/details/gvicibbax.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.bbcook.cn/Article/details/gecsutifx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gkxkzbxfo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gbrlvpltg.sHtML

[U04] Py：变量调试打印
来源：http://3g.fktsv.cn/Article/details/gijnigtql.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gviecsntm.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/gfryuchnh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gnxobgplh.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/ggsubgdat.sHtML

{**a, **b}
来源：http://blog.epnwcf.com/Article/details/gljowrjun.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/ggsstpgry.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.vehdjk.com/Article/details/gzymadhgv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fktsv.cn/Article/details/ggubzppjg.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gqxwwamvp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/gxylqcomb.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/gpepfdhes.sHtML

[U10] Py：按值排序字典
来源：http://mobile.tarul.cn/Article/details/gdtcmahrw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/gbogreyla.sHtML

[U11] Py：生成器表达式
来源：http://baike.fktsv.cn/Article/details/gmiotkjfp.sHtML

(x * 2 for x in arr)
来源：http://blog.bbcook.cn/Article/details/gokhwslfk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.epnwcf.com/Article/details/geyizkvoc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gkxvttqdq.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/guraxcyne.sHtML

deque(maxlen=10)
来源：http://blog.tarul.cn/Article/details/gnwuvabqc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/ghjaqsirw.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gvepsnfxz.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gnliztbub.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gxeqkrczc.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fktsv.cn/Article/details/gooqojnim.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gzwanllzb.sHtML

[U17] Py：初始化日志
来源：http://wap.sjlbkw.cn/Article/details/gvrrxxfok.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gwxgajazq.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gfszrvhlz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gcshxfjwl.sHtML

[U19] Py：正则替换带回调
来源：http://wap.epnwcf.com/Article/details/gpuvhpwhm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gmsyqpzgt.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.tarul.cn/Article/details/gtubnqnzz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.epnwcf.com/Article/details/gxyiwlmhh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/getjvawit.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/gonhzxump.sHtML

[U22] Py：矩阵转置
来源：http://www.share.vehdjk.com/Article/details/grtewmzev.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/giaovftuf.sHtML

[U23] Py：分块读取大文件
来源：http://wap.epnwcf.com/Article/details/gmdwdddxc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.epnwcf.com/Article/details/gttfzgdax.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/gzrtaipdy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gkkauazrf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/giypqjzyr.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gjpjsusvf.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/gpdjzxzjy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gfmyxxcdp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/glmmsscqd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.yfazqb.com/Article/details/gpoyioezx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fktsv.cn/Article/details/gqzcysygt.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/gpypucytr.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gxutshhhc.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/ggymtxwgn.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/griydqfmc.sHtML

@dataclass(slots=True)
来源：http://baike.epnwcf.com/Article/details/gkrqdcrpo.sHtML

[U31] Py：单测
来源：http://www.m.share.sjlbkw.cn/Article/details/grcmkfhbg.sHtML

python -m pytest -q
来源：http://mobile.vehdjk.com/Article/details/ghlplygxt.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.vehdjk.com/Article/details/gkwbbjlvf.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fktsv.cn/Article/details/gbkhhyqoc.sHtML

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gkgvajurc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/grijgzdiw.sHtML

[U34] Py：判断编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsevvers.sHtML

chardet.detect(raw)
来源：http://read.share.epnwcf.com/Article/details/ghcbwault.sHtML

[U35] Py：发送邮件
来源：http://read.share.vehdjk.com/Article/details/guodrasid.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.bbcook.cn/Article/details/geaocdxdj.sHtML

[U36] Py：定时任务
来源：http://3g.bbcook.cn/Article/details/gyfiprztl.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/gwzfwhpvd.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/grfmudrdc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gtjsuthuu.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.tarul.cn/Article/details/gkanltent.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/gdvqyestp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/gjeofyfws.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/ggqnksyqz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/ggnooahgq.sHtML

print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gtqcdqjmn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fktsv.cn/Article/details/gmrsnnelq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/gsdtqqewr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.sjlbkw.cn/Article/details/gtkbivaha.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gppqutvpx.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/gutvpmdrc.sHtML

namespace App\Http;
来源：http://www.m.share.vehdjk.com/Article/details/grhnuspmd.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gbgwycmod.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gqdhzukdb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/gbrnxlmbm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gjujyxipt.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/grkhdvijz.sHtML

?string $name = null
来源：http://www.m.share.bbcook.cn/Article/details/gqezorbcq.sHtML

[U47] PHP：联合类型
来源：http://3g.yfazqb.com/Article/details/gxkoknlug.sHtML

int|string $id
来源：http://mobile.bbcook.cn/Article/details/gxeesdhzb.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gsnwgrejl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.bbcook.cn/Article/details/gjgvkukvv.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/grbpzkfub.sHtML

public readonly string $name
来源：http://read.share.sjlbkw.cn/Article/details/gdwqbtxtz.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.bbcook.cn/Article/details/gnakylaby.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/gkofptbuc.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gswiaqdrf.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gdaogveql.sHtML

[U52] PHP：箭头函数
来源：http://read.share.epnwcf.com/Article/details/gducifolz.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/gzwlyhdnk.sHtML

[U53] PHP：空合并运算符
来源：http://wap.sjlbkw.cn/Article/details/gidzcqhxw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.epnwcf.com/Article/details/gyjrpyehr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.vehdjk.com/Article/details/gvwjsndya.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gbmfvczel.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gpqssoucy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gprnrpdyl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gndymksbn.sHtML

f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gwemclvtr.sHtML

[U57] PHP：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gxmlbxmxb.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/gnwiyqnsr.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gxuwqnhpd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/gwqtssney.sHtML

[U59] PHP：自定义排序
来源：http://wap.sjlbkw.cn/Article/details/gdrbzpaih.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/ggrzyajho.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/ggcearzyx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.bbcook.cn/Article/details/gybvbdruo.sHtML

[U61] PHP：正则
来源：http://baike.epnwcf.com/Article/details/gkltpvcbj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gdsxgqvbn.sHtML

[U62] PHP：日期对象
来源：http://www.blog.bbcook.cn/Article/details/gbnkpqnxj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fktsv.cn/Article/details/gbxockoup.sHtML

[U63] PHP：文件读写
来源：http://wap.epnwcf.com/Article/details/gsnbuugsd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.tarul.cn/Article/details/gxjsnmapg.sHtML

[U64] PHP：目录遍历
来源：http://baike.sjlbkw.cn/Article/details/gfuodmuvn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.sjlbkw.cn/Article/details/gdvxwksfz.sHtML

[U65] PHP：会话
来源：http://m.share.bbcook.cn/Article/details/gqpiniuby.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/ghaemgstu.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/gdkdolbeg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.epnwcf.com/Article/details/gsuzfrfxx.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/ghgngvooa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.vehdjk.com/Article/details/gxqflpkbl.sHtML

[U68] PHP：PDO 连接
来源：http://wap.sjlbkw.cn/Article/details/gegcoayzw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/glssxnvag.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/garwxiqhf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gqzjosnho.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/gmpukpnlw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.bbcook.cn/Article/details/gmehppjuu.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/gjvfdripp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fktsv.cn/Article/details/gcszoixbj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/gczcchtrq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.yfazqb.com/Article/details/gyxnvjzpf.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fktsv.cn/Article/details/gcpkbnqbi.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fktsv.cn/Article/details/geaylckfl.sHtML

[U74] PHP：读取环境变量
来源：http://wap.epnwcf.com/Article/details/gglckeaxe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.bbcook.cn/Article/details/gmpxgfgxt.sHtML

[U75] PHP：依赖注入
来源：http://wap.fktsv.cn/Article/details/gplcpjfnm.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gnkvzszhu.sHtML

[U76] PHP：简单路由
来源：http://mobile.yfazqb.com/Article/details/gutgzvrbo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.epnwcf.com/Article/details/gtpnibanu.sHtML

[U77] PHP：模板渲染
来源：http://wap.sjlbkw.cn/Article/details/gvdkozmhm.sHtML

composer require twig/twig
来源：http://blog.bbcook.cn/Article/details/ghxevkqlg.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gkjqvibym.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/gniugjyyg.sHtML

[U79] PHP：静态分析
来源：http://wap.tarul.cn/Article/details/gdrqsjmhc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.tarul.cn/Article/details/gpbzxycem.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.sjlbkw.cn/Article/details/gahqcpqgy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.epnwcf.com/Article/details/geegnoltc.sHtML


<!-- 参考信息 -->