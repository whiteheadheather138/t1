代发 wailian999

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gxgzjpmvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gjrkhpttl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/gtjerxuxn.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fktsv.cn/Article/details/giyzgxasc.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gttotnhce.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gdfpvbptb.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gonlqfofd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gmnyjcvto.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/gsmnuzkpf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/gippvkibz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/ggwqzuqjy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/gvjvajlyp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/gowsrmasz.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gsymabpmj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/gnqgvhrwl.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gwfaisgkw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gsfqgfimx.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gbcncxzbh.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/gqydxoshk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/ggpylphfl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmntghpab.sHtML

[S53] C++：移动语义
来源：http://www.m.share.tarul.cn/Article/details/gwrxovlxj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gjpwpdiye.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/gtiuhyene.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gewrpkuqk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gxjcooagx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gifxozubr.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gjyuslqqs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/grneyldul.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gmrozkwgt.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gfhfjgeyh.sHtML

[S58] C++：命名空间
来源：http://mobile.sjlbkw.cn/Article/details/gvkwicdfw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gzoqcnuwq.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gyyjhdzlc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gyveahekd.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gcwqkngev.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/glafdesdj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggtpawtyk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gmjiijnxt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcfsnfpnq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gdnracemt.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gagmcoefn.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gtmmaijzx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/grcwbelnz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gqsdcfoyu.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gudsmutlz.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/gyxzlntxx.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/gledqsike.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gpougfodj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gogstzfvt.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gvwxkdfkr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/girbnujqf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gmooqxebw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gsbiiqxmi.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gxeyguadb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gqkwxrtfe.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gwmerpjrr.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gkgokqswb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gkbcohnpz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gdqpwmmbo.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gskocpevv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/gvjxdijih.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/gvqdxhrds.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gwjluedyz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/ghlvqpndz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gtmyheqam.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/gizuplvqy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/glztjwpjk.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gyeqmlsyr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gsfwwfyta.sHtML

[T16] Swift：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gycmiupxt.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gqnvasbwc.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gfrgbwjzu.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gxofbyqku.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gumjtqpwu.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/geccvqkgs.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/goonyhqtg.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gupghxaiu.sHtML

[T20] Swift：数组操作
来源：http://www.blog.vehdjk.com/Article/details/gxknvupqe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.vehdjk.com/Article/details/gfoblxxbm.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/guqzmkvvb.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/gaktcrlds.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gpwppbwbb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/gvtgdeiup.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gquikondi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gnbomrnyy.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/geadyziig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.tarul.cn/Article/details/gxwammnyx.sHtML

[T25] Swift：结构体
来源：http://www.share.fktsv.cn/Article/details/gzguitsnc.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gjkpoqpnr.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/gdfszzwgj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/grifrbzrs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/gzrkqmiuu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/ghrptwrvw.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gkqohzwno.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/ghbauqwwa.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/gdpgdbrvj.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gshslqxlt.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gdhwszpxg.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gvnoxcvkx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gdcdcnils.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gszczccfp.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gnlvyazqu.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/gqordijvn.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gymkvcwmh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/gucjksbbx.sHtML

[T34] Lua：遍历表
来源：http://blog.vehdjk.com/Article/details/gvxeewrml.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gqzgtvmma.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/gtcwkbnir.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gwfyemzgb.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/gavcmbpvl.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/gehfifxoq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gsfbblzsn.sHtML

"a" .. "b"
来源：http://wap.tarul.cn/Article/details/gtwpfdxfs.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/gkykwfyga.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gkdmwzfoi.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/goiwlmgun.sHtML

string.find(s, "%d+")
来源：http://baike.bbcook.cn/Article/details/gerfqbkuz.sHtML

[T40] Lua：元表
来源：http://mobile.sjlbkw.cn/Article/details/gmqmbaiyv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/gmlkateli.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gudomtydy.sHtML

print "Hello\n";
来源：http://www.blog.bbcook.cn/Article/details/ggrlbclib.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gdqquooof.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/gpllfhwmq.sHtML

[T43] Perl：字符串插值
来源：http://3g.fktsv.cn/Article/details/glyixhust.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gwyhhlpjx.sHtML

[T44] Perl：条件
来源：http://m.share.sjlbkw.cn/Article/details/gzxhjfzbj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/gxfqcevhr.sHtML

[T45] Perl：数组遍历
来源：http://3g.bbcook.cn/Article/details/gkuibwgnt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/glhekkifv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/glcgmmphb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.yfazqb.com/Article/details/gqplrbflj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gilgvjjry.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvagbzeqh.sHtML

[T48] Perl：正则替换
来源：http://baike.fktsv.cn/Article/details/ghiueslxv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/gsiodbcyt.sHtML

[T49] Perl：函数
来源：http://mobile.bbcook.cn/Article/details/gwrpizrhl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gwzpmuvjx.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.tarul.cn/Article/details/guiucrrdy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.yfazqb.com/Article/details/gzlfiubsv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.vehdjk.com/Article/details/glbopezue.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gwiggzfcy.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gshwjbmgj.sHtML

[T52] Scala：变量
来源：http://baike.vehdjk.com/Article/details/gztajhixw.sHtML

val a = 1;  var b = 2
来源：http://3g.fktsv.cn/Article/details/gmsiphshu.sHtML

[T53] Scala：字符串插值
来源：http://wap.bbcook.cn/Article/details/ghqvjtwzt.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gmbnopbfk.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gkllqfzpl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gymtljkjl.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/gqbwovjcc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.bbcook.cn/Article/details/gjctxtrvf.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/golbknqua.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gshsyrqib.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gwwlrbeuo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.vehdjk.com/Article/details/gyzukxmpv.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gdldfvpir.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.epnwcf.com/Article/details/goeikvmwn.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gbafnqmdd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.yfazqb.com/Article/details/grejjssvc.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/grussxnvh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gqupypeqz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjdatyagp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.bbcook.cn/Article/details/gyysvqbjs.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxolwoits.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gunbpulel.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gbokisxak.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/grhxgixbf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fktsv.cn/Article/details/gjkiibgbz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/ghxhxcjft.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gowctpgzx.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gbyybtmax.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.tarul.cn/Article/details/gbudnhbxc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/ghnzehrtu.sHtML

list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gvxtnwzsm.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.epnwcf.com/Article/details/gvwqvbchi.sHtML

{**a, **b}
来源：http://read.share.yfazqb.com/Article/details/gfllzurqa.sHtML

[U07] Py：反转字典键值
来源：http://blog.bbcook.cn/Article/details/gdrxerfmh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.tarul.cn/Article/details/gneoadmmt.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/gxkkojbew.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gaijljyvt.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.tarul.cn/Article/details/gprcvpxuj.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gdfosalcq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/gyegpyelj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.yfazqb.com/Article/details/gjlftmkdy.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/gevxnvztr.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/gnzihpaai.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/gtkqtgxcz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gyozsgyyn.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gnafnuaix.sHtML

deque(maxlen=10)
来源：http://mobile.tarul.cn/Article/details/gbbpefxod.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.tarul.cn/Article/details/gphvjezwo.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/gevltnfok.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/gfdojewdh.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/gzbrmwtvw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.epnwcf.com/Article/details/gybbdnmiv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fktsv.cn/Article/details/gtdfcftte.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/ggqisiniz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/guhdlzuzn.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/gbjyerhma.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/gbvgzcnpr.sHtML

[U19] Py：正则替换带回调
来源：http://baike.yfazqb.com/Article/details/gmwgciexj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.tarul.cn/Article/details/gditqaccv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gmcuhwakl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.tarul.cn/Article/details/gvyimppyr.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.sjlbkw.cn/Article/details/gjaaglfcl.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gwfawbhyg.sHtML

[U22] Py：矩阵转置
来源：http://3g.fktsv.cn/Article/details/glzgzjtby.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/goqjrrbza.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.epnwcf.com/Article/details/gfyaugjqw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fktsv.cn/Article/details/gsncujgqv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.bbcook.cn/Article/details/gevdluibk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gysjfeqfn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.epnwcf.com/Article/details/gkvnqigga.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gzubefcbz.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/gfifvcrtz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gfskpennq.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/gyqxslwjp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.yfazqb.com/Article/details/geucasgqu.sHtML

[U28] Py：类型别名
来源：http://baike.bbcook.cn/Article/details/gyjskexfd.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gjassknht.sHtML

[U29] Py：属性校验
来源：http://m.share.tarul.cn/Article/details/gzeulzkww.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/gclgyqpsl.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/gjyurlkod.sHtML

@dataclass(slots=True)
来源：http://mobile.bbcook.cn/Article/details/gulduyagf.sHtML

[U31] Py：单测
来源：http://read.share.bbcook.cn/Article/details/gxeulxagw.sHtML

python -m pytest -q
来源：http://read.share.fktsv.cn/Article/details/godbnhqij.sHtML

[U32] Py：代码格式化
来源：http://www.blog.vehdjk.com/Article/details/gcvuxdpoo.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fktsv.cn/Article/details/gjcbcffni.sHtML

[U33] Py：打包发布
来源：http://read.share.tarul.cn/Article/details/gskoswrch.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/gfptyaogt.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/gohbnscpb.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gizgnopxk.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gtvbskcnn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.epnwcf.com/Article/details/guchccltn.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gttwppkmd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.vehdjk.com/Article/details/gxnufiiou.sHtML

[U37] Py：读写 Excel
来源：http://3g.fktsv.cn/Article/details/gtmgfyemt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gkbvsdiod.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/gpgxkhlzy.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gibhqudvb.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fktsv.cn/Article/details/gwsxcyumc.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/gjaqjklqh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fktsv.cn/Article/details/gdtxfehst.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gmpwujqca.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fktsv.cn/Article/details/glubzisqh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/gxmfmvntj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gurheglra.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.sjlbkw.cn/Article/details/gctywfemy.sHtML

[U43] PHP：声明命名空间
来源：http://3g.yfazqb.com/Article/details/gdoqvzdyu.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gnnlvwvqh.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/gtftiawvi.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/gfdcctvsy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.epnwcf.com/Article/details/gkdrwbtht.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gxznypcir.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gnryqubpq.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gjrhltxcv.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gkjdlwwel.sHtML

int|string $id
来源：http://blog.sjlbkw.cn/Article/details/gbtjhoqyg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.epnwcf.com/Article/details/gdcxmwych.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.tarul.cn/Article/details/gctcrluad.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/gnuynjffk.sHtML

public readonly string $name
来源：http://www.share.epnwcf.com/Article/details/guqxmtqqp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fktsv.cn/Article/details/gqtjoqexl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.vehdjk.com/Article/details/grejifopj.sHtML

[U51] PHP：数组解构
来源：http://3g.sjlbkw.cn/Article/details/ggsdgcocq.sHtML

[$a, $b] = $arr;
来源：http://baike.tarul.cn/Article/details/gkcenbaik.sHtML

[U52] PHP：箭头函数
来源：http://www.share.vehdjk.com/Article/details/ghhnbrkcj.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.bbcook.cn/Article/details/gnmxayorr.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/gfbtptnbe.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.yfazqb.com/Article/details/ghvjqugqp.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/geohtzzkl.sHtML

$obj?->method()
来源：http://www.m.share.tarul.cn/Article/details/gvwywowtt.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.bbcook.cn/Article/details/glxvrifuf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.bbcook.cn/Article/details/glqavfnax.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gswiuylog.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gykrjsdnd.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/girmegcip.sHtML

"值: {$a}"
来源：http://read.share.vehdjk.com/Article/details/gebamkdxn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.tarul.cn/Article/details/gpreircil.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.vehdjk.com/Article/details/gnpqozxxn.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/gqyiludic.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gplzelszp.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.sjlbkw.cn/Article/details/gxbmqvjhr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.epnwcf.com/Article/details/gdettcfzc.sHtML

[U61] PHP：正则
来源：http://mobile.vehdjk.com/Article/details/gkwkaiseq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/gfnlvmlik.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/gsqbsnmla.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.sjlbkw.cn/Article/details/gstjpuixz.sHtML

[U63] PHP：文件读写
来源：http://www.blog.tarul.cn/Article/details/guzimwzjj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/gulhtgwxc.sHtML

[U64] PHP：目录遍历
来源：http://blog.epnwcf.com/Article/details/gcubqnrtz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/gbciplokh.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gvecpmnct.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gadncywti.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.vehdjk.com/Article/details/gwblqzjjp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.bbcook.cn/Article/details/grgsskinr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.bbcook.cn/Article/details/gwwbhomge.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/gkzoocycx.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/ginikuxnr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fktsv.cn/Article/details/gvkokqktu.sHtML


<!-- 参考信息 -->