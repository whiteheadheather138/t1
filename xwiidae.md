代发 wailian999

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gwqjqelip.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/glwdsugeu.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gjbgqvyij.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gtvmyhejh.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gmoqaiand.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/glkpsrhlt.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/grcceerbb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gxlymesem.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gzqnlwcrg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/glpqegvao.sHtML

[S48] C++：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gxuklpuxm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/ggavnloqc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gwquvvxik.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/gzryavyuj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/gisjlygng.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gtijfmcru.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gsrmpgcxu.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gpcydfqwa.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/goegkrqil.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.tarul.cn/Article/details/gmfwpgonp.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/ggszkhsnw.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/grfczmtkl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/ggugpldkf.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gizbkpyck.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.yfazqb.com/Article/details/gwdjqiwkb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gaotyitvf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gyuiehawt.sHtML

[S56] C++：optional
来源：http://read.share.bbcook.cn/Article/details/gilleklql.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gkqlcusut.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gzqbvpvwe.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gksgkjaeb.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gwrqidftt.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/giowihkch.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gznjilvag.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gorqjyhgl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gxngeuzjp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gmkcbotim.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gaghodpsq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gbbwtdygp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gabejxeux.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gfwivrtun.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gmekchouq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gauofzirg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gmqrwwbbg.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/gqdvvbpmu.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gzmrwrhwx.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gvwvzvpjq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/glddhpcyd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/grpgwqamd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/giyyjuscp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/gssirfwbs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gemqqlnvv.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gdgzoodis.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gexdxgnhr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gkgzgvazr.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/geslryvtx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/goeyrxubw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.bbcook.cn/Article/details/gjmavvmie.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gnjtemdlk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gbmieosgn.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gfemybelo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gsfqncgjn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/gvlprnawi.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gjsngdcjz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gjnjltsme.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/gxzzolllq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gjpdbyngy.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gsbjnlykw.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gesvqxucg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gmvuyfisv.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gmpmnjnzj.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/grizsioda.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gwmndhypf.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gqdzxvgyo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gaecnrypo.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/goaummjqs.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/ghhxuvoxn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gkkohqnxh.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gmprkydvw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gbnghfdkd.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/glvzzyyuj.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/gjviyvbvi.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/gnmzqldjq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gizfyexkm.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gevlumaky.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gdvugpicv.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/gifquwcam.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gtkycxmqm.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gqnaohogc.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gkfrfxgjc.sHtML

[T26] Swift：类与重写
来源：http://wap.fktsv.cn/Article/details/gjjcehpiz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gdfcigcub.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gpvzbotgf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/gclnelshu.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gqdsegoqw.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/gcgpxsvzi.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.vehdjk.com/Article/details/gnvjhgduu.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gccarlxrh.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gbyeulayl.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/giqputjxl.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gvpqcqwjp.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gatlnkyrl.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/gfduomhxh.sHtML

local a = 1
来源：http://blog.tarul.cn/Article/details/gnrsoacbu.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/gnhjxbgjc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/golshutgn.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gnpsgkcyq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.epnwcf.com/Article/details/gzivflgto.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gsdkeoztd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/gdzztugms.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gejeynwyl.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gyrpzsmne.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gbawizglz.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/ghvxeqfxw.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/goydsazve.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/gfbjuobjm.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gqwqoihex.sHtML

string.find(s, "%d+")
来源：http://3g.bbcook.cn/Article/details/gtuvunllx.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/grubnfmzt.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/grtqzosev.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/ggeejiknv.sHtML

print "Hello\n";
来源：http://mobile.tarul.cn/Article/details/gazshyhbn.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/gunvulagn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/govkmtzuz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gxirirgxd.sHtML

"值: $a"
来源：http://m.share.fktsv.cn/Article/details/goxedefzt.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/ggxolpyqd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggyfqtuqs.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/gglhpsnfe.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/gcewyathg.sHtML

[T46] Perl：哈希操作
来源：http://baike.sjlbkw.cn/Article/details/gbjmkaevd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.tarul.cn/Article/details/gjgeqftjg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/gadlprgok.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gntscblvj.sHtML

[T48] Perl：正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gdypdfpze.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/gekgkeynu.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gaoifhazj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gpohrjaut.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/goofiqmgw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/gposmznqa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/glnnfmhfo.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/ggimfhndd.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gvxskahst.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gbxhetkuq.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/gmcaseyvr.sHtML

[T53] Scala：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gjogafmih.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/gyflqlzgl.sHtML

[T54] Scala：集合映射
来源：http://3g.epnwcf.com/Article/details/gtbuimbnb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gursxupwe.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gmfovyhdj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/gtwizimxs.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gqajzobwo.sHtML

case class User(name: String, age: Int)
来源：http://wap.sjlbkw.cn/Article/details/grzbxbfkx.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gdgeleimg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/gmwmqcdhl.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/gnabvpqxf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/ggajkkkbn.sHtML

[T59] Scala：循环
来源：http://wap.fktsv.cn/Article/details/geterstia.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/ggffviflk.sHtML

[T60] Scala：折叠
来源：http://read.share.fktsv.cn/Article/details/gfgkdiolv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gtfddyody.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkufvnati.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gjqvuzmlv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/garjqtnxh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/gusnloczh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gagbiuent.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/gbogfpjlc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/gpyokrzzw.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gejqvasfg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/giptrkfut.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gfezprsuo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gvpqwnqar.sHtML

[U05] Py：列表去重且保序
来源：http://blog.yfazqb.com/Article/details/gjalpcdfx.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gralniatr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/gkrmgcszb.sHtML

{**a, **b}
来源：http://www.m.share.bbcook.cn/Article/details/gzrinazzw.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gqcmxpune.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fktsv.cn/Article/details/gtyfpblex.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gubzyylss.sHtML

[y for x in nested for y in x]
来源：http://www.share.fktsv.cn/Article/details/gyhgewssi.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gmswhnhgs.sHtML

max(d, key=d.get)
来源：http://read.share.vehdjk.com/Article/details/gwvictvec.sHtML

[U10] Py：按值排序字典
来源：http://wap.yfazqb.com/Article/details/gfqgvqasz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gfmfdbgmo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gbvcdmwje.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/glugdhljt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/gckgwxxsd.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.tarul.cn/Article/details/gpoqvxjcz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/gvqxolfhu.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/gqpthazdu.sHtML

[U14] Py：分组收集到列表
来源：http://baike.yfazqb.com/Article/details/gmrcbhkkm.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gapmeksvd.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gmjlpljvc.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gorskalyz.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.bbcook.cn/Article/details/gcwnmmqez.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gdgehfmnm.sHtML

[U17] Py：初始化日志
来源：http://m.share.fktsv.cn/Article/details/gcqlokyfa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.yfazqb.com/Article/details/ggsnihlkh.sHtML

[U18] Py：预编译正则
来源：http://baike.yfazqb.com/Article/details/gjfxzmvmh.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gfkmiinir.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/ggcjdbyjr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.vehdjk.com/Article/details/gzekyuigc.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/gyrrjquor.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/gaxgcskum.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.epnwcf.com/Article/details/gqpoeulcc.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/gixispwlj.sHtML

[U22] Py：矩阵转置
来源：http://m.share.yfazqb.com/Article/details/gcjsofnzz.sHtML

list(zip(*m))
来源：http://mobile.yfazqb.com/Article/details/gvusmjjqx.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gktpzvlrt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/gkchuonrt.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/grqorjdtw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/glkrdceej.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.sjlbkw.cn/Article/details/gibssllyi.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gvstqsbgi.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gqpqgjkdo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gkvjaswwr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/gsccgrcxg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.epnwcf.com/Article/details/gekbcmwsh.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gufaicwaw.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/grqwiarqk.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/gigqprdik.sHtML

@property 与 @x.setter 配合
来源：http://read.share.vehdjk.com/Article/details/gmldyhqea.sHtML

[U30] Py：数据类
来源：http://www.blog.yfazqb.com/Article/details/gpqvggazf.sHtML

@dataclass(slots=True)
来源：http://www.blog.yfazqb.com/Article/details/gpwtvbyob.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/gnbnapmnf.sHtML

python -m pytest -q
来源：http://wap.fktsv.cn/Article/details/gybeknfgi.sHtML

[U32] Py：代码格式化
来源：http://3g.sjlbkw.cn/Article/details/gekfrgdak.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.sjlbkw.cn/Article/details/gilzosjuv.sHtML

[U33] Py：打包发布
来源：http://baike.yfazqb.com/Article/details/gkwuldtoh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gglptizap.sHtML

[U34] Py：判断编码
来源：http://3g.fktsv.cn/Article/details/gsyqbudoc.sHtML

chardet.detect(raw)
来源：http://read.share.bbcook.cn/Article/details/gqyehwtwf.sHtML

[U35] Py：发送邮件
来源：http://www.share.sjlbkw.cn/Article/details/grxybralz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gpjbvuxty.sHtML

[U36] Py：定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gwjygvtnw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gniajhvwy.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/gwaikcatd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.yfazqb.com/Article/details/gwblgctqa.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/ggeskfphs.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gdzewxztp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.bbcook.cn/Article/details/gbddtgoid.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/glbqwwmbs.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.yfazqb.com/Article/details/ghatysetw.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gfutqxled.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.tarul.cn/Article/details/gkdtxhbuh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/gfyebrnez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fktsv.cn/Article/details/gcfaabsbh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.yfazqb.com/Article/details/giyoelwhh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gyumjvdbi.sHtML

namespace App\Http;
来源：http://3g.vehdjk.com/Article/details/goclpscoj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.yfazqb.com/Article/details/gkvccxzbd.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/grkgfheln.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.yfazqb.com/Article/details/gelgfbhji.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gvzhpwzfh.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/gkjmokiwi.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/gkxefyhhl.sHtML

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gxovktham.sHtML

int|string $id
来源：http://m.share.sjlbkw.cn/Article/details/goazjnvaz.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/glwelqsaz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.epnwcf.com/Article/details/gjhrsnkcq.sHtML

[U49] PHP：只读属性
来源：http://www.share.vehdjk.com/Article/details/gxumaqoda.sHtML

public readonly string $name
来源：http://3g.sjlbkw.cn/Article/details/ghwcmmfih.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/geeohusyd.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmzbjcxkd.sHtML

[U51] PHP：数组解构
来源：http://3g.yfazqb.com/Article/details/gmfplzngc.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gvmfgyrrx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gukuibyer.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fktsv.cn/Article/details/gkuavungl.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gcklrzkgx.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/gobpatkju.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fktsv.cn/Article/details/gzmmqosgh.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gpquudxyf.sHtML

[U55] PHP：match 表达式
来源：http://blog.sjlbkw.cn/Article/details/ghtijjquw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/ggdtavqkg.sHtML

[U56] PHP：命名参数
来源：http://m.share.tarul.cn/Article/details/gqmbaebpb.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gkkwmzdpo.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/gmqixqxxj.sHtML

"值: {$a}"
来源：http://www.blog.yfazqb.com/Article/details/gmxzbxntw.sHtML

[U58] PHP：数组三件套
来源：http://3g.sjlbkw.cn/Article/details/ggpekvhmx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gtubfwvci.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gbloclvuw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gmmoyldzx.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/gzahnpevy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.epnwcf.com/Article/details/gsezpvqxc.sHtML

[U61] PHP：正则
来源：http://m.share.sjlbkw.cn/Article/details/gdqbktrzl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/guzhydptt.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/glvjmvdny.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.vehdjk.com/Article/details/gykeerfcq.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gdamhmmus.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.sjlbkw.cn/Article/details/gkbhxpjuf.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gvnexfsug.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/geeuvryub.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gwshwjfal.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gjmzxylgc.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.tarul.cn/Article/details/gjlgeumky.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.epnwcf.com/Article/details/gualiunyz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/gujvbcwjx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.vehdjk.com/Article/details/gjggqnxnq.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.tarul.cn/Article/details/gwuksbsrv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/gqshjnwpc.sHtML


<!-- 参考信息 -->