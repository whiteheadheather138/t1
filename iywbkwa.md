代发 wailian999

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gdlfbohed.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gfmxwkcso.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gummogisp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/glwvrgpsa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gmihrxtix.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gokuoqkun.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gpufgfyyr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gwjapshev.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gztklrgpe.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gobssflrj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gkkctrhqb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/gkdniuoha.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/glbjscpgq.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/ggmcbawiv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gbeiilrqj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/gfngngwlo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/gqqhnddfw.sHtML

[S53] C++：移动语义
来源：http://www.blog.yfazqb.com/Article/details/gvkoyeleq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/gquppmhfa.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gixzomgzo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/ghbbxsety.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gqqwdtcor.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gjgerceda.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/giacqygai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gxmpksctu.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/guvgnohoe.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gzmdmopyg.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/gjbmehgad.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/gzvtnplol.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/gynowvusv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbiwfbhc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gojsgbcbs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gidbwaedd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfnoyupkt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/geymukdnr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gphrbdxok.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gsqarohfd.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gbpukvfhu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gixrtjmdm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/ggfmgqqgr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gfuntpjar.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gitkvcdiq.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/gzkdcxwej.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/giaixobpt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gbiidksbh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/gruxeckyj.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gxmzjjdgw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/guexbbpte.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gxlmalsre.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gupjhqdza.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gxaqeelxi.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gpftbqgfi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/grmasxzzb.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/geyeduapg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gjhjgzske.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.tarul.cn/Article/details/gubtctchm.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/grwvdczug.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/gkypgfuno.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/gnffbuhwq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/gdyzejqxi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/giguyraji.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/glohjvxcz.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fktsv.cn/Article/details/gjxtbvgtw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gifjqvfft.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/gaavtaern.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gsqbcorzc.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gxzyezleu.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gnlqekoiu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gphxjzove.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gggwpglwm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/glffdyyzb.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/ggczgveer.sHtML

[T19] Swift：可选绑定
来源：http://wap.epnwcf.com/Article/details/gimwmlbil.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/gqrxrboio.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/giwpgjdsq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.epnwcf.com/Article/details/gymooyhoh.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/gsuzecpyf.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gxfmldhhn.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/gqcrkdlcp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/ggqfcsgdk.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gqiikndqv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gyjipggev.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gnpemnvdt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gzmuihjqe.sHtML

[T25] Swift：结构体
来源：http://read.share.sjlbkw.cn/Article/details/ggmpstnar.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/gmjyxzuiy.sHtML

[T26] Swift：类与重写
来源：http://m.share.vehdjk.com/Article/details/gjhxchycz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/glwwxpukb.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gtospxsml.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gowbvejja.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gxozhcway.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gshwuedbf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gqymaxoac.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gqmihccye.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gkfszlsfb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gjvvncnbr.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gjttxaojp.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gwwfwdlyz.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gavixbawu.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/giuwrbsmj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fktsv.cn/Article/details/gwxvjqiwa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.yfazqb.com/Article/details/gpsbhfsxx.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gheedfbwp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.tarul.cn/Article/details/gpbfdthtn.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gfqvianlr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gfrmcyfqv.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/guvhbgsqv.sHtML

function add(a, b) return a + b end
来源：http://www.share.fktsv.cn/Article/details/gfsjaqchs.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gjzrplxfr.sHtML

"a" .. "b"
来源：http://www.m.share.fktsv.cn/Article/details/ghddopqdu.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/gjhakaahb.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gtcxqqsdt.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/gofcrvmwi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/gtfghnmxl.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gefmrcohx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.yfazqb.com/Article/details/gxtlyldnp.sHtML

[T41] Perl：Hello World
来源：http://www.share.tarul.cn/Article/details/giglbhadm.sHtML

print "Hello\n";
来源：http://m.share.sjlbkw.cn/Article/details/ganmvdtek.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gofdscspj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/gfeaobuhu.sHtML

[T43] Perl：字符串插值
来源：http://www.share.yfazqb.com/Article/details/givuzpayx.sHtML

"值: $a"
来源：http://blog.fktsv.cn/Article/details/gaosgtqfy.sHtML

[T44] Perl：条件
来源：http://www.share.epnwcf.com/Article/details/gxolsatrz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gehcditnk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.tarul.cn/Article/details/gowujytzg.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gtpftiuar.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gwbckwyqq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gjaxflhfm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gssldgqux.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gkgkrrmmq.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/glqufkhmc.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/ghjaqavqb.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/gnxtnogao.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gmuvbdeyf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gpnktxkdx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/guovoatek.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gyqlkjflh.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/gicmcvizb.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gpvxetjjh.sHtML

[T52] Scala：变量
来源：http://wap.tarul.cn/Article/details/gjivnfekg.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/gwlvrisws.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gtpikhofq.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/ghfzumkhe.sHtML

[T54] Scala：集合映射
来源：http://mobile.bbcook.cn/Article/details/gbrwutphv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.epnwcf.com/Article/details/gjukyrqel.sHtML

[T55] Scala：集合过滤
来源：http://blog.vehdjk.com/Article/details/gwzunmkje.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gspnffvqs.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gmflqyawr.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fktsv.cn/Article/details/grkcdknfu.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gfvpwcvae.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gibguuagb.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/guvgcpvwy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gzlmndtox.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gyjaxffcq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.tarul.cn/Article/details/guxhfyxbk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/goujotsgv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.epnwcf.com/Article/details/gkooktbaa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmlweqpmm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gnekvuduz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjnurnxna.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gjqrfbedw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/gjyhplaer.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbwhyzif.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gneqzzxnd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gjjoijbiy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gvxylsekq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.vehdjk.com/Article/details/gcopjbzaw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gskcmccoa.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/gpxlwztid.sHtML

list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gckfrdwqg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/giormscwu.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/gsxemqvfv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gchutaydf.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/grtgfnzye.sHtML

[U08] Py：展平二维列表
来源：http://blog.vehdjk.com/Article/details/gyikkukln.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/gxagtrslj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/gonhtnati.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/ggcjxgvjn.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/ghrrfmqkq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gfluqcmvv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fktsv.cn/Article/details/gittkuokl.sHtML

(x * 2 for x in arr)
来源：http://read.share.bbcook.cn/Article/details/gkihointn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.bbcook.cn/Article/details/gwjiaspxr.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gezgeupyk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/gqtjxmxow.sHtML

deque(maxlen=10)
来源：http://www.blog.yfazqb.com/Article/details/gggncqecm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.vehdjk.com/Article/details/gmubycvws.sHtML

defaultdict(list)
来源：http://baike.epnwcf.com/Article/details/gexruvsgi.sHtML

[U15] Py：高精度计时
来源：http://blog.bbcook.cn/Article/details/gkxvjyghz.sHtML

t = time.perf_counter()
来源：http://www.blog.yfazqb.com/Article/details/gugbalmjn.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/grvxsuuoq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gytonjkcj.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/givwritab.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.yfazqb.com/Article/details/gtoionlyo.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gxfbtxrvr.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/ghuzkogoa.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.bbcook.cn/Article/details/gkjnsygrg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gfpffgzie.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/gdvathdie.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/grksddcor.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.vehdjk.com/Article/details/gjvemoctt.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmidvysu.sHtML

[U22] Py：矩阵转置
来源：http://m.share.tarul.cn/Article/details/gwtffawgq.sHtML

list(zip(*m))
来源：http://www.share.fktsv.cn/Article/details/gasaqoarv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/ghdukdnwy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gzssllmiw.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gwzucckbr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gggofjeon.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/gwphgqsqe.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gutclzkfz.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/goqcqrdie.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.epnwcf.com/Article/details/gzklgujik.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.sjlbkw.cn/Article/details/gxkbnsvwr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gvyckxgxg.sHtML

[U28] Py：类型别名
来源：http://blog.tarul.cn/Article/details/gitxlzhit.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/gfbchgfol.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gazdckdbh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gymxrftpe.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/gtmqukijr.sHtML

@dataclass(slots=True)
来源：http://mobile.tarul.cn/Article/details/gwsfiqzhh.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/glidktpyw.sHtML

python -m pytest -q
来源：http://www.blog.bbcook.cn/Article/details/gnqjfghrh.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/gcfzksica.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.epnwcf.com/Article/details/goaibibrn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.epnwcf.com/Article/details/gfxatztdn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.tarul.cn/Article/details/geppakjul.sHtML

[U34] Py：判断编码
来源：http://read.share.vehdjk.com/Article/details/gekoeusvk.sHtML

chardet.detect(raw)
来源：http://wap.yfazqb.com/Article/details/gcqyioryr.sHtML

[U35] Py：发送邮件
来源：http://wap.tarul.cn/Article/details/gvpiqslez.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.tarul.cn/Article/details/ggiurbcsc.sHtML

[U36] Py：定时任务
来源：http://mobile.yfazqb.com/Article/details/gvxrrtgih.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.yfazqb.com/Article/details/gzhereuux.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/gbjfumpfk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.vehdjk.com/Article/details/gkszmtitk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gzcbclqzo.sHtML

Path(__file__).resolve().parent
来源：http://www.share.tarul.cn/Article/details/gieicwyiu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.tarul.cn/Article/details/gsefxbsnz.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/gviokmdsu.sHtML

[U40] Py：打印到标准错误
来源：http://wap.sjlbkw.cn/Article/details/gyklyfkxn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gjujljzpe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/gqdoqvpgb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/gorivlqqd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.yfazqb.com/Article/details/gdjjobdqx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.tarul.cn/Article/details/gxegwbccw.sHtML

[U43] PHP：声明命名空间
来源：http://3g.sjlbkw.cn/Article/details/glkwptylb.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/grcfitews.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.epnwcf.com/Article/details/gitlzotvj.sHtML

declare(strict_types=1);
来源：http://read.share.sjlbkw.cn/Article/details/guufuuwnt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fktsv.cn/Article/details/gnbhiavuq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/glqsofalb.sHtML

[U46] PHP：可空类型
来源：http://www.share.yfazqb.com/Article/details/ghywluhhf.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/gbcefhbxk.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/gofeplomg.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/glmlrwoit.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/girywzhgl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fktsv.cn/Article/details/gqzvjzvmf.sHtML

[U49] PHP：只读属性
来源：http://wap.fktsv.cn/Article/details/gszcunfko.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gbkpajlko.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/gonaxuvdp.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.vehdjk.com/Article/details/gbsehkxxp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/giunzfqxt.sHtML

[$a, $b] = $arr;
来源：http://m.share.tarul.cn/Article/details/gkdqcfkfn.sHtML

[U52] PHP：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gruregjsg.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/geplluxqg.sHtML

[U53] PHP：空合并运算符
来源：http://3g.sjlbkw.cn/Article/details/gjtvyqbfo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fktsv.cn/Article/details/gnorzhwxc.sHtML

[U54] PHP：空安全调用
来源：http://m.share.yfazqb.com/Article/details/gozfjcncb.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gihqndfin.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.epnwcf.com/Article/details/gcpykcsio.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gvdfuiaoo.sHtML

[U56] PHP：命名参数
来源：http://blog.yfazqb.com/Article/details/gjzqquxnv.sHtML

f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/goyxiwzpg.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/grjznjvlo.sHtML

"值: {$a}"
来源：http://m.share.yfazqb.com/Article/details/gsyagjndf.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/ghwuchabj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzslhopda.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.epnwcf.com/Article/details/gfntuxfwj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gdgiftesg.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.sjlbkw.cn/Article/details/gzpusfdlr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.yfazqb.com/Article/details/gimvfqonc.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gyqagipjt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gwadocxnf.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gbdlthghq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gwkylfqve.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/gmfgimocf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gczqclbay.sHtML

[U64] PHP：目录遍历
来源：http://www.share.yfazqb.com/Article/details/gsudysbzi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gowmaxpry.sHtML

[U65] PHP：会话
来源：http://www.share.sjlbkw.cn/Article/details/gvtqkrqpx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fktsv.cn/Article/details/guonmqffz.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/gmmxxlkxh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/goxdrdbny.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gewmeoapd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/gmuxntbml.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gourpyvlt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.vehdjk.com/Article/details/gptknjacp.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fktsv.cn/Article/details/ggdefzsom.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.sjlbkw.cn/Article/details/gbbaxbptt.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gtqvqbltl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/gexucjumx.sHtML


<!-- 参考信息 -->