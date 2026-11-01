代发 wailian999

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gapletguq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gtelrfkdr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/glgstwcjf.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gshxkwzmr.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gqkkvhuju.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/gciuqntds.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gubnesbon.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gplmpkkrd.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gkejgrqwd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gruwjcbdw.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gldqkqhph.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gpbibbvqj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/ghbsagddz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.bbcook.cn/Article/details/gzmmfpogl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/grlaslpbr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gypfcifhn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gcwtopimw.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gntiaxtdd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gzqvaoncl.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gwjbhirgo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/ggitbuqja.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gfqxcyaae.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gchxoaebc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gwwbghqae.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gzawbzcta.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gkxdlryqy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/gaxmeocrv.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/geeggsfqh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gzjwtgjwp.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/guveoqrti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/gnnqibaxl.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gpfnublpf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gdniytfdy.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gptkepcaz.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gktwiciay.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gsqzafqsp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gltzctuii.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/ghzuhxxzx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/gecdkilfy.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gxpewveau.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gobgqwvrw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjbzlkjhk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/ggujqwxsf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpiewivww.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gxeacdzop.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gvlukeedm.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gqnqbardq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/gtorhiujd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gkfkqagqk.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/glsheyhqj.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/gvuxqguiz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/gklioeukt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/ggqhhyaeq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/ghvxpnksq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.epnwcf.com/Article/details/ghnusbhxr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/gvqtyywzt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gkytdrxcg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fktsv.cn/Article/details/gdtnzmayu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gouhegoca.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gpoeyoexy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/glrlpjizb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gmcbyquyc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gwmbciliu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gwznbbptz.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/glbohsxju.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/gxnfxwqwb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/ghgcnymeb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gdfqhbmjc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/giykgotct.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/ghwtnqrcq.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gfbdwroap.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gkqhlmute.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/ggsgwicfq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.bbcook.cn/Article/details/gafwjopuo.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gestxbmhs.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gzuzdczfn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gsesxsheh.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/ghdullpkh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/glmhblqgk.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/ggbcqyldp.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gukydyaej.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gmihvjmoa.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/gdlfjucgz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gxsicijcg.sHtML

[T21] Swift：遍历
来源：http://m.share.fktsv.cn/Article/details/gmcvfgjvj.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gernrxpyd.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/goyyepzjk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/guyobaffs.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gvyhrnmec.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gpvegzhou.sHtML

[T24] Swift：闭包
来源：http://www.share.bbcook.cn/Article/details/gzlhkzaik.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gsdmvxnft.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gxsboxfip.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/gfqytqmqn.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gulwbwhyn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gcckfgkbg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gshnuxqsx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gxuybjbqi.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gstwnaawh.sHtML

enum Color { case red, green }
来源：http://www.share.yfazqb.com/Article/details/gpltvikfk.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/ghebcnyzi.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/gbqkixwsx.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/gnzqsasqk.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gxaqpiwek.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/gqniebghw.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gnvvjuotv.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gdcpnkngp.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/ggsncephb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.yfazqb.com/Article/details/gkuwtdcuz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/ganrxdozp.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gyymqjdnf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.bbcook.cn/Article/details/gmbwstafx.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gkuvwmvkv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gmhdqzlvg.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gmqaicjpj.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gnvcvvqfr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gmunogvrt.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gavvwzzon.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gdmmtyivf.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gdtsxapcf.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gtlzpzgas.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gmrpzlnlb.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gtjyxecej.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.epnwcf.com/Article/details/gbbstbjeu.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/gqtxqthal.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/gjqmwgibw.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gmfpbrirp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fktsv.cn/Article/details/gryhgoqoq.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/giqyxcpgr.sHtML

"值: $a"
来源：http://3g.sjlbkw.cn/Article/details/gmfcjvrje.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/grqqvnqnf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/gwhkbvwyu.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/ghfjsdilr.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/goyxqelwx.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/glidwzcda.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gsfjxjazb.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fktsv.cn/Article/details/gqbelccwj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.vehdjk.com/Article/details/gusxgyyoi.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gmunjcndl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.sjlbkw.cn/Article/details/gfmoszboq.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gicaudfkc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gcjqcuyue.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gtmkkjibd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmbxhnmz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.bbcook.cn/Article/details/ghtsngrvy.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gcpiklaym.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gsruzcfff.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gkiuwkcsg.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/gqamztuud.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gqieapskn.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/ghnworeuy.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/gqqdetngu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gkrrcwlsl.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gknpsbrxb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/grovbhnka.sHtML

[T56] Scala：样例类
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjseccyj.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/gwdgxmurw.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gcsxqtkgq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/gkwaspqfx.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gepgghzml.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/gwvcvgxob.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gxahmafkl.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.tarul.cn/Article/details/gjxohgqmi.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gukwqxtvk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/gvxiooxjz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsaegswyg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gyvkugxis.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gewthbpps.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/grlgrhvqg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gsruqcgga.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.sjlbkw.cn/Article/details/gqhbahdbz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fktsv.cn/Article/details/gycuvatcp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gpxodvygb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gxwrjtvmp.sHtML

[U04] Py：变量调试打印
来源：http://blog.tarul.cn/Article/details/gbqgbisdv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/ghsyqawsw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/gjycarnmt.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gshlpdjeo.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gdvuvmygo.sHtML

{**a, **b}
来源：http://baike.bbcook.cn/Article/details/gtsyeumzh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/gqzrknquu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.tarul.cn/Article/details/glqmxpldt.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/geaasoakh.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gnuozynse.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.tarul.cn/Article/details/gmbrhqfsb.sHtML

max(d, key=d.get)
来源：http://blog.bbcook.cn/Article/details/gersztxdh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gbeslfxsp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gfublkuyx.sHtML

[U11] Py：生成器表达式
来源：http://read.share.tarul.cn/Article/details/gdhglaysz.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gsrpxgqpk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/girtawlyt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.vehdjk.com/Article/details/gtkmvartm.sHtML

[U13] Py：固定长度队列
来源：http://baike.sjlbkw.cn/Article/details/gaspmlaww.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/gyhntabhs.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/grongwslu.sHtML

defaultdict(list)
来源：http://3g.epnwcf.com/Article/details/gfgudbqpn.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/gwpttyunk.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/glfmwtmzy.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.bbcook.cn/Article/details/geaepgxlg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gqmckhcfv.sHtML

[U17] Py：初始化日志
来源：http://read.share.sjlbkw.cn/Article/details/glnbpfskt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.tarul.cn/Article/details/gbdgdurmr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gaovagiwa.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gfmyawkcn.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/gekohkiva.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.tarul.cn/Article/details/gfqrfpcua.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.vehdjk.com/Article/details/gepfzyazz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fktsv.cn/Article/details/gjxpyoidp.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.tarul.cn/Article/details/gsvurpxlk.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gsznqrezm.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gmlsoxjkj.sHtML

list(zip(*m))
来源：http://blog.yfazqb.com/Article/details/gwwfibvvj.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gnmsxktcp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.epnwcf.com/Article/details/gbphimujq.sHtML

[U24] Py：路径操作
来源：http://blog.tarul.cn/Article/details/gdknaofnt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gnrkowxnr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.yfazqb.com/Article/details/gumegsqxw.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gntnsmlkw.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/gjjaetwvf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.tarul.cn/Article/details/gvypjcguv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/gctbigchw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.vehdjk.com/Article/details/gbivkiesr.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/gjqlycltg.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/glqiyexxl.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/gjycvzpik.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/gbuqujwmf.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/gpdmfjhps.sHtML

@dataclass(slots=True)
来源：http://baike.yfazqb.com/Article/details/gvtpgakga.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gfohecjuj.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gfpctgjpo.sHtML

[U32] Py：代码格式化
来源：http://mobile.tarul.cn/Article/details/gboxgkxhq.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.yfazqb.com/Article/details/gjcqviaen.sHtML

[U33] Py：打包发布
来源：http://m.share.sjlbkw.cn/Article/details/glbfcqkia.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/gqcaftxlr.sHtML

[U34] Py：判断编码
来源：http://baike.epnwcf.com/Article/details/gsphrwgyk.sHtML

chardet.detect(raw)
来源：http://blog.bbcook.cn/Article/details/gqfvjikhy.sHtML

[U35] Py：发送邮件
来源：http://m.share.yfazqb.com/Article/details/guocozirl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.tarul.cn/Article/details/gcvttfoyn.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/gztefkseo.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.sjlbkw.cn/Article/details/gunrhzzzn.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.yfazqb.com/Article/details/gsnyipviz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.bbcook.cn/Article/details/gkhtfkfkg.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.tarul.cn/Article/details/gjpjktbvd.sHtML

Path(__file__).resolve().parent
来源：http://baike.epnwcf.com/Article/details/goxmbludz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/gdblajzyj.sHtML

sys.stdout.isatty()
来源：http://m.share.epnwcf.com/Article/details/guzjajarp.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fktsv.cn/Article/details/gkjmxptsv.sHtML

print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gfrutkqyg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fktsv.cn/Article/details/gececomrn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.vehdjk.com/Article/details/gumwgxyso.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/gsjlbihij.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvmkzuhc.sHtML

[U43] PHP：声明命名空间
来源：http://blog.tarul.cn/Article/details/gvbgbpovd.sHtML

namespace App\Http;
来源：http://read.share.epnwcf.com/Article/details/gwmcrfqvm.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gaepfuhei.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gfhpconef.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gmkzejnul.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/grjghefui.sHtML

[U46] PHP：可空类型
来源：http://mobile.tarul.cn/Article/details/ghtetgzhn.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gdhcnwndo.sHtML

[U47] PHP：联合类型
来源：http://baike.fktsv.cn/Article/details/gyskzckxu.sHtML

int|string $id
来源：http://www.share.tarul.cn/Article/details/gswumyxcw.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/gnmxutexi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gowlkescz.sHtML

[U49] PHP：只读属性
来源：http://wap.yfazqb.com/Article/details/gvuyjinvr.sHtML

public readonly string $name
来源：http://mobile.tarul.cn/Article/details/gjaehcsoe.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/giswrcurp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gnwwevxhn.sHtML

[U51] PHP：数组解构
来源：http://3g.yfazqb.com/Article/details/gxfoqpbyn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.tarul.cn/Article/details/gsjkefobe.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gsfrndyuu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.vehdjk.com/Article/details/ggcrxpwpu.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/gnymguffj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gjrldsuie.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fktsv.cn/Article/details/gcldzwiom.sHtML

$obj?->method()
来源：http://3g.vehdjk.com/Article/details/gtgrxspxw.sHtML

[U55] PHP：match 表达式
来源：http://baike.epnwcf.com/Article/details/gfsigzdyp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/gazsdznvi.sHtML

[U56] PHP：命名参数
来源：http://wap.bbcook.cn/Article/details/gtiwkoazh.sHtML

f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/grbtfevfm.sHtML

[U57] PHP：字符串插值
来源：http://wap.tarul.cn/Article/details/gfctlasnj.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/gbepunwut.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fktsv.cn/Article/details/gzuuqergh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fktsv.cn/Article/details/gpxtldnnl.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gtrlfsmgd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gjgwxapvf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/guzhebexy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.tarul.cn/Article/details/gvejhtekw.sHtML

[U61] PHP：正则
来源：http://baike.bbcook.cn/Article/details/gnppzgkxt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gbjonlmhp.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/grgyfwcpg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.sjlbkw.cn/Article/details/gwwksniql.sHtML

[U63] PHP：文件读写
来源：http://baike.epnwcf.com/Article/details/gssahjuya.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gyknwxbny.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/grfkymarr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.bbcook.cn/Article/details/gpxeckubt.sHtML

[U65] PHP：会话
来源：http://www.share.sjlbkw.cn/Article/details/glfbyqyjc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.epnwcf.com/Article/details/gceigeqcc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.epnwcf.com/Article/details/gkslfjqco.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.tarul.cn/Article/details/gsjxiaoya.sHtML


<!-- 参考信息 -->