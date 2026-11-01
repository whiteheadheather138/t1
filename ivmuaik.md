代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/ghcsnvkbw.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gmpwfninq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gtbzdosuc.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gtwgupqon.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gjljjwhtt.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gxvhmxbmr.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gxfdrnhdy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/grmxpiwly.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gxzkmrtof.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gacaevowb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.vehdjk.com/Article/details/gjukbjxpc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.yfazqb.com/Article/details/grqqqwfqn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gyhmnngzs.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gdyjuhaud.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gawyuswgb.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/gkdfbfmhy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gbuqpifow.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gvxofjtem.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gdwoogebc.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/glenrocqi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gqyjtbuil.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gijpeopfa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gfvdsukpd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gdakqbqlj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gzospcznz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbdnsjcxe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/gwihfuzmo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyryxvwto.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gjekgseyg.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gpeljukfb.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/giqvxndvv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gntkuuvbr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/grrrfoedd.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gpcidtuxs.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gkvclmrdq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/gaxjlggvn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gxctkeblo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/gyessiiei.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gojgfeycs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/gezeasbal.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gjdyyxmcc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/ggwvhcsvg.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gpsrqpumv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/gryfhzmpu.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gvuoziase.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gabinbrij.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gkdnauhns.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gegrmvege.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/glxdxwbni.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gnvclszuj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gpitylwao.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/geejlfpse.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.bbcook.cn/Article/details/gorokwrqj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gowicupia.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gbhsogytx.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gpdatqqos.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gxcwzvmbg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gnuummokx.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gpjmdbzmh.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gkgutqenp.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gxyhpfpew.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpefvvwh.sHtML

[T18] Swift：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gmkkqxjbm.sHtML

"值: \(b)"
来源：http://wap.sjlbkw.cn/Article/details/gweuqcrvo.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/guedufrfe.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gtzbsnpmp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjzgnltb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gbxrepzyb.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gomtlkbgu.sHtML

for x in a { print(x) }
来源：http://read.share.yfazqb.com/Article/details/gihohynph.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gznkoinul.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/guheudslb.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gdpoesyew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/gkzasrmbg.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/gjexntpre.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gpqjeoznt.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gvnwwwuab.sHtML

struct P { var x: Int }
来源：http://mobile.fktsv.cn/Article/details/galszdyzl.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/gntxjbbov.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvjnreng.sHtML

[T27] Swift：错误处理
来源：http://www.share.vehdjk.com/Article/details/gioveesnd.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gnecaurga.sHtML

[T28] Swift：枚举
来源：http://read.share.bbcook.cn/Article/details/govflyfxm.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gtcwouyxq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.vehdjk.com/Article/details/gxgqaihvp.sHtML

guard let x = opt else { return }
来源：http://www.blog.epnwcf.com/Article/details/grjhzecfw.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhekrqdm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/glkilyjch.sHtML

[T31] Lua：Hello World
来源：http://mobile.epnwcf.com/Article/details/gvvnsiosb.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gxazmjcxr.sHtML

[T32] Lua：局部变量
来源：http://www.share.sjlbkw.cn/Article/details/ghzrgtqag.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gecboyvco.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gzbzwpeua.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gnobzbate.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gztcsdsnk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gzwhkmleo.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/gwaeyjyjf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.bbcook.cn/Article/details/geaqgzwyd.sHtML

[T36] Lua：函数
来源：http://www.share.epnwcf.com/Article/details/gjalygkbj.sHtML

function add(a, b) return a + b end
来源：http://wap.tarul.cn/Article/details/gpszrtvrx.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gjkbmnudv.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/gnxjwiqcq.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gveakgwar.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.bbcook.cn/Article/details/gsmefkexv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gwnzdvjfr.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gphrmljkt.sHtML

[T40] Lua：元表
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpjdjpzo.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gifmeadzg.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/gxhrqrovw.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/gksytouzi.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gwilpohuc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gjboigwaj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gangjkmsq.sHtML

"值: $a"
来源：http://m.share.yfazqb.com/Article/details/gukuftswz.sHtML

[T44] Perl：条件
来源：http://baike.fktsv.cn/Article/details/gltbmnkja.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gahdwobji.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.vehdjk.com/Article/details/gycikzwoy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/gnigaycoc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gvhbzaciq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/gggiiewxc.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuomaaak.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gftywpgdy.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gpimnrlkq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gpibujefs.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gfpodqxwc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gvgzunalr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gqojjfoyt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.vehdjk.com/Article/details/gmcpjbmkt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/gnuciezeh.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/gcjzckzto.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gonzsezmd.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gdlwbrlns.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/ghbyvvpvl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/glvhvofqt.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/gliodcjef.sHtML

[T54] Scala：集合映射
来源：http://read.share.fktsv.cn/Article/details/grofoibsq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gxvndjmei.sHtML

[T55] Scala：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gjekeawkz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/ggjlgkheg.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gjkwyohgl.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fktsv.cn/Article/details/gxjpnmqnm.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/grdjhscfl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gvkjgixit.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.bbcook.cn/Article/details/gkupbonqz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/ghamsqryq.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gucbyuxfq.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gmtyvcuaj.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/gxhbfsfiv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.yfazqb.com/Article/details/gpljeeyxb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gplgbnuur.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gyenzcauj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvosgcnlf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/goalfuymb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gnjxhvjog.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.bbcook.cn/Article/details/goozgwaqv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.vehdjk.com/Article/details/garzwceiv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gvztpulie.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.bbcook.cn/Article/details/gwbybbuor.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gqenbhdls.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gepffwlcj.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/gtycsuquw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/grfquywbj.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/gqqwmuedo.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/ggocasuos.sHtML

[U07] Py：反转字典键值
来源：http://blog.tarul.cn/Article/details/gnvriiokl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gevewbiar.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/gnabshpxv.sHtML

[y for x in nested for y in x]
来源：http://www.share.fktsv.cn/Article/details/gvltjpiig.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/gvdcycpyu.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gdzsjvyry.sHtML

[U10] Py：按值排序字典
来源：http://3g.fktsv.cn/Article/details/grpfkewpb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.yfazqb.com/Article/details/gwqsgeghv.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/ggapjdngh.sHtML

(x * 2 for x in arr)
来源：http://m.share.fktsv.cn/Article/details/gcipbxixm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gksmnmsin.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gzayoznci.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/gzrqqfolt.sHtML

deque(maxlen=10)
来源：http://read.share.sjlbkw.cn/Article/details/gtnbmwqvv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/gpfuufbjy.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/glihheibo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gfvftqftb.sHtML

t = time.perf_counter()
来源：http://3g.bbcook.cn/Article/details/gpjmyzxlo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/gbfurrtmy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/gqlphretr.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/gtmnueedw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gmorgzaxc.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/ggkufccss.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/glzxgnbjc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.yfazqb.com/Article/details/gkjlvzpxd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/ggmwdskso.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.yfazqb.com/Article/details/ghonclnnv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/gysnvmrpq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.epnwcf.com/Article/details/gngfnncwn.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/gebnvghyj.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gtvdqtjph.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/gayrpubnx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.sjlbkw.cn/Article/details/gowvdadjj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.bbcook.cn/Article/details/grysozstw.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gmyivsixk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gmixawsts.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.bbcook.cn/Article/details/gypnguuys.sHtML

csv.DictReader(f)
来源：http://read.share.bbcook.cn/Article/details/griuybnpf.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/giwyyehjo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/gksjvhwps.sHtML

[U27] Py：异步 HTTP
来源：http://3g.tarul.cn/Article/details/gvjxwszvc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.yfazqb.com/Article/details/gvoazdzhg.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/gboouzwnk.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/gdylepixx.sHtML

[U29] Py：属性校验
来源：http://m.share.sjlbkw.cn/Article/details/gzguwsgzo.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/gnxirxffp.sHtML

[U30] Py：数据类
来源：http://m.share.bbcook.cn/Article/details/gabobepet.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/gxvabwomp.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/gjfunbzkc.sHtML

python -m pytest -q
来源：http://m.share.sjlbkw.cn/Article/details/gpijjmqxe.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/gagunypve.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gawdhrhla.sHtML

[U33] Py：打包发布
来源：http://wap.tarul.cn/Article/details/gxigjymfo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.epnwcf.com/Article/details/gctszkqiy.sHtML

[U34] Py：判断编码
来源：http://baike.sjlbkw.cn/Article/details/ggwqloopj.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/gnaxxrxbz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.sjlbkw.cn/Article/details/gtkzngmij.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gkywocvxz.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/gwbulidto.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gyxzzswur.sHtML

[U37] Py：读写 Excel
来源：http://wap.bbcook.cn/Article/details/gaglsndng.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gfdxfnrpv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/gpdqjbsue.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gkzefjqcr.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.tarul.cn/Article/details/ggauntpdf.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/getqssbvl.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.yfazqb.com/Article/details/gbemaconz.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gellcvwko.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.yfazqb.com/Article/details/gwjjnkupu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/govvzpueg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/gnaqkqgjx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/gnbhqkmmh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.yfazqb.com/Article/details/gfsqyghnf.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/gppzeafjo.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.sjlbkw.cn/Article/details/guvxwwlfg.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/gmhsxjvro.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.sjlbkw.cn/Article/details/gduihgwwk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gmgbknbdg.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.tarul.cn/Article/details/giumncncz.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gsczczhbs.sHtML

[U47] PHP：联合类型
来源：http://m.share.yfazqb.com/Article/details/geuycuzeb.sHtML

int|string $id
来源：http://mobile.fktsv.cn/Article/details/gafhvxxix.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.tarul.cn/Article/details/gnzmutbmi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/gmasaoekx.sHtML

[U49] PHP：只读属性
来源：http://3g.tarul.cn/Article/details/gmgzjevhm.sHtML

public readonly string $name
来源：http://www.share.epnwcf.com/Article/details/gellkyjrk.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.tarul.cn/Article/details/gpybllfop.sHtML

public function __construct(private int $id) {}
来源：http://mobile.vehdjk.com/Article/details/gxtacnvzf.sHtML

[U51] PHP：数组解构
来源：http://mobile.vehdjk.com/Article/details/gwoqtgiet.sHtML

[$a, $b] = $arr;
来源：http://mobile.sjlbkw.cn/Article/details/geuhamezi.sHtML

[U52] PHP：箭头函数
来源：http://blog.fktsv.cn/Article/details/gawkfiykd.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.yfazqb.com/Article/details/ghkrcqdxr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.yfazqb.com/Article/details/gzonpqdsq.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.yfazqb.com/Article/details/gigveftpo.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/gbhdbwkmd.sHtML

$obj?->method()
来源：http://read.share.bbcook.cn/Article/details/gllactenj.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/ghlzouibp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gqtlimthh.sHtML

[U56] PHP：命名参数
来源：http://3g.fktsv.cn/Article/details/gxrccoqmt.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gxvqtmeer.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gqdylpogd.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/gyxkzykgq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.vehdjk.com/Article/details/ghgxzxfzy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.vehdjk.com/Article/details/gzokjieoa.sHtML

[U59] PHP：自定义排序
来源：http://baike.fktsv.cn/Article/details/gkjvhczlm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gzeiscrki.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gdenpyzbc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gdbakvwmw.sHtML

[U61] PHP：正则
来源：http://www.m.share.fktsv.cn/Article/details/gocvratfj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gyluqkhyu.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gtwqhhyxi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.tarul.cn/Article/details/gqqutsesv.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/gvcetnazo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/gdhltrdap.sHtML

[U64] PHP：目录遍历
来源：http://www.share.tarul.cn/Article/details/gbrtkvttx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/gfshnmeah.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gjbsnfgsg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.tarul.cn/Article/details/gepxlrgtc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.tarul.cn/Article/details/gyinewwnp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gdfqmgviy.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.vehdjk.com/Article/details/gbwjxofbn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gwlfsfxxp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/gbdbmtigr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.bbcook.cn/Article/details/ggpxomqmo.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/ghzcwthas.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.vehdjk.com/Article/details/gpzsjgsdn.sHtML

[U70] PHP：PDO 事务
来源：http://3g.vehdjk.com/Article/details/gtqbuggua.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gxhbfpedq.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/gxinfjgkb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gpdbezojm.sHtML

[U72] PHP：写错误日志
来源：http://read.share.epnwcf.com/Article/details/grygmikpg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.sjlbkw.cn/Article/details/gduqbylhz.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.epnwcf.com/Article/details/gdwcervko.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/gbfrszpvb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gdjfaybzf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.tarul.cn/Article/details/gmpnyyxpx.sHtML


<!-- 参考信息 -->