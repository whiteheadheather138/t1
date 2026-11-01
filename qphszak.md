代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.epnwcf.com/Article/details/gnkcyucqm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gjclkmzmn.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gclxtyvxz.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gewewogvr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gesbnamec.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gklmnqhdm.sHtML

const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gdtparioj.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gpfcnsowj.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gwigegtyz.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gpxsnktxg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gyhdelexw.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gqlqgnvby.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/ggfnwczdt.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/glfwvcjsp.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gkgszpxhl.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gkdxhbzxk.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gpaoousuq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gwylefnad.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gcmpoyman.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gnjtcpdav.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gfdhuopes.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gcejefrxj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/gtfsamsxq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gxialxwpo.sHtML

[S35] C++：map
来源：http://baike.tarul.cn/Article/details/gbyrleydb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/geebigxuf.sHtML

[S36] C++：unordered_map
来源：http://www.share.vehdjk.com/Article/details/gkgvnkztx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gfjkkmwus.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/ggxzxoovo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/giqoroxij.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gjnrhfjfp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gchsxzvxw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gwcujysrx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/gzqpyfkhm.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gsopztazj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gmlfpnpqw.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/grtuhbpvy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gblwwlxiq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.yfazqb.com/Article/details/gzhxejium.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/garovqonc.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gnczwvavr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gcwhxlnfe.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/ganlmawom.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/grdjkpcxf.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gomcbokmf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gdclyyoux.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/ghlxxgvjt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/getmnoqbx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/giejfbcxe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.yfazqb.com/Article/details/ghibgvmfl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gweogaiyw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gvlnbfvlz.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gxnccnzjr.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gslfppngt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.tarul.cn/Article/details/giwdhubkx.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/grublfddw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gywgoqatu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/glrviyqla.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gemsknrjd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gpjxpikfw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gdvfjbhek.sHtML

[S53] C++：移动语义
来源：http://www.blog.sjlbkw.cn/Article/details/gkhypdtpq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gqikhuydr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gaxqeoytl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/goosouait.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/ggshwlikt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gufyvgizr.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/ghgefaniu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.vehdjk.com/Article/details/gderpcrtc.sHtML

[S57] C++：编译期常量
来源：http://mobile.bbcook.cn/Article/details/gwjrteypd.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gnbfrvxbc.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gvfiscwgi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/gxpfzpbfj.sHtML

[S59] C++：静态断言
来源：http://www.blog.vehdjk.com/Article/details/gfrfoefbo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/ganeehdjz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtzzajho.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gonlfkntu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghqastmoa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gvpogzwpi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guypsfqdg.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gmlolbhcz.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gxxpgswak.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/gqhifbszz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/grndtirzn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/ghgiyujoz.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/gjyqngfnw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/ghnqympfp.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/gyyirmkjr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gxirdikxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gjszyfzmy.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gnlushdum.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gizgvohal.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gzptuotvc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gxmythpdn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/goouelpiw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/gszurdrvp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gyrjmpvzg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gvzwgnbeo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/gigvpmbqr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gujvcfrqs.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/geiagwkhm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gdcgmqytr.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gfkmimcxh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/guazglayh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gncladiba.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/grvrbfmhy.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gkeacqzry.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/grnqunpaz.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gowmlgerw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gzscdafpz.sHtML

[T16] Swift：Hello World
来源：http://wap.epnwcf.com/Article/details/grktvrvvc.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gddwusizr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/ggwomgqrk.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/ggixjhohn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gsejcaefq.sHtML

"值: \(b)"
来源：http://mobile.tarul.cn/Article/details/gwydcbwgb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gwfttfjge.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/gemcseytm.sHtML

[T20] Swift：数组操作
来源：http://blog.yfazqb.com/Article/details/gpzbcadvn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.epnwcf.com/Article/details/gftpehnsw.sHtML

[T21] Swift：遍历
来源：http://3g.fktsv.cn/Article/details/gmwsvuhio.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gwymxrttk.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gisemvycb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gyqonjjnz.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gtbtbeqlz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gdwbnmarv.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/ghdecalyd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gubscyicu.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/gfkjddwov.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gwjpzlhbl.sHtML

[T26] Swift：类与重写
来源：http://wap.fktsv.cn/Article/details/gwidkxsnw.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gjsoztkbz.sHtML

[T27] Swift：错误处理
来源：http://wap.vehdjk.com/Article/details/gsdptfjcz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsztfkfik.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gqetnjgkd.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gvtyifzoy.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/guqsxkzso.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gcbngvhxz.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/grrltrxdw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.sjlbkw.cn/Article/details/gliceuemz.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/gjjqpdval.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gqpexlkdb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.vehdjk.com/Article/details/gwemlvkrk.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gyqcofbzx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fktsv.cn/Article/details/guleheqpx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gbuholppi.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/gabrczwgl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/gvqdfxyno.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gicykcfhi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.tarul.cn/Article/details/gexaozial.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/glnxckcjw.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gfqsvkefo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gllesqkht.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gfvefwosk.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/glsvenstp.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gjleodfyx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.tarul.cn/Article/details/gppetlcxo.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/gxtqgckbu.sHtML

[T40] Lua：元表
来源：http://www.blog.bbcook.cn/Article/details/gwywddzvp.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gvhlpgwmt.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gbwjdjoyj.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gvlewlxix.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gsmziqjyj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/gitimmjvl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gipbozmxz.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gvdekmqgo.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gezguzjzb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/goshsroms.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gjicxquvu.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/gepotjjmz.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gkfwzjfue.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gtpmvcgzg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gjfrxsrjp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/gzsqdrvxn.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/gqrtjwcub.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gbsggyzyg.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gckibbdby.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gmvjuwvid.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gpeiqhaiy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gmdutozri.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gkswvjckd.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/geulexkxl.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gtctskwij.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/gbkpcjxxp.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/geilolarb.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/godrwlqnn.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/gbsntwpba.sHtML

[T54] Scala：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gkxatbpzb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gaabqlrtw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/gldcncagv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/goebkkrfs.sHtML

[T56] Scala：样例类
来源：http://www.blog.yfazqb.com/Article/details/garvqyzli.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/grutvwrik.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gwdcnrbio.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.yfazqb.com/Article/details/gdnoxlvfx.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gnrqnkyxk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gajldtejp.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/gxsfxneoz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gjzizfagk.sHtML

[T60] Scala：折叠
来源：http://www.share.bbcook.cn/Article/details/gfkxkwkjg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.yfazqb.com/Article/details/gxyrnktpp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxizgutcn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gtfcsubep.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grdtxkdgh.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/godmesgvh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.yfazqb.com/Article/details/gklqgjdxl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.epnwcf.com/Article/details/ggkephtld.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.vehdjk.com/Article/details/gpfijymft.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/gyyuayybd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gekpwfnfp.sHtML

[U04] Py：变量调试打印
来源：http://wap.bbcook.cn/Article/details/geaayxabm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gdwzpyagd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/glexvsezx.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gykqycduq.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gwxkazhzx.sHtML

{**a, **b}
来源：http://www.blog.tarul.cn/Article/details/gxpfbsqxi.sHtML

[U07] Py：反转字典键值
来源：http://mobile.bbcook.cn/Article/details/gqkbirihv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/gdafxytvw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.sjlbkw.cn/Article/details/gjosdpovu.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/ggfbvcoft.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/ggyvkghdl.sHtML

max(d, key=d.get)
来源：http://www.blog.vehdjk.com/Article/details/geepjwvoy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gnwkajuml.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/gjfvnafrz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/gdnznkfeq.sHtML

(x * 2 for x in arr)
来源：http://wap.epnwcf.com/Article/details/gzxobtcnd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/gbpfppiqo.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gdhbbvzib.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/gueyofwmq.sHtML

deque(maxlen=10)
来源：http://www.share.yfazqb.com/Article/details/ginhfpmpi.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.tarul.cn/Article/details/gaxazktcg.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gupgkfsui.sHtML

[U15] Py：高精度计时
来源：http://www.blog.tarul.cn/Article/details/gmxqjbseo.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/grstawcdq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gxxvtzjuv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fktsv.cn/Article/details/gepljfvev.sHtML

[U17] Py：初始化日志
来源：http://www.blog.bbcook.cn/Article/details/ggfxbjtaw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.vehdjk.com/Article/details/gjjcievvu.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gyfimluxt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/geeltqzpm.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.epnwcf.com/Article/details/gtsnnqeke.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/ghhsfpfuj.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gzbhllyfc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.vehdjk.com/Article/details/gbcprdnmq.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/gkolzmvoy.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/gvoulmxpn.sHtML

[U22] Py：矩阵转置
来源：http://3g.yfazqb.com/Article/details/gtboodiuc.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/gxxfwymdd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fktsv.cn/Article/details/gwzeaphzz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/gxiiczzqs.sHtML

[U24] Py：路径操作
来源：http://www.blog.sjlbkw.cn/Article/details/glyjkhari.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gcuoyofgg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.bbcook.cn/Article/details/gxjdllwaz.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gniuebtyr.sHtML

[U26] Py：并发下载
来源：http://wap.sjlbkw.cn/Article/details/gpqvtcjpx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/gdfkdztpf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gjcocqbkq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/goksddidf.sHtML

[U28] Py：类型别名
来源：http://3g.fktsv.cn/Article/details/gzzpqgzkr.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/grdnnvqkx.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gsefezwts.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.epnwcf.com/Article/details/gokckghmp.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gpbcxdkrf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/gigrmyhlo.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gczcvorqx.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/geabppcgz.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/gyunafnfk.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.sjlbkw.cn/Article/details/gyazkmpul.sHtML

[U33] Py：打包发布
来源：http://m.share.epnwcf.com/Article/details/gcbgrlwuz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/ghlfrpxpw.sHtML

[U34] Py：判断编码
来源：http://read.share.tarul.cn/Article/details/gltwpozvp.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gwfnfehld.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/gpdgvcbys.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.vehdjk.com/Article/details/gyttlzpde.sHtML

[U36] Py：定时任务
来源：http://m.share.epnwcf.com/Article/details/ghupexevv.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.tarul.cn/Article/details/gxzyvznnj.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/gyoqwdnxx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.epnwcf.com/Article/details/gzhkhosvk.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gwcomvcrv.sHtML

Path(__file__).resolve().parent
来源：http://www.share.epnwcf.com/Article/details/gsclfjzzi.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/gzvaprpmq.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gfgtquzio.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fktsv.cn/Article/details/ghoptwlfl.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gwtzmdhlx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.epnwcf.com/Article/details/gdqmaezda.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/gnhkjdwty.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.vehdjk.com/Article/details/guwfdjxkq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gjfcpsvum.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.tarul.cn/Article/details/gdbgqgpwz.sHtML

namespace App\Http;
来源：http://www.share.bbcook.cn/Article/details/gociasyhd.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/gdrnoievn.sHtML

declare(strict_types=1);
来源：http://www.blog.epnwcf.com/Article/details/gilcewfjx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gzjuogaut.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/goiccveim.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/glmzdzuqo.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gjmiuhpws.sHtML

[U47] PHP：联合类型
来源：http://baike.sjlbkw.cn/Article/details/gqmnmqqgg.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gqhivcrfm.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/gcxqicctb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.yfazqb.com/Article/details/geheigctb.sHtML


<!-- 参考信息 -->