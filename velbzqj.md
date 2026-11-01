代发 wailian999

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/gbearxhfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gomnmfdsk.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gwjwerosk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gzmdmcmdy.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/gberxxint.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gjcgjncov.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gyvpqqoil.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/ghbgvrmox.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gzuuvzkuy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gvcrrsdlc.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gsatbdffa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gxpkliyiw.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gdceelvfz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/gcxqkvyye.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/gzgpujrgl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/gxffglfmi.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/ghicosyfu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/goxpgcpis.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gdfqgtegk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/giflupbyn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gpqpcaimd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gdmnfqwlb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/gtkziyjdv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/gylakrxro.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gywiiauru.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/geupnqzul.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gomuoosgj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/ghptkzppv.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gbsdknuoo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/govgaltwu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gbfutwero.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/goebwkaat.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gfekiykcx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/giftzrhvn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gzzihwlrj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gdwubvxxb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gkrsmcpvz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gdbinvdto.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/ggehuzelu.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gtamocxrm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gtbiagnmy.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gtmmnoxjk.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/geryralal.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gqpcfxtkq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/goxofqckg.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gpgcwhdzc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/gviboshzq.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gfmebsqcs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gcatsczvq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gpqfkjlin.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gxhnlpfnp.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gaatxdson.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gudgpiebh.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gnimllnpg.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gvuxxezpa.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gpnoalqar.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gtbbcezeq.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/glrekkend.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/guhvyrqgb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gvpftydjj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gygmybzji.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/groskczaf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/ggqakufsj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtimwsmhr.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/germogojt.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/giokfaskf.sHtML

[T02] Kotlin：变量
来源：http://mobile.bbcook.cn/Article/details/gzbeszprz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gixmupfan.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/gpvrnnemi.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gxvqkknsx.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gighilvap.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gydufyatt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gkevwzjdb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/ghocmzoqe.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/glmugkuxo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fktsv.cn/Article/details/gyibanerj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gsuotcqsu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.vehdjk.com/Article/details/gnznsgdot.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gknmcfgyr.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.epnwcf.com/Article/details/gvtopqjud.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/gueawqgbp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gfidpsrtv.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gqgksepqj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gmlabxihe.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/geagtrvjs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gkbnwlojv.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gumhfsecl.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gedmtajog.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gxertgpde.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/goxbrpxab.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gijyvzoyp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gfnusfsgo.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gkdqcbwbg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gnuliuujg.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gudkmkrkg.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gyvfxrlzq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gxrjqihvs.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gnuiowtou.sHtML

[T18] Swift：字符串插值
来源：http://3g.bbcook.cn/Article/details/gvubpmogt.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/guoshgtck.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gcjxoaqjw.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/gppnjvhqt.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgwiskjw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gjcvcztln.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/gcupxwwkx.sHtML

for x in a { print(x) }
来源：http://blog.vehdjk.com/Article/details/gggxkplym.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gfhhprvfw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gcubehdva.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/ggbkhazio.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/giacuviif.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/gyjuloifk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gixdejlah.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/gkybzgvug.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/gpchysefp.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/gljapmpax.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gkwjihzdp.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gdvwklztt.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fktsv.cn/Article/details/giqkoqomy.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/gsgqgcety.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gyumvskjp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gffhrhgjx.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gotxaebtl.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gtzxhwtdx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/gxkayqzde.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/grroslvhk.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gbzhltlqk.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gptdcnyxy.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/gcxgxwvrs.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gitqyssxd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gpsncyfzy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/ggnskslog.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/gkravzbtk.sHtML

[T35] Lua：字典表
来源：http://wap.sjlbkw.cn/Article/details/gphadkveq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/grggdunvu.sHtML

[T36] Lua：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gppwgrlsv.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/gounblmad.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/gqcxgdpml.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gfgjukpdo.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gpblgrgob.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.tarul.cn/Article/details/gyuhpynrd.sHtML

[T39] Lua：模式匹配
来源：http://blog.vehdjk.com/Article/details/guyzvdkss.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gfxbnryct.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/glqbbxzmw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/gpkmmhytg.sHtML

[T41] Perl：Hello World
来源：http://3g.fktsv.cn/Article/details/gwirpoheh.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/godfkmmyq.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gexuqeuqy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.bbcook.cn/Article/details/gqnxxaxmm.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gqhkdpnma.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/gghkpfsfc.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/gjnyqulqh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.vehdjk.com/Article/details/glfbyyixa.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.yfazqb.com/Article/details/gablnnvln.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/goruxqilk.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gtyeiajbz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gwkyrjgcn.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/grrjijkum.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.bbcook.cn/Article/details/gnilhjxxp.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/gxdsrbsij.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.tarul.cn/Article/details/gfsueslpy.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gyojzyomb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gfpvgfrdd.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/grklfygfs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.bbcook.cn/Article/details/gjhppfivm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gjjsxcnlr.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/gwsuvggxt.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/ggshjskcc.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gqmcytpfx.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/gdoxbtwuw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gnaehcymu.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/guneinyed.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gbhmmpxao.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.yfazqb.com/Article/details/gcdyzatsa.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/grznfurmt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/grotsmqle.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gzlqvmvfc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gifbfbnmj.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gxdodstyk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gldlgnyrj.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gwsqxwfxv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/gcekkidga.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/graxqqhzm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gbwhbwkna.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gsixjlfsp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.sjlbkw.cn/Article/details/gazynspmv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grvcwhpua.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gkrgqznnp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnblxshzu.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/gznphekdg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.vehdjk.com/Article/details/grfwtrxpt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gzyzdaqbe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/ggshpoogs.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/gxfrotxel.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/gffjygyzv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gxstdfosn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.sjlbkw.cn/Article/details/gxbsmttau.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gtudxeidd.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gonlblrdt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.tarul.cn/Article/details/gfglosojs.sHtML

{**a, **b}
来源：http://www.share.fktsv.cn/Article/details/gbohfwvku.sHtML

[U07] Py：反转字典键值
来源：http://baike.yfazqb.com/Article/details/godwevlei.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/gwgpnpmgz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/gfuuokshv.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gkiqkjeek.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.epnwcf.com/Article/details/gaqoyomrp.sHtML

max(d, key=d.get)
来源：http://baike.yfazqb.com/Article/details/gttdxupdz.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gdetgrxgv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.epnwcf.com/Article/details/gatooxlgu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.tarul.cn/Article/details/gonnvtroa.sHtML

(x * 2 for x in arr)
来源：http://m.share.bbcook.cn/Article/details/gjxadknsj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.bbcook.cn/Article/details/gfofxpsdw.sHtML

Counter(arr).most_common(3)
来源：http://3g.vehdjk.com/Article/details/gyqqxwteh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gunfssapo.sHtML

deque(maxlen=10)
来源：http://blog.tarul.cn/Article/details/gwbkhdalw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/ganlwrenq.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gbdgjjpna.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gguxqfvmc.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gvujufprq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gmlcilhvw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.tarul.cn/Article/details/gyvkxqpsv.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/gvpccfrgh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/growseslw.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gkzupuaxy.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/ggupcyrax.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fktsv.cn/Article/details/gtxbujwqb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.vehdjk.com/Article/details/ggizutfte.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/gvdcfpelg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.tarul.cn/Article/details/gvvlhuttq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/gjlldfgqx.sHtML

@contextlib.contextmanager
来源：http://3g.epnwcf.com/Article/details/gcxvkkhol.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/gnaodlcil.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gxqlurjka.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gylkscidf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.bbcook.cn/Article/details/gpbksuluf.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/glhpwyicj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gfxcaomjg.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gtztmnujw.sHtML

csv.DictReader(f)
来源：http://3g.sjlbkw.cn/Article/details/gfoqlugvx.sHtML

[U26] Py：并发下载
来源：http://blog.vehdjk.com/Article/details/gffgmmumc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/ghotepjcu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.epnwcf.com/Article/details/grxurbuqr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.tarul.cn/Article/details/grqhjhpoh.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/gkvkavwla.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gexviusxi.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gdomlsvpt.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.yfazqb.com/Article/details/gmgcyenaw.sHtML

[U30] Py：数据类
来源：http://read.share.vehdjk.com/Article/details/gnvfomdvv.sHtML

@dataclass(slots=True)
来源：http://www.blog.bbcook.cn/Article/details/gqqckxqhc.sHtML

[U31] Py：单测
来源：http://3g.vehdjk.com/Article/details/gpzsdafkq.sHtML

python -m pytest -q
来源：http://read.share.fktsv.cn/Article/details/gggwngfsv.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gvjhqoech.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.bbcook.cn/Article/details/gqaxzyezk.sHtML

[U33] Py：打包发布
来源：http://m.share.vehdjk.com/Article/details/gnjdiyngb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.vehdjk.com/Article/details/gmbjvcsat.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/gfuszzpld.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gueqsqewa.sHtML

[U35] Py：发送邮件
来源：http://read.share.fktsv.cn/Article/details/gxfpzmlqp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.tarul.cn/Article/details/goxucrkmn.sHtML

[U36] Py：定时任务
来源：http://baike.tarul.cn/Article/details/grebkeiun.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gyyaglsqw.sHtML

[U37] Py：读写 Excel
来源：http://baike.yfazqb.com/Article/details/ggoaxjcej.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.sjlbkw.cn/Article/details/goalrsbee.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/gvsnujbqu.sHtML

Path(__file__).resolve().parent
来源：http://baike.epnwcf.com/Article/details/gdvpzokkl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/giruaywzk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrdhiuds.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gbhmlotqi.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gynwnzzkc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gralyxxjb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.vehdjk.com/Article/details/gsalrvcwr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.epnwcf.com/Article/details/gneqdziqv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gslmrjwbr.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.tarul.cn/Article/details/gcnstyfza.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gwlecspgc.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdlehjri.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/grlecgzxu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.vehdjk.com/Article/details/gjygsexny.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gzxdgaqvu.sHtML

[U46] PHP：可空类型
来源：http://m.share.tarul.cn/Article/details/gwbcgkqel.sHtML

?string $name = null
来源：http://read.share.fktsv.cn/Article/details/gbeuiyfoc.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gsokillss.sHtML

int|string $id
来源：http://baike.vehdjk.com/Article/details/gvvuixpdr.sHtML

[U48] PHP：纯枚举
来源：http://3g.vehdjk.com/Article/details/gqbjpiula.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/ggthirnpb.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gqdlkzmht.sHtML

public readonly string $name
来源：http://www.m.share.epnwcf.com/Article/details/gzuurtdsh.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gykygjbqo.sHtML

public function __construct(private int $id) {}
来源：http://mobile.tarul.cn/Article/details/grlfuxyge.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/gtnphamrc.sHtML

[$a, $b] = $arr;
来源：http://mobile.epnwcf.com/Article/details/gtywxezfy.sHtML

[U52] PHP：箭头函数
来源：http://blog.tarul.cn/Article/details/gixrwqmab.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.vehdjk.com/Article/details/gzeiuuqrr.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/gxrqnvfvn.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.yfazqb.com/Article/details/gvnzunvxz.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/gxxuhrgpw.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/giyllubiz.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gxurimfhj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.vehdjk.com/Article/details/gafcakacb.sHtML

[U56] PHP：命名参数
来源：http://baike.sjlbkw.cn/Article/details/gxgrnbbhg.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/ghdgyvfzr.sHtML


<!-- 参考信息 -->