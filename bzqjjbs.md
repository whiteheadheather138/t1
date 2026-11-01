代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/geqavpubq.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/glvsfwtod.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gvsfmdspj.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gcvwwcmtu.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/gkxoqpmkc.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/geazwvhbl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gkkepouaz.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gzztgvbyc.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gfcxsfzfz.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gqwjvqyrz.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/goktgjejd.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/giqrnaowg.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/ghqcznwod.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/glqkhpnjk.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gamstkxle.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gmbxagxjy.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gnyxqdfly.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gwcllsuoh.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/ghhluqaqk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/ghuppzgcc.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gsibzsato.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gxhqxxvxc.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/grenvqpwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gnzxvmvnh.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/grxnvjldc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gcrzfbfsb.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gxpjsvvks.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gxhtbbqva.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gummoofrz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gkhbtreoy.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gvfrahhxv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gnqqhwitu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fktsv.cn/Article/details/gkritejcd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gknkvcbxi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gkrmwdzmi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gchevvgnk.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gknzyebtd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gkqtedsdm.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gxksprlxv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.tarul.cn/Article/details/gdjqnopki.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gvhuarbee.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gngyokepy.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gbraxtcdd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gbjgvcwyj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/ghfqrrdxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gvuekgtsf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gylknhukc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvnopbcv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/givtssvxa.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/gfktcrlsf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gbqyzyoig.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gkopliuwg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gqalgnein.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gbjaewsqh.sHtML

static_cast<double>(a) / b
来源：http://3g.vehdjk.com/Article/details/gzerpkumj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gfxlldnvk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gwsokcupa.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvujpxeo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.tarul.cn/Article/details/gufigajna.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gajeoicvb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/geevevdpk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gtyzjzoov.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.bbcook.cn/Article/details/gpnejrkrt.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/gvsltfjry.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gqrkxmnno.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/gycreylno.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gthfpwdyc.sHtML

[S58] C++：命名空间
来源：http://baike.epnwcf.com/Article/details/gomhkgacu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/ghuhmywuc.sHtML

[S59] C++：静态断言
来源：http://3g.sjlbkw.cn/Article/details/gmijcjzox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gqgwsdapw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxgnzpav.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gwmeqmyte.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkgdzvfrs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/guevkptqn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqcvieprf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gtxrtongh.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gsvtobrow.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/ggfxbewin.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gfiukxhbf.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/gbbltmubm.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gledtfygv.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gkphuwnwh.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gvqcmkcps.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.sjlbkw.cn/Article/details/guaynwolr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gulcuyrch.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/giaauyoaq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gysxgpvvl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gwmjutngv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gkzlyrpgt.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gogfwgbak.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/gkqzrvdlw.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gerkxjnct.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/gqnliehkn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/giikvtaah.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gdpcmipaq.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/gquaidhfe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/guwhjrqvp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/glrrhbyhw.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gscekcqjf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gqignhfmn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.epnwcf.com/Article/details/ggtxomyjc.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/gzoofbbxz.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gchoydebd.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gtejgpleb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/gtnzhoirm.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gxmdmenhh.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gupyhwjhl.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/gbakmjyhk.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gyslumazw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gmeotpreg.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gasmlhbez.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gmnfepiug.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/gfvquwbbs.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gjnfzqklr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gykssyjtc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.epnwcf.com/Article/details/gbroczgri.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/glwtiyzpg.sHtML

[T22] Swift：字典
来源：http://www.m.share.vehdjk.com/Article/details/goumotyis.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gbklskoer.sHtML

[T23] Swift：函数
来源：http://baike.yfazqb.com/Article/details/gjnyncdye.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/gvzcodktz.sHtML

[T24] Swift：闭包
来源：http://m.share.bbcook.cn/Article/details/gkqlregst.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gvdujquso.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gfakotaeh.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gieljuiqm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.epnwcf.com/Article/details/gcdfmgwbv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gtnatybrw.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gauxtmlra.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gzbhqnyzg.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gdzldxreu.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gkdlcbgil.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/gnxanixfj.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/gpytfmyre.sHtML

[T30] Swift：协议
来源：http://m.share.yfazqb.com/Article/details/goxbvbdfm.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/ggtpkbacx.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gedklsvrd.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gtudfvacy.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gocicjleh.sHtML

local a = 1
来源：http://www.share.epnwcf.com/Article/details/gzwqkskth.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/gqgweywti.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.yfazqb.com/Article/details/gvleqgmrz.sHtML

[T34] Lua：遍历表
来源：http://baike.bbcook.cn/Article/details/gblpojvdg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.sjlbkw.cn/Article/details/gadlfcgbw.sHtML

[T35] Lua：字典表
来源：http://mobile.sjlbkw.cn/Article/details/gtmfpsspp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gluqqklwr.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/grbxmurns.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gvbckllfi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gdooyayft.sHtML

"a" .. "b"
来源：http://www.share.epnwcf.com/Article/details/gpunsuhhk.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvuxjqro.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.tarul.cn/Article/details/guuytdjdf.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/ghhzbndap.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gizrjayfz.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/gigoluwpt.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/goqhdrcwq.sHtML

[T41] Perl：Hello World
来源：http://m.share.bbcook.cn/Article/details/gmjygeorn.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gvksjbxsu.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gxngswqik.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gwfigakut.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/ghmegegfj.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gmphcaxre.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/gczjjnlnk.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/gcmdgzqcu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gjiglqlrj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsmlijbv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gfwrhctee.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/ghjvtnxhb.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gvleuybmx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fktsv.cn/Article/details/ghsbsrvje.sHtML

[T48] Perl：正则替换
来源：http://3g.yfazqb.com/Article/details/gfcjrkykp.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gylvfhvyk.sHtML

[T49] Perl：函数
来源：http://www.blog.bbcook.cn/Article/details/gdqganonv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gxsvmzthn.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gtqblmlyg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.yfazqb.com/Article/details/glruuvlzd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.epnwcf.com/Article/details/glzmmhakc.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/glkgfnsqm.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gzaafrnyi.sHtML

[T52] Scala：变量
来源：http://blog.epnwcf.com/Article/details/gemhlyzjf.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gersyvwxd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gleijcupg.sHtML

s"值: $b"
来源：http://baike.fktsv.cn/Article/details/ggwlgezzx.sHtML

[T54] Scala：集合映射
来源：http://baike.vehdjk.com/Article/details/guiehrypt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.epnwcf.com/Article/details/giqfvsnyu.sHtML

[T55] Scala：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gphphvzjh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fktsv.cn/Article/details/gqfpxjpox.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/guvtksqxk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.bbcook.cn/Article/details/gpyrjmcjh.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gboyltmlh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gnaypjghi.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/goybzskes.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.vehdjk.com/Article/details/gwrhdoobw.sHtML

[T59] Scala：循环
来源：http://m.share.vehdjk.com/Article/details/gxshrtkcd.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/gazwjkyiq.sHtML

[T60] Scala：折叠
来源：http://3g.fktsv.cn/Article/details/gebxrwazw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/gwskowjsa.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqnjmthah.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gbaxjbjiy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gumkxaoif.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/ghkugcoii.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gunkeefpw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.tarul.cn/Article/details/grnejgkta.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.yfazqb.com/Article/details/gumazjpwv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/glujjrwth.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.sjlbkw.cn/Article/details/gpebookgk.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/giapakzyy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gixnmasrg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gcpzvoqet.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gdrlvglmh.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/gkdgbrjgk.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gettsomoq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gdndarycl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.bbcook.cn/Article/details/gvmolmrpp.sHtML

[U08] Py：展平二维列表
来源：http://m.share.epnwcf.com/Article/details/gobaevwtu.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gcckswxke.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/gqgrmifcc.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/gceiayagp.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fktsv.cn/Article/details/gmeaufxri.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.vehdjk.com/Article/details/goaxtyeeq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.sjlbkw.cn/Article/details/gxrmmjreb.sHtML

(x * 2 for x in arr)
来源：http://read.share.epnwcf.com/Article/details/gpvewrafd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gthhzitga.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gsfrddoiv.sHtML

[U13] Py：固定长度队列
来源：http://wap.epnwcf.com/Article/details/gutudxfxj.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gezeohdbx.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gboipvjgm.sHtML

defaultdict(list)
来源：http://m.share.yfazqb.com/Article/details/gqcacepqn.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/glsmajxzl.sHtML

t = time.perf_counter()
来源：http://baike.sjlbkw.cn/Article/details/gimuljxrr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/gobxghehp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.bbcook.cn/Article/details/gaapacasy.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/grwvhrvcn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/glikqflvo.sHtML

[U18] Py：预编译正则
来源：http://www.share.fktsv.cn/Article/details/gajxjocnj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gwnelfvzk.sHtML

[U19] Py：正则替换带回调
来源：http://wap.vehdjk.com/Article/details/gbdmuvpkr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/gizzrovmw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.vehdjk.com/Article/details/gajcimrwh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gqgrhmbvy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.bbcook.cn/Article/details/gbwckplaa.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gythmkfar.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/gqgcayscn.sHtML

list(zip(*m))
来源：http://3g.fktsv.cn/Article/details/giyoytlro.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/gkhqqukvl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.epnwcf.com/Article/details/gewppwkcw.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gcsagmxqk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gmlyjguus.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.epnwcf.com/Article/details/gtoeviomm.sHtML

csv.DictReader(f)
来源：http://mobile.fktsv.cn/Article/details/gqykloqrf.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/gomgqncsl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.epnwcf.com/Article/details/gexqprqgt.sHtML

[U27] Py：异步 HTTP
来源：http://3g.tarul.cn/Article/details/gxyrsidqh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/grxuzdssg.sHtML

[U28] Py：类型别名
来源：http://wap.sjlbkw.cn/Article/details/gdbznwfll.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gzdwpcuxv.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/gebxcggvm.sHtML

@property 与 @x.setter 配合
来源：http://baike.bbcook.cn/Article/details/gtfbhmaia.sHtML

[U30] Py：数据类
来源：http://mobile.tarul.cn/Article/details/gkplaaavu.sHtML

@dataclass(slots=True)
来源：http://www.m.share.yfazqb.com/Article/details/gplgvjwxm.sHtML

[U31] Py：单测
来源：http://3g.sjlbkw.cn/Article/details/gjpcflhsa.sHtML

python -m pytest -q
来源：http://3g.bbcook.cn/Article/details/ggnbuakpw.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gtebwlfvk.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.vehdjk.com/Article/details/gimxlewyz.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/gsrybncsr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.bbcook.cn/Article/details/gjsjelhnw.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/ghotepdnp.sHtML

chardet.detect(raw)
来源：http://blog.epnwcf.com/Article/details/goltqbrgs.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/gpjpinbsu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.sjlbkw.cn/Article/details/gqecphfrd.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/ggsoddygl.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.vehdjk.com/Article/details/gulhfypik.sHtML

[U37] Py：读写 Excel
来源：http://wap.sjlbkw.cn/Article/details/gcmzduqjs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.vehdjk.com/Article/details/gwnzuyjzl.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/gqdzclcft.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gnhkrsbcj.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.sjlbkw.cn/Article/details/gecxqtmnc.sHtML

sys.stdout.isatty()
来源：http://www.share.fktsv.cn/Article/details/ggweampui.sHtML

[U40] Py：打印到标准错误
来源：http://blog.vehdjk.com/Article/details/gpmmtcujw.sHtML

print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gkruzfigj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.yfazqb.com/Article/details/gmyfpcpoz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.bbcook.cn/Article/details/gwfawkfpc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gbkrdrlrw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.yfazqb.com/Article/details/gwzpktxpf.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gmmfdrycx.sHtML

namespace App\Http;
来源：http://m.share.yfazqb.com/Article/details/ghjfvjpyj.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fktsv.cn/Article/details/gdglzmvqy.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxegipzdz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.bbcook.cn/Article/details/gwwywmlut.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gdelzipof.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gquqsohgs.sHtML

?string $name = null
来源：http://blog.vehdjk.com/Article/details/gybixoxoc.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gragkzudy.sHtML

int|string $id
来源：http://baike.yfazqb.com/Article/details/gecmkdybq.sHtML

[U48] PHP：纯枚举
来源：http://baike.yfazqb.com/Article/details/gzbodvsyx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.tarul.cn/Article/details/gpbelmwij.sHtML

[U49] PHP：只读属性
来源：http://baike.bbcook.cn/Article/details/gjqfcojuy.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/grcyyxwcu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/glwihwpzp.sHtML

public function __construct(private int $id) {}
来源：http://blog.fktsv.cn/Article/details/gukjabtkk.sHtML


<!-- 参考信息 -->