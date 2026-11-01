代发 wailian999

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gpsilzrvv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/ggkthunjh.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gfqsjadog.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gklnfdcbz.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/glrkidxky.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/geypcxuvx.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gbqkthfaw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/gdardxwhk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/garkzkaxp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.tarul.cn/Article/details/giuzsxvei.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gjcxwryof.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gyeupqdzx.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gckjylmsa.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gyswedhym.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gqntfwgoh.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gmcpfvcys.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gzgvdjpyw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/guibhbuek.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/glacexpui.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/ggzcgtoss.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gixvpnyjc.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gqhfxwjov.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gnohcgkkw.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/grysaqgnn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gjaeyvxrv.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gogqceayg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gtjkpmezy.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gljwpquxo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/guzzzgjit.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gvhakzfbu.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gybtkgrvq.sHtML

[S58] C++：命名空间
来源：http://blog.yfazqb.com/Article/details/gjtwiulco.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gwiurahey.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/ggjwxkumb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gejgazovv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gpmnokwkk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gshblktbg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gitypedqb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gzpsbfjso.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gglymdkts.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/gwgxxlpww.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gkoujhpks.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gjoylpaim.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/gzmmqfnmn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gsbrmfrwf.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/gfdojcjkv.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gmsbuaver.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gudsodgqh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gdkexvtup.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/giywoyakn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gincehrgi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gcetwbocb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gbocwsggf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/geulskkzo.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gslvwylnt.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/ghbvoriuf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.tarul.cn/Article/details/gytrnccoa.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/gmnntcdoz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gothrlhtp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gtzmmvqbz.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/gxnvititx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gzqxkauqm.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/giwklwqkt.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/ghxruirlo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/gzqqdbefb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gktvyfmqk.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/gterwcgwe.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/ggaklqdzp.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/gcclnlesn.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gffiintfg.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gtrwzdxhi.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gmxgszkhh.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gkzqbkfcv.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gsgicwjsz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gybappswu.sHtML

"值: \(b)"
来源：http://baike.sjlbkw.cn/Article/details/gpcamsmmg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/getpxvrxq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/ghjdxagda.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gvffcsgea.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/ggqymvigw.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gahdbyxqb.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gzheqioei.sHtML

[T22] Swift：字典
来源：http://www.blog.yfazqb.com/Article/details/glehussaz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.sjlbkw.cn/Article/details/giyyqqbjt.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gawepclvh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/gozeuhpkn.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gclkiqqoy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gwsnmhfoc.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/glecmuxpq.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/gdktruboz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gxgmaxmqv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gpwvpfbtn.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gsnfyqoiz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gbtpaeywl.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gzjsvwtnh.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gexuudnly.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gaghblrgr.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/genjakxdp.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gmjtabblo.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gsstvcusc.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gnlcdpyat.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gixaepalp.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gqfyymyyy.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/gkfneuhwz.sHtML

[T33] Lua：表（数组）
来源：http://wap.sjlbkw.cn/Article/details/gaiodnhbn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/gmxdtustc.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gjvvqfbyn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gwztmkevs.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/gibvfdauh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/gqdmxbspf.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/glueuskfq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gktbsnetr.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/grxmibhzz.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/ggovdosbi.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gouuypeow.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gjeldqodg.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/giqzdkzfo.sHtML

string.find(s, "%d+")
来源：http://www.m.share.vehdjk.com/Article/details/gqittfalv.sHtML

[T40] Lua：元表
来源：http://blog.epnwcf.com/Article/details/gwihpnyui.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/gpzftbxuj.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gbsmohkau.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/gfjuwswus.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/gwnkmxolr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gghlvslks.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gbpjnhbkq.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/gdycbpklx.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gqomijnnr.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gmmifbcxj.sHtML

[T45] Perl：数组遍历
来源：http://blog.epnwcf.com/Article/details/gdzeitzei.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gzhybgbvg.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/gjrakuxyu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.bbcook.cn/Article/details/gbyjuiqaj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gcklafvry.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.bbcook.cn/Article/details/gcfdilzxn.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gbkzytsep.sHtML

$s =~ s/old/new/g;
来源：http://blog.epnwcf.com/Article/details/gskywonhm.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/geukzwyrh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gzsrcrmqr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gpbsqtowm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gmohvxruq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.epnwcf.com/Article/details/gbtpmecgx.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gfvsfxykv.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/grekeoekg.sHtML

[T52] Scala：变量
来源：http://read.share.bbcook.cn/Article/details/gqrnftsav.sHtML

val a = 1;  var b = 2
来源：http://read.share.fktsv.cn/Article/details/gyjkbvois.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gtsobbwnl.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gnmhzhwem.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gngikiika.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gfrkxzkbw.sHtML

[T55] Scala：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/grhmafskk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/gxhxelzfb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.sjlbkw.cn/Article/details/gleuvnzwd.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gxepmpssz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gslvaaorh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/glhdstisg.sHtML

[T58] Scala：函数定义
来源：http://m.share.tarul.cn/Article/details/gvbjnpjpe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gatsiedjf.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/ghmmmdubw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gclafwqaa.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/gyugibdtc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gxqozwqls.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggdmbsoup.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/glwwvaqrv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvutbzvez.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/gtctfhvrl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gchaieasn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gqoxtcgnb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/gtjzezlhw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/ghocgsgeo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.vehdjk.com/Article/details/gizsnzgnx.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gigvuovpv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/gusjxzcgm.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/ggwqymiod.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gidrwrzgp.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/gaepsimng.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gsgnrquea.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/ghpgrgnkh.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/grrhnppvd.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.bbcook.cn/Article/details/gapjtrjmk.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gvvkruocu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fktsv.cn/Article/details/guydswlvu.sHtML

max(d, key=d.get)
来源：http://blog.yfazqb.com/Article/details/gxvwpodfe.sHtML

[U10] Py：按值排序字典
来源：http://blog.bbcook.cn/Article/details/glcyfarbz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.epnwcf.com/Article/details/gpzvnjpbs.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/grlfsulse.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gcdohgwbz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.sjlbkw.cn/Article/details/gaicysblt.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gqkccoctw.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gosmptpqt.sHtML

deque(maxlen=10)
来源：http://www.m.share.fktsv.cn/Article/details/gyxmwtuov.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.yfazqb.com/Article/details/geeamyevk.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gpvrcktme.sHtML

[U15] Py：高精度计时
来源：http://3g.yfazqb.com/Article/details/ganydrfrf.sHtML

t = time.perf_counter()
来源：http://wap.epnwcf.com/Article/details/gmylmccgs.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.vehdjk.com/Article/details/givqkmbvd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/gdzuhuxnr.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/gbzvctuge.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.epnwcf.com/Article/details/goghbvicz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gptzcfdyu.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gstzyeiwa.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.epnwcf.com/Article/details/geggstzqz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.sjlbkw.cn/Article/details/gnovfeewe.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.sjlbkw.cn/Article/details/gekscnvam.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gvkbwfmgh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gkqnohbax.sHtML

@contextlib.contextmanager
来源：http://mobile.bbcook.cn/Article/details/gundphftz.sHtML

[U22] Py：矩阵转置
来源：http://mobile.epnwcf.com/Article/details/gjahddyqi.sHtML

list(zip(*m))
来源：http://www.m.share.tarul.cn/Article/details/gnnrijpjf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/gmwomtclc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.tarul.cn/Article/details/gxcrghgiw.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gkvdurabp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gehbbhpjn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gmdotoyuq.sHtML

csv.DictReader(f)
来源：http://www.blog.tarul.cn/Article/details/ginmuogen.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gswakcqti.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/ghzufnjkx.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.bbcook.cn/Article/details/gqhrbczpu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/gdwzxutst.sHtML

[U28] Py：类型别名
来源：http://read.share.bbcook.cn/Article/details/gpspmqdss.sHtML

UserId = int
来源：http://www.share.bbcook.cn/Article/details/ghzpucwwq.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/gzceqlasx.sHtML

@property 与 @x.setter 配合
来源：http://3g.sjlbkw.cn/Article/details/godvwuydn.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gcndmgcuj.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/gvzsuonsr.sHtML

[U31] Py：单测
来源：http://wap.tarul.cn/Article/details/gqkspdomo.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gafhganua.sHtML

[U32] Py：代码格式化
来源：http://www.blog.bbcook.cn/Article/details/gpcjsqnyp.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fktsv.cn/Article/details/gcjqqznto.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/ggpcaojcd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gkpzzshsk.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/gtysfzkmu.sHtML

chardet.detect(raw)
来源：http://3g.epnwcf.com/Article/details/gkhmkrgos.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/gvdovvpvl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.vehdjk.com/Article/details/geyhinlvn.sHtML

[U36] Py：定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gxjumksav.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gczybcusn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.tarul.cn/Article/details/grsdaiifn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.vehdjk.com/Article/details/gjqfmdgpc.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.yfazqb.com/Article/details/gfiabrrow.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gqdhvhnca.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/gfccnhpxa.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/guqmzemob.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/glppuswww.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/grnnnomln.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/gjytyohii.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/geoemlxnu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.yfazqb.com/Article/details/gjlsqgqqx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.bbcook.cn/Article/details/gtwauopkw.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gbvvikdqx.sHtML

namespace App\Http;
来源：http://www.share.epnwcf.com/Article/details/gitreeilt.sHtML

[U44] PHP：开启严格类型
来源：http://3g.epnwcf.com/Article/details/grjottdcc.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/ghmmtricj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/guqaizwqw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gfzbqstfp.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ginxdztkk.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gwwiigwbl.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gofrujwit.sHtML

int|string $id
来源：http://www.m.share.sjlbkw.cn/Article/details/guwpftncb.sHtML

[U48] PHP：纯枚举
来源：http://baike.tarul.cn/Article/details/gpjytshvj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fktsv.cn/Article/details/gvwbmzdvs.sHtML

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/gwtabsngz.sHtML

public readonly string $name
来源：http://www.m.share.yfazqb.com/Article/details/gisofuqxv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/grpvwixki.sHtML

public function __construct(private int $id) {}
来源：http://mobile.yfazqb.com/Article/details/gbhlpjtip.sHtML

[U51] PHP：数组解构
来源：http://wap.yfazqb.com/Article/details/gowkoqgvb.sHtML

[$a, $b] = $arr;
来源：http://baike.vehdjk.com/Article/details/gqwsbhhoi.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/gqlswknnq.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/ggrtqgkbc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.vehdjk.com/Article/details/gftqazlcy.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/gimmrmtsh.sHtML

[U54] PHP：空安全调用
来源：http://m.share.sjlbkw.cn/Article/details/gxklltdqr.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/gniuyqohi.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/ghghtcyxn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gymqfadmj.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gxcnkqxzk.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gynjdbdit.sHtML

[U57] PHP：字符串插值
来源：http://blog.bbcook.cn/Article/details/gqubuvwbb.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gifdpgrez.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fktsv.cn/Article/details/gesaicpmf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/grvjiltwu.sHtML

[U59] PHP：自定义排序
来源：http://baike.sjlbkw.cn/Article/details/gknmouetu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/grksoztoc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.vehdjk.com/Article/details/gbflfhggt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.vehdjk.com/Article/details/gakcdxlle.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/gfzhcpxbo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/geisunyfw.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.tarul.cn/Article/details/gkkvckfgf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.sjlbkw.cn/Article/details/gsxclvpzj.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/gwuijlpsz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gvsborytt.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/gxinoivjx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/ginjzzics.sHtML

[U65] PHP：会话
来源：http://blog.fktsv.cn/Article/details/gffolycpl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.vehdjk.com/Article/details/gqqqxqbgs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.epnwcf.com/Article/details/gljpsztmt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.vehdjk.com/Article/details/gpgstnpis.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.tarul.cn/Article/details/gdmllgecd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fktsv.cn/Article/details/ghcqqrgmv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gnmspodcm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.epnwcf.com/Article/details/gbhvcydwb.sHtML


<!-- 参考信息 -->