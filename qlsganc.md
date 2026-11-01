代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkotukgm.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gwjjpslvq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gqqlxaaoh.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gjcgxntey.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gijqehjqd.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gewggxevg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/gmkuthatw.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gppbvmmfj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gqdlmbylf.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gquoxkdpm.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gnqqgiehd.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gqypaszgh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/gbrzoyuec.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gejbgskul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gvcfmvzpb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/gnbqtzdob.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gsfkasutx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggagvniew.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/giqalqlpe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/galhlscyw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gwrxkhnfq.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gfoglxqtm.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gxvqllpsu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gwmmhbruk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/gxlclloyi.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/ghifxisoh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gytsjpqly.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/gxukzvdxh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.tarul.cn/Article/details/guhlmuxzy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gnygvxkuo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gzmiknlsn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gmzpqdfvr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gtuaddiud.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gcrwtnlvo.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/glijcwqhg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/granosmdb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/gclacchve.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/giiivsivq.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gdagdfirq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.sjlbkw.cn/Article/details/gbnqgyuaw.sHtML

[T11] Kotlin：协程
来源：http://www.share.sjlbkw.cn/Article/details/glbpoijog.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gyvndqweo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.tarul.cn/Article/details/gikgxtcne.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gpyusnkax.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gzjenhesl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gbisobxvy.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/gedyjbnzk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gdtuwpvfn.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gkjfixhey.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gfcchesyb.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gsnrwdxqm.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gvpapzmmi.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gdevhogvd.sHtML

var a = 1;  let b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gwjxrggxp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gcpnyhizn.sHtML

"值: \(b)"
来源：http://baike.bbcook.cn/Article/details/gaytyjwwm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/geifzikca.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gfiksssth.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/govjhujoz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gstehbgbo.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gfojedmwt.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gyrfwiwji.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/gwqnoomcj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/ggwvlqjiq.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gffxvdtch.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/gtlarrhpi.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gjdsrlfjx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/grdkvcoko.sHtML

[T25] Swift：结构体
来源：http://m.share.fktsv.cn/Article/details/gubkfbyzm.sHtML

struct P { var x: Int }
来源：http://www.m.share.yfazqb.com/Article/details/gwkyjatfn.sHtML

[T26] Swift：类与重写
来源：http://www.share.fktsv.cn/Article/details/gohrnaggd.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gsbayioiw.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/guupxngkx.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gzhxlynfw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gcfvzitbc.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gekbalcns.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/grrkfvayj.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gsozcrzeq.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gvdfjvucu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/gavoaijil.sHtML

[T31] Lua：Hello World
来源：http://m.share.vehdjk.com/Article/details/gortdhzlp.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gmlccrxhs.sHtML

[T32] Lua：局部变量
来源：http://www.blog.vehdjk.com/Article/details/gzoytkxqc.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/gdphmblwd.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/gfiryzmtc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gjwvmtsub.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gwwxrkvzd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.sjlbkw.cn/Article/details/grihcghzs.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/gmgfjfvuo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/ghbksaqmo.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/gipjysiyl.sHtML

function add(a, b) return a + b end
来源：http://m.share.bbcook.cn/Article/details/gyrfqlngh.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gblrkjciw.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gfljlkpje.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/gysbbwurc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/gunsnpuny.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/giuhtrvop.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gauuuscyu.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gbsbwromj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.tarul.cn/Article/details/gbutccytr.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ggyffopyd.sHtML

print "Hello\n";
来源：http://baike.fktsv.cn/Article/details/gskkriwlg.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gwagqbahg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gowoxwaaw.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/gkvfrundo.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/ghuscvhdu.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gtmxeaiol.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/gmmaakcxy.sHtML

[T45] Perl：数组遍历
来源：http://read.share.vehdjk.com/Article/details/gdvxbugvf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/giaiotrwx.sHtML

[T46] Perl：哈希操作
来源：http://3g.vehdjk.com/Article/details/gjdiusulc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/gstqclczm.sHtML

[T47] Perl：正则捕获
来源：http://3g.yfazqb.com/Article/details/gkxufnwxs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gaptvoohh.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gqcwhybah.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/gkhxronrr.sHtML

[T49] Perl：函数
来源：http://mobile.fktsv.cn/Article/details/gqzqsoeie.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gvmkkljqp.sHtML

[T50] Perl：逐行读文件
来源：http://3g.tarul.cn/Article/details/ggbrhcoso.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gdnxcynop.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.bbcook.cn/Article/details/glukdxdki.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gplfhiyuj.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gnitxyacj.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gimnigqci.sHtML

val a = 1;  var b = 2
来源：http://mobile.fktsv.cn/Article/details/grybjhanv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/giftcxrsc.sHtML

s"值: $b"
来源：http://blog.vehdjk.com/Article/details/guikytwxs.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gohnqampw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gefdioebj.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gzqoklpat.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gmxmrcyzg.sHtML

[T56] Scala：样例类
来源：http://read.share.sjlbkw.cn/Article/details/gekalurjo.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gjymapcbp.sHtML

[T57] Scala：模式匹配
来源：http://read.share.vehdjk.com/Article/details/ghjyguwzf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gpipeagov.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gfbuyynbj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gulfgfgox.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/gxvykjrjy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gpvnoelbi.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/gpfmqujzj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/grvmcrkyc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggvniuevh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gjedkbblv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjmfxmhix.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/grftwhuda.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.bbcook.cn/Article/details/godmtmpnl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gbuawdwpv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.vehdjk.com/Article/details/guzmasmsb.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fktsv.cn/Article/details/giotjtuad.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.vehdjk.com/Article/details/gwxbvomhj.sHtML

[U04] Py：变量调试打印
来源：http://blog.yfazqb.com/Article/details/grhostcch.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.bbcook.cn/Article/details/gkngepppe.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/gwdmbmmtv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/gnmcqpywk.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gbutpfjia.sHtML

{**a, **b}
来源：http://www.share.bbcook.cn/Article/details/grtbsekrr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.vehdjk.com/Article/details/givnoxsnh.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gksjtgage.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/gqhekgdvt.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/gkxrylzja.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/gglbtuibs.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gmjrvuocu.sHtML

[U10] Py：按值排序字典
来源：http://baike.fktsv.cn/Article/details/gpfxhzvwb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.epnwcf.com/Article/details/gejzmkyiv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/givkmlpel.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gokquqgks.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fktsv.cn/Article/details/gvyexudah.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fktsv.cn/Article/details/gnthscsrg.sHtML

[U13] Py：固定长度队列
来源：http://blog.tarul.cn/Article/details/gynfeirzv.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/gqnuqwojc.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/gosnnyiwj.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gobfpmyhs.sHtML

[U15] Py：高精度计时
来源：http://m.share.sjlbkw.cn/Article/details/gxnpcudij.sHtML

t = time.perf_counter()
来源：http://mobile.epnwcf.com/Article/details/gcjgqtaqk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.yfazqb.com/Article/details/grxltpczb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.yfazqb.com/Article/details/givmgixck.sHtML

[U17] Py：初始化日志
来源：http://wap.epnwcf.com/Article/details/gtsbdupsj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.bbcook.cn/Article/details/gyabpabjz.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/gagmltapo.sHtML

pat = re.compile(r"\d+")
来源：http://baike.bbcook.cn/Article/details/gwprtrmtl.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gjykddqqk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/gvzoeewfr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gzzapscze.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.tarul.cn/Article/details/ghdmnbtrt.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/gutmiaryn.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gdtobwqug.sHtML

[U22] Py：矩阵转置
来源：http://3g.sjlbkw.cn/Article/details/gtxiofjrz.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/gjpsbqpqb.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gywgogesk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.vehdjk.com/Article/details/gwswqobjb.sHtML

[U24] Py：路径操作
来源：http://www.blog.fktsv.cn/Article/details/gmbrbpkdi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gxiquaxdu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.bbcook.cn/Article/details/gtoynflnu.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gsphbqxqp.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/gcwzrxdkp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fktsv.cn/Article/details/glxwfumas.sHtML

[U27] Py：异步 HTTP
来源：http://blog.yfazqb.com/Article/details/geqwikxkv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.vehdjk.com/Article/details/gkaqcsmwa.sHtML

[U28] Py：类型别名
来源：http://read.share.sjlbkw.cn/Article/details/gwrteobzm.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gqaiuxzwc.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gyborderk.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/glqtkfhtl.sHtML

[U30] Py：数据类
来源：http://baike.vehdjk.com/Article/details/gbphqowrb.sHtML

@dataclass(slots=True)
来源：http://read.share.fktsv.cn/Article/details/gevyllyhk.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gwclsqbmn.sHtML

python -m pytest -q
来源：http://wap.yfazqb.com/Article/details/gznylewgc.sHtML

[U32] Py：代码格式化
来源：http://mobile.fktsv.cn/Article/details/gucwmrtij.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.bbcook.cn/Article/details/gxwxksgjz.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/gdliaqbmo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gfaiechru.sHtML

[U34] Py：判断编码
来源：http://3g.fktsv.cn/Article/details/gvkcsaabj.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/gvnjonomk.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gdjjqrcqd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/gnnnuftrt.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/gpuwncndx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gavjjctsb.sHtML

[U37] Py：读写 Excel
来源：http://www.share.tarul.cn/Article/details/gfnpxkvuj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/gojhadhqm.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.sjlbkw.cn/Article/details/gtffwgttk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.yfazqb.com/Article/details/goitallgy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/giuexmswo.sHtML

sys.stdout.isatty()
来源：http://m.share.fktsv.cn/Article/details/gpoyzyfln.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gbobsceuq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gtmwwlayx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/gqoxbinee.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/geicahljs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.yfazqb.com/Article/details/guhagqtmn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gkdayipyj.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.yfazqb.com/Article/details/grngwbrml.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gqvptecsu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.vehdjk.com/Article/details/gjofbiaof.sHtML

declare(strict_types=1);
来源：http://m.share.sjlbkw.cn/Article/details/gslvhipta.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.bbcook.cn/Article/details/gjlghdpea.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gtmzczgte.sHtML

[U46] PHP：可空类型
来源：http://mobile.epnwcf.com/Article/details/gwrnrnaqo.sHtML

?string $name = null
来源：http://mobile.sjlbkw.cn/Article/details/ghignthra.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gnwqhuxbl.sHtML

int|string $id
来源：http://www.share.tarul.cn/Article/details/gwssxtpem.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/gtuoicjkz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/gqdtduwrp.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gryebvvuk.sHtML

public readonly string $name
来源：http://3g.vehdjk.com/Article/details/gillgqfwc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gjxhbhrhc.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfiytlwqh.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gjtgmyirl.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gfqmhzscn.sHtML

[U52] PHP：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gnuwvpoux.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gbpbxorqm.sHtML

[U53] PHP：空合并运算符
来源：http://3g.sjlbkw.cn/Article/details/gpmbnxkzk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.tarul.cn/Article/details/getpzmvsh.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gsrkckhhx.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gulnzsqcj.sHtML

[U55] PHP：match 表达式
来源：http://m.share.yfazqb.com/Article/details/gohkcoxqz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.tarul.cn/Article/details/glvpgvpff.sHtML

[U56] PHP：命名参数
来源：http://read.share.epnwcf.com/Article/details/garcezjbs.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gpelqgqpq.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gjqvkclkk.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/gbitunudx.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/gomyntokl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/grrbwayor.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.tarul.cn/Article/details/gpglytufg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gjaldbnax.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gfoxezfzz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gmxthxnfz.sHtML

[U61] PHP：正则
来源：http://m.share.vehdjk.com/Article/details/gcbzjpjbz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gzogympsv.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/gefxcwcnc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.epnwcf.com/Article/details/gmysnwodn.sHtML

[U63] PHP：文件读写
来源：http://m.share.epnwcf.com/Article/details/gbzwpvweg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.tarul.cn/Article/details/guqnuioov.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gbzkccycz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/gtwqcgaqy.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gqmkoxvfx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fktsv.cn/Article/details/gypsyalbj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gkcityglc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.vehdjk.com/Article/details/gsofzvfdi.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gkbqwofkh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/grpsscvel.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fktsv.cn/Article/details/gxznnanib.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.sjlbkw.cn/Article/details/gfjwbbypn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.bbcook.cn/Article/details/griwqhvoo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.tarul.cn/Article/details/gbndykaua.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/gdznizzlb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/gpgitepxx.sHtML

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gmlzgymrc.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gqjgucejx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.vehdjk.com/Article/details/gisdmbbuk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/gcviragli.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/gjacwiyae.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.epnwcf.com/Article/details/ggmfziioy.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/grlopscbi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gqbauyhyp.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gnwccibiy.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gjlbnopws.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gjnkzxhlr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.vehdjk.com/Article/details/goafgkbfg.sHtML

[U77] PHP：模板渲染
来源：http://m.share.vehdjk.com/Article/details/gmzoavjbb.sHtML

composer require twig/twig
来源：http://wap.tarul.cn/Article/details/gfajihlfp.sHtML

[U78] PHP：单元测试
来源：http://baike.vehdjk.com/Article/details/gvoujxqrc.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.epnwcf.com/Article/details/gkyoqzirf.sHtML


<!-- 参考信息 -->