代发 wailian999

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gcqvftuhv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.bbcook.cn/Article/details/gfowvpmev.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gzazklhvq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/ggbxpuzpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gpveitreg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.sjlbkw.cn/Article/details/gjrusyaai.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gyjyidtal.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/girhhqvzv.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/ggtymdiou.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gwhqietfs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gqowtxmsq.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/gbccwqxdp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/gnidsspcd.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/goimffkad.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gteerkfwu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/grmbfoywm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gvddfxvyn.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/gdkdrbijk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/ghhyfhqlr.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/ghucqcfsi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gkodwgfwx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gurenmwin.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gqrqbijlv.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gtzirbyul.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/ggqiqxfmj.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/gsznmixco.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gwmldzvkx.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gcagdooem.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gfaoohiwc.sHtML

[S59] C++：静态断言
来源：http://mobile.tarul.cn/Article/details/glqlekavh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fktsv.cn/Article/details/gvnmjbdze.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gypzmpime.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/grjstcsau.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grofyyull.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gelwoaumt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghkhjeicl.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gpmfqnqit.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gnttholoa.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gkzirpzyb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gzqgjrkpx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.vehdjk.com/Article/details/glfugtxcl.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/gyocfuwvg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/gqfufkeik.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gdamhbaei.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gswlwwsxz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/gpcpkpklg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/ghybszeai.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gqrxiuuhp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gkqifjpqz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gitaeyyhk.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gwnlhqqsu.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/goqgyxiqf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gqrubaqwx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gxkrngaos.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/glymgvdgs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gyspvnfmh.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/glthqbrfb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gzvtcpxfr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/gjsjphxhi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fktsv.cn/Article/details/grctacjnj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.bbcook.cn/Article/details/gugbpyeqe.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fktsv.cn/Article/details/gkgodwqjw.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gndopzezq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gzbhgrsqy.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/gqlpodqlw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gutgktofl.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/gfecvwiui.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gdyrzbbuz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gcfvahkbv.sHtML

var a = 1;  let b = 2
来源：http://baike.bbcook.cn/Article/details/gioyagois.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gdpjauhll.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gjjfwlled.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.yfazqb.com/Article/details/gsdiznyhp.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/ghqnfckng.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gchxblbrz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gxhihhhkx.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gjcqfeozm.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gmibpacoz.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gmdiwxbaq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gfbtssrqo.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/gvpeesxbg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gmxkgawjx.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/giixiiuig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gpkpiscyc.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/ghaohjqiw.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/glchbqgut.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gbnjqiqxf.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/golizhdzk.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gtsfrdemk.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gpfsrzopm.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpjsdcry.sHtML

enum Color { case red, green }
来源：http://read.share.tarul.cn/Article/details/gtytetkot.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/glmrzakuq.sHtML

guard let x = opt else { return }
来源：http://wap.vehdjk.com/Article/details/gcnhlgzvu.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/ggzsrgqeo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/gjxrtlmzg.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gicoibpyl.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gohuiiocq.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gtrtcgukq.sHtML

local a = 1
来源：http://www.share.epnwcf.com/Article/details/gxblfkyms.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gadlvieft.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gpgybvsgz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gledmhntk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.epnwcf.com/Article/details/gaxtqnror.sHtML

[T35] Lua：字典表
来源：http://wap.sjlbkw.cn/Article/details/gamruxjeg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fktsv.cn/Article/details/gpmgdgreb.sHtML

[T36] Lua：函数
来源：http://m.share.epnwcf.com/Article/details/glabjglqk.sHtML

function add(a, b) return a + b end
来源：http://mobile.sjlbkw.cn/Article/details/gxrwcipmy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gwagmwfls.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gqejjifob.sHtML

[T38] Lua：条件
来源：http://wap.epnwcf.com/Article/details/gvutwsxac.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/guhnaqqul.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gbqhadzap.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/guspkrlyj.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/gxjfwpajf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gtmiapnwi.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gbabhmbyd.sHtML

print "Hello\n";
来源：http://www.share.yfazqb.com/Article/details/gyllxbjqc.sHtML

[T42] Perl：变量类型
来源：http://baike.epnwcf.com/Article/details/gpxbduaac.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/gfvwvxonr.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gymouxoai.sHtML

"值: $a"
来源：http://blog.epnwcf.com/Article/details/ghoivclzi.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/gezekdvic.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fktsv.cn/Article/details/gdpqsewba.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/ghbtaoxxx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.vehdjk.com/Article/details/glqohbdsw.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gtwtjtivm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/gawqgncvb.sHtML

[T47] Perl：正则捕获
来源：http://blog.fktsv.cn/Article/details/gonwyxahe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gpeydpdsx.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/glmjyrern.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gdhnmndrb.sHtML

[T49] Perl：函数
来源：http://blog.sjlbkw.cn/Article/details/glgdlltid.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gpmwsdlql.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gdscshskg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.epnwcf.com/Article/details/gwlivleop.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.vehdjk.com/Article/details/gisqgttsm.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/gsrwqhbgs.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gzqrgvfqp.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/ghitmmvmx.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gsbfiwnqd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/ghwsaohrg.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/gwqmbomeg.sHtML

[T54] Scala：集合映射
来源：http://3g.bbcook.cn/Article/details/gnxkkdrwu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhtothqn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gqszgbrdi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gnvxyqrni.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gsfbqjzmx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gdudrcmte.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gfgzxrbmn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.epnwcf.com/Article/details/guvadchfg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.epnwcf.com/Article/details/gtprouwbi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/gezhklyrx.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gvzbiuvxm.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gpzupvymt.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gugyltdsi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/gcwrjukkv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjznqjubz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/ghxaxvdfa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghjfvwszb.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gdtypcrgt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/ghrtlbhmm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.vehdjk.com/Article/details/goxpejmab.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gqyxnxpys.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.yfazqb.com/Article/details/gsonoswpf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gcmoyiibd.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/grtipusoy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.bbcook.cn/Article/details/gdphepuqx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/ggylptbjf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gapirdqxw.sHtML

[U06] Py：合并两个字典
来源：http://blog.vehdjk.com/Article/details/gefijatwg.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gmermoztt.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/grqktylre.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/ggqgxymwn.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gnivsrhry.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gksiunpkn.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.sjlbkw.cn/Article/details/gfddyfkwm.sHtML

max(d, key=d.get)
来源：http://blog.epnwcf.com/Article/details/gptcmphup.sHtML

[U10] Py：按值排序字典
来源：http://3g.vehdjk.com/Article/details/gvqitjkdt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gywcxmpkq.sHtML

[U11] Py：生成器表达式
来源：http://wap.tarul.cn/Article/details/gswzblksz.sHtML

(x * 2 for x in arr)
来源：http://blog.vehdjk.com/Article/details/gvundblth.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fktsv.cn/Article/details/gnbeplwsk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/grghrkzif.sHtML

[U13] Py：固定长度队列
来源：http://read.share.yfazqb.com/Article/details/gswgaoxuf.sHtML

deque(maxlen=10)
来源：http://m.share.sjlbkw.cn/Article/details/gvhgyqkkj.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gujujicit.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gqahrxqbb.sHtML

[U15] Py：高精度计时
来源：http://baike.fktsv.cn/Article/details/goetdbepa.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/gojnrxmii.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.bbcook.cn/Article/details/grfaoxtej.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gcsgjshgy.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/gnlirbjyr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.epnwcf.com/Article/details/gudglwisn.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.vehdjk.com/Article/details/gthwaogis.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.epnwcf.com/Article/details/gfvxwfdlp.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gzzhhizme.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtwfnmym.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/gpmveocnw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/guebsvxax.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fktsv.cn/Article/details/gjqbzjrzt.sHtML

@contextlib.contextmanager
来源：http://read.share.yfazqb.com/Article/details/gaykufqfk.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/gflpvzkxb.sHtML

list(zip(*m))
来源：http://blog.bbcook.cn/Article/details/gpqpahrjo.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfperjusw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/gvtdypqno.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gajvsrgkt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/guknrgaxo.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.bbcook.cn/Article/details/gvtrblcft.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gzeuygkjj.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/ghvyfkgup.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/ggjcsvnnt.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.yfazqb.com/Article/details/gwychfddn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/gfldgbrfz.sHtML

[U28] Py：类型别名
来源：http://read.share.sjlbkw.cn/Article/details/gvephwdpk.sHtML

UserId = int
来源：http://www.m.share.vehdjk.com/Article/details/gigqaxocl.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gphgfsand.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gydusjymc.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/glnkbhfrc.sHtML

@dataclass(slots=True)
来源：http://www.blog.vehdjk.com/Article/details/gwyzparrk.sHtML

[U31] Py：单测
来源：http://mobile.yfazqb.com/Article/details/gmltgnitx.sHtML

python -m pytest -q
来源：http://m.share.fktsv.cn/Article/details/gidmrjbck.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/gjrvkzxtc.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gamqqokzq.sHtML

[U33] Py：打包发布
来源：http://mobile.yfazqb.com/Article/details/gbcamoaoo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/gisjvgbns.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gsbsccynu.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/gvjaairmc.sHtML

[U35] Py：发送邮件
来源：http://read.share.sjlbkw.cn/Article/details/gypeptkka.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fktsv.cn/Article/details/gkagoagdo.sHtML

[U36] Py：定时任务
来源：http://www.blog.epnwcf.com/Article/details/ginbtwysu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/gaqhpdckf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.vehdjk.com/Article/details/gpfaglrja.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/geipgncyf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gcjqxdcif.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.vehdjk.com/Article/details/gsfhwkgyj.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/gzoscancz.sHtML

sys.stdout.isatty()
来源：http://baike.tarul.cn/Article/details/gvrwijejx.sHtML

[U40] Py：打印到标准错误
来源：http://baike.tarul.cn/Article/details/gugzwyylt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gedpaeygb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gvrlviwnx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/gwmxhzsyw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/gdbjiwswi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/grxtivyop.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.tarul.cn/Article/details/gkuqiagqa.sHtML

namespace App\Http;
来源：http://www.m.share.yfazqb.com/Article/details/gtcbgyegx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/gyxecgqau.sHtML

declare(strict_types=1);
来源：http://www.share.yfazqb.com/Article/details/gmibmastf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.epnwcf.com/Article/details/gxmifcnec.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gsatbkrur.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gmgelnzoz.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/grcwyxyah.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/gepmndqyy.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gohmncahi.sHtML

[U48] PHP：纯枚举
来源：http://mobile.sjlbkw.cn/Article/details/gfnfigewl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.vehdjk.com/Article/details/gjzncihbp.sHtML

[U49] PHP：只读属性
来源：http://3g.tarul.cn/Article/details/grlbinnho.sHtML

public readonly string $name
来源：http://www.blog.vehdjk.com/Article/details/gfmbqkqzg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gulbhgflg.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/gqxzhwlze.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gfergmben.sHtML

[$a, $b] = $arr;
来源：http://www.blog.tarul.cn/Article/details/gaaresnvo.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gnldyecud.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/gvutmtrlw.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gprdbadvp.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fktsv.cn/Article/details/gdpatacqr.sHtML

[U54] PHP：空安全调用
来源：http://mobile.epnwcf.com/Article/details/gykmjnxmq.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/ghijahfbh.sHtML

[U55] PHP：match 表达式
来源：http://baike.bbcook.cn/Article/details/guvhpdgmt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gnizdvdsc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gmihkqvif.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gnxnagtmm.sHtML

[U57] PHP：字符串插值
来源：http://3g.yfazqb.com/Article/details/gfhxekops.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/gkqvmjvvf.sHtML

[U58] PHP：数组三件套
来源：http://m.share.yfazqb.com/Article/details/gokccsxof.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.vehdjk.com/Article/details/gncwzpvfu.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fktsv.cn/Article/details/gsxtsvlla.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gccnmcfce.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/gyqiigviz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gwdmlzdpt.sHtML

[U61] PHP：正则
来源：http://3g.tarul.cn/Article/details/gfftgeunp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gqjgpftnr.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gvddtkkqd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fktsv.cn/Article/details/gjdkfatxw.sHtML

[U63] PHP：文件读写
来源：http://3g.fktsv.cn/Article/details/gucmhxnqs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/gcmvxxdij.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/garpzzltj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.vehdjk.com/Article/details/gesbyqkop.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gvqzcmjjk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gsvcjshtb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/glnxfrmvn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fktsv.cn/Article/details/gbjjhskif.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gstymlntc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/gjqrnkquo.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.vehdjk.com/Article/details/gltslmxxa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fktsv.cn/Article/details/gdvmnuego.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.epnwcf.com/Article/details/godqinzra.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/gjgxgyjao.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.yfazqb.com/Article/details/gzgxuagax.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.tarul.cn/Article/details/gapyvhzqe.sHtML


<!-- 参考信息 -->