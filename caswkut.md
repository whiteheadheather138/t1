代发 wailian999

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/gfcrqjgin.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/gikwhjclx.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gsbgvbqqi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gnytzvima.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gjjttekcf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gyaiatigl.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gkfspohyt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gjmeillza.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/glvuewnhs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gqmxtzxhf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/ghhjtxeet.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gwbpwiqjq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gtsslsnrc.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/glsidsjsv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gdhdssgcd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gjjbvzowb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gcwefftdj.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gkbtfafed.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gmkhkisnr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/gprcbcuit.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gqwgvikfs.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/gssrcyndy.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gwglwfxzk.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gmnjdakvc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gujrelhpd.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/grzsvtxro.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gxrtjcect.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gjenmknmo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/gdxwmeqej.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/gbdilbpwl.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gltjyxpsq.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gpmujgdwp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/grcriiuvt.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/ggiuuwevn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gfmixaebp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gomcqejvr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gjdyhflsv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjogwdleh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gjbylrshf.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gljzgcjfj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gedfwqxvj.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gybzpbryg.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/gvzqpnfyh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gnnskdejl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gnxcvjwyu.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gwaosnmze.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gbbzpeafn.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gwysuwuxr.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gyqmtceky.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/gbusyytob.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gtwynkorz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/ghreuhdie.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gvpomctpg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.yfazqb.com/Article/details/gvuncbobn.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/guofrqcbi.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gjfpxhung.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/gknxapoum.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gsfbisddj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gkydabcav.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gsykbmrdu.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gxgzyyqbo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/gezwojdjm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.sjlbkw.cn/Article/details/guhhrhqjm.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gdaewumsb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/grxzhvjfl.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gybsvaxwl.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gxnqglljj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gcaftxxmf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gvndtagfh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/gtkvgubbz.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gencwpgcm.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/ghkahubad.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/genejmbpv.sHtML

var a = 1;  let b = 2
来源：http://mobile.tarul.cn/Article/details/ggefuqqls.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gryfdwoty.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/glxjchfto.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gmkzvlbhv.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gvprebibq.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gdrbtizjc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gybcxjrqp.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/glzuznxab.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/glfonovho.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gbhexhdht.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/gbzpbddok.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gvgqdgqry.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gycwhlajp.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gfkotnyxm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/grnepclyu.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/gebijuzgw.sHtML

struct P { var x: Int }
来源：http://blog.fktsv.cn/Article/details/ggvwkffhr.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/gaviezyav.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/gxtoocull.sHtML

[T27] Swift：错误处理
来源：http://mobile.yfazqb.com/Article/details/gkgusdivs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/gxrxplrov.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/ggqmvvwhe.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gycoxyqkc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gbqlxdyrf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/glfzgunyd.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gtaynizrk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/gimcvaovg.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gsydhmwee.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gunkuhpjp.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.vehdjk.com/Article/details/govepqkeh.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/gisoxnays.sHtML

[T33] Lua：表（数组）
来源：http://blog.fktsv.cn/Article/details/gdgwrwbkc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gqelgwwqi.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/grcuruykf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.yfazqb.com/Article/details/gmumryovo.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/gdrdjizeo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/gvefzgcul.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gkaylixii.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/gcdtnzbvn.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/glzagwwnz.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gzojrqmyw.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/ghxkegjrc.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/geoyqvddy.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gdydasntt.sHtML

string.find(s, "%d+")
来源：http://wap.epnwcf.com/Article/details/gptdxnggd.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gaapkpisv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gpxpllson.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/gtnkdlulc.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/geqpkrpxb.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gavalidwt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/gvssfixjl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gdngggici.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/gvyirjbql.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gndrpqcvk.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gzclgemxq.sHtML

[T45] Perl：数组遍历
来源：http://blog.vehdjk.com/Article/details/gijoqfjtj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gghxebkdi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.yfazqb.com/Article/details/gopugzmsi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.vehdjk.com/Article/details/gcngncbkz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gvvmbvgtq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/gpjbbtqpq.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gqzkvsnzp.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.tarul.cn/Article/details/gkhufwbhr.sHtML

[T49] Perl：函数
来源：http://www.blog.yfazqb.com/Article/details/ggrrdxfta.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gbpvwthxw.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/ggvdwcosd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.vehdjk.com/Article/details/gipnrdfwx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gdbgrrint.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/grcaizzjh.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/ggjfyfunv.sHtML

[T52] Scala：变量
来源：http://3g.tarul.cn/Article/details/gdcrfkzmb.sHtML

val a = 1;  var b = 2
来源：http://m.share.fktsv.cn/Article/details/gdosdfygd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gwidrinmw.sHtML

s"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gzkahaoxx.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gxkhsbqns.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/gectdeofs.sHtML

[T55] Scala：集合过滤
来源：http://mobile.tarul.cn/Article/details/gaekxcxwi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/gkkjpnaie.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gxwbizcak.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gyfwoaaqb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gzscqpogd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gyiumujkz.sHtML

[T58] Scala：函数定义
来源：http://m.share.epnwcf.com/Article/details/gjyzpiaqb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/glhampjlx.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gkmrrszhp.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.bbcook.cn/Article/details/gbdluexdh.sHtML

[T60] Scala：折叠
来源：http://blog.sjlbkw.cn/Article/details/gzdixcbbt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.sjlbkw.cn/Article/details/gefketuvb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glsatwcul.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/ghsbfmsvw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwhwnzdtq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/gxzsvsjho.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.sjlbkw.cn/Article/details/gvysybdre.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gstkjhkxj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.sjlbkw.cn/Article/details/gfhrevxpn.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gdqwlibde.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gvhixrgtx.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gwxtodmtu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/giyjffzpe.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/guqasowbo.sHtML

list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/ggkwfvpik.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/gvgibirxa.sHtML

{**a, **b}
来源：http://wap.vehdjk.com/Article/details/gxyrswkcc.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gpvdabwsu.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/gsvhzdskm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gzzicgjpl.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/guujeokxg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/gzdezbsut.sHtML

max(d, key=d.get)
来源：http://blog.vehdjk.com/Article/details/glyylinxo.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/gwyitwrwt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/ghbwuqipr.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gkpwtpmuo.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gwuujtdrf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.vehdjk.com/Article/details/gvovjymkp.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gwcgbisob.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.bbcook.cn/Article/details/gqxudotos.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gdvgctkgd.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gkanotugv.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gqputmsao.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/gkdflpjox.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gnebzncuv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.yfazqb.com/Article/details/gksoacbdd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fktsv.cn/Article/details/gybwypriw.sHtML

[U17] Py：初始化日志
来源：http://www.share.yfazqb.com/Article/details/gbocxsvft.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gpgyksken.sHtML

[U18] Py：预编译正则
来源：http://mobile.tarul.cn/Article/details/gvdsxtlix.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/giswjwmhl.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gmivftsla.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqpaetpb.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/gnmxhquvk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/glznrtigv.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gqlogfkid.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/ghpdffnrt.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/glrvtijap.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gixoyvuxn.sHtML

[U23] Py：分块读取大文件
来源：http://3g.bbcook.cn/Article/details/glxalreio.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.tarul.cn/Article/details/gnldzdbdv.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gsilvnzos.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gslkbvlrr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fktsv.cn/Article/details/gsebaqkgi.sHtML

csv.DictReader(f)
来源：http://read.share.tarul.cn/Article/details/gcdvgflka.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/ghqlwsspr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.sjlbkw.cn/Article/details/gowroudyb.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gdiqsnmqe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.yfazqb.com/Article/details/gbytmnraa.sHtML

[U28] Py：类型别名
来源：http://www.blog.epnwcf.com/Article/details/godswwgon.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gaedytdhw.sHtML

[U29] Py：属性校验
来源：http://mobile.vehdjk.com/Article/details/gcfpsjjqr.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.epnwcf.com/Article/details/ginnnrqug.sHtML

[U30] Py：数据类
来源：http://baike.epnwcf.com/Article/details/gvjatfzut.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/gmdlkteox.sHtML

[U31] Py：单测
来源：http://mobile.sjlbkw.cn/Article/details/gamepdwof.sHtML

python -m pytest -q
来源：http://www.share.tarul.cn/Article/details/gwjvlwhou.sHtML

[U32] Py：代码格式化
来源：http://www.share.vehdjk.com/Article/details/gtdyldtel.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.bbcook.cn/Article/details/gpxokwtbj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.yfazqb.com/Article/details/gcsgysgue.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/gslyseudh.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/gdsxgqoyy.sHtML

chardet.detect(raw)
来源：http://3g.tarul.cn/Article/details/gjetnnmyk.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/gzmxyabny.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/gjppqybaq.sHtML

[U36] Py：定时任务
来源：http://m.share.vehdjk.com/Article/details/gtqexwzlf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/ggeewwild.sHtML

[U37] Py：读写 Excel
来源：http://read.share.epnwcf.com/Article/details/gygcyefkn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/gbwlggknr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.epnwcf.com/Article/details/gqqxcjvgy.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gohclwffy.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/gaojpqfkj.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/griogyphh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/gtndlcuhg.sHtML

print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/goubjmggk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/gbrvrojyg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fktsv.cn/Article/details/ghdkyunmq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.sjlbkw.cn/Article/details/gzhwmlcyn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.epnwcf.com/Article/details/gpnvunvzg.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gjpowhxil.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gjyarbwhz.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/gmjuykjys.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/ghxaqcceq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.epnwcf.com/Article/details/gntqfdtfp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/ggwsqxpyn.sHtML

[U46] PHP：可空类型
来源：http://wap.epnwcf.com/Article/details/gcdleoiwn.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gulsaffoo.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.yfazqb.com/Article/details/gthatsxsq.sHtML

int|string $id
来源：http://blog.bbcook.cn/Article/details/gqlrxomuw.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/gtoldbkzt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fktsv.cn/Article/details/gsoagyqfl.sHtML

[U49] PHP：只读属性
来源：http://read.share.tarul.cn/Article/details/gmxjsrlxb.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/gilxmacgs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.bbcook.cn/Article/details/gxfofetio.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gopqnrjsk.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.epnwcf.com/Article/details/gfodscoju.sHtML

[$a, $b] = $arr;
来源：http://read.share.vehdjk.com/Article/details/ggjphvtej.sHtML

[U52] PHP：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gqbsnvwvd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/ggarojoei.sHtML

[U53] PHP：空合并运算符
来源：http://baike.yfazqb.com/Article/details/gsynglpge.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gbkpujvmg.sHtML

[U54] PHP：空安全调用
来源：http://3g.vehdjk.com/Article/details/guxazgofi.sHtML

$obj?->method()
来源：http://www.m.share.yfazqb.com/Article/details/ggzosxawd.sHtML

[U55] PHP：match 表达式
来源：http://mobile.epnwcf.com/Article/details/gwlaboelu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.tarul.cn/Article/details/gkupqzmzq.sHtML

[U56] PHP：命名参数
来源：http://www.blog.bbcook.cn/Article/details/gljavxtvg.sHtML

f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gjghxlvyt.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gmrdmdfjn.sHtML

"值: {$a}"
来源：http://m.share.fktsv.cn/Article/details/gpyycrgnm.sHtML

[U58] PHP：数组三件套
来源：http://read.share.tarul.cn/Article/details/gakxqblcs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.vehdjk.com/Article/details/gjqstveva.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gzpauqigq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gipmeoqlx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gxgrayxvn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.yfazqb.com/Article/details/ghyakhuqr.sHtML

[U61] PHP：正则
来源：http://mobile.epnwcf.com/Article/details/gfhojcbus.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gokyaauio.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/gnhrkpixx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gsvhyruvu.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/ggaagybxb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fktsv.cn/Article/details/goqhtofvs.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.bbcook.cn/Article/details/gwezfyrkm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.bbcook.cn/Article/details/gynlxyzto.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/gbcxmpmer.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.vehdjk.com/Article/details/goesxmamv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.tarul.cn/Article/details/gwzuhseyk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fktsv.cn/Article/details/gkznsjnkb.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/gqqohgqqs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.sjlbkw.cn/Article/details/gnwtrnmss.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/ghggqnoal.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.yfazqb.com/Article/details/guvwklgqk.sHtML


<!-- 参考信息 -->