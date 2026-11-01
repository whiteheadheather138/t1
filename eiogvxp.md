代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.vehdjk.com/Article/details/grwfspakj.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gibvnvwko.sHtML

memcpy(dst, src, n);
来源：http://www.blog.vehdjk.com/Article/details/gmmohhvcu.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/ggxhhfcee.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gvilaupou.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gyhodmbbt.sHtML

const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gwkinxtrn.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gmbvmwfxj.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gfroulopc.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gaiaceclc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/ghcsyieuc.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/grdbnnjzd.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/guqyypatw.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gambvrqwp.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/ggrifoivg.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gkwyuwgfy.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gelfttddj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsposmvr.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gwlhjssdc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gslwivvne.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gwoydjxif.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/grxfnitmq.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gcjkflxdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/gwdqnyyzi.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gkeeoeqpl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gbnbrrzdw.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gbelvpvtk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/ghxpkcjwr.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/ggbpdifrr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/guasvbccf.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gycabeocn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gayeydkrd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gvcnquhki.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/glsqqtozw.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gauzurlfs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/gjtzelgrl.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gfgkamdyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gezdcwhre.sHtML

[S42] C++：继承与虚函数
来源：http://wap.yfazqb.com/Article/details/gomwbeknc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gahocqhsm.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/gcxwzdfns.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/grviojtuv.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/ghytpshyp.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/gqtyyixoj.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gfrbupdmh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gploptqyb.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gvntgqftd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gnackjqoj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/gxbjsiocd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gexlpaqkg.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gunszkwch.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gctncbdab.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gserocbca.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gakdndzts.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gjeptbscx.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/ghufydytp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gnunbmkso.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gxbjfuplc.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gcqzuvull.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gagiqksoz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gfvyetzpc.sHtML

[S53] C++：移动语义
来源：http://www.share.vehdjk.com/Article/details/gznijxlcd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gxathyitx.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/glpbwvdbb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gcytxsynb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/givakvwwb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gucyleojg.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/gnqtwiaim.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/ghonchnrn.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gjqtxypgn.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gvmakkmlq.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/grlclyiok.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.bbcook.cn/Article/details/ghpgchxsn.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/grlruashl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gxycngcly.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gewhbssec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gxhypwkoi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcuhgqhog.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gdmkcwalh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gczszxuwl.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/gejxaarrs.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gwnxaebym.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gzmbnqywd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gjdxnovsh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/gwmzjcvup.sHtML

"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gcmhdwnxy.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gslnfieuc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/ghzpfyrso.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/geujktffd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gynqemqhc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/grfzdyewn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gvlylhpnh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gpqwkeonx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gnxyhaxik.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gocagiswh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gdmpxbbrk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gzbaypoos.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gmsidmigg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/gdtswxxbi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gcycgcgxy.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/ggljwzaui.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gxffbxfcz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/grqwpmmlm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gsfjhumdh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/gbrqmphev.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gppicehnd.sHtML

[T14] Kotlin：循环
来源：http://baike.fktsv.cn/Article/details/gztrwoxfa.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gwmyysvnk.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gqysepxhd.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gxclhfevy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gctzwvbhb.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gzaypvaau.sHtML

[T17] Swift：变量与常量
来源：http://3g.epnwcf.com/Article/details/gjptjwqwv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gzobmqrej.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gxuonoerc.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gvokucaun.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/ghjxjxfin.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gntsdnqqc.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/gfphfcild.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fktsv.cn/Article/details/gitjpqhpx.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/glhsdjijj.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/gtrksvevs.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gldflukig.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gbajrwyda.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxbufzfnn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/gmypagebt.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gkirmwfjc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gfjdtnrdo.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/gemuqcirp.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gxhvfypua.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gsozpwgde.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/gprxhzggs.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gwgvkuzyf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gpisjwlbd.sHtML

[T28] Swift：枚举
来源：http://baike.tarul.cn/Article/details/gvprllaeb.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/geslumxym.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/ghygokaer.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/glykktder.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/guuklpbym.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.bbcook.cn/Article/details/gphwocgvz.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/gtuyjedag.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gaswqoqns.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/gtjteymid.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gxdsxqhwr.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gmksyerau.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gdnwrptnb.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gjbcjlnir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/ghwemiryg.sHtML

[T35] Lua：字典表
来源：http://wap.yfazqb.com/Article/details/grgsxldrc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/gxawupnrk.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gvxjcknpp.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/gkitxaayz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gutjmlhbt.sHtML

"a" .. "b"
来源：http://mobile.fktsv.cn/Article/details/gnmapobqj.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gmanzlhau.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/guqmfcfng.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gcuujqggk.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gzpieykkq.sHtML

[T40] Lua：元表
来源：http://www.share.tarul.cn/Article/details/gyvbggztt.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.vehdjk.com/Article/details/gntyqigeo.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/gvalbpgej.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/ghylhlwcy.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gquxeffgv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gzllzftej.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/grckeiqyc.sHtML

"值: $a"
来源：http://wap.bbcook.cn/Article/details/graorpswq.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gtfvgftun.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gfbcztzqo.sHtML

[T45] Perl：数组遍历
来源：http://mobile.epnwcf.com/Article/details/gxvzkzpry.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/glyiysnis.sHtML

[T46] Perl：哈希操作
来源：http://baike.epnwcf.com/Article/details/gxzgypxqg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gqxdszuyw.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gmfliffja.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/glrfgnlsj.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gjexhssbk.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gfnzbfhlm.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/ghkxchpem.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gbkyznuec.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/giwoewfwq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.tarul.cn/Article/details/gysnmzoaq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gmqrkxrsk.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gmwscjgtu.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gwblchiew.sHtML

[T52] Scala：变量
来源：http://www.blog.tarul.cn/Article/details/googvraof.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gucjmnekf.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/ghkrhqdjp.sHtML

s"值: $b"
来源：http://baike.vehdjk.com/Article/details/ghmsahmvj.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gzuxzzfwp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.tarul.cn/Article/details/ggxrxaeen.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gymkzsixc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.vehdjk.com/Article/details/gyeoidbgg.sHtML

[T56] Scala：样例类
来源：http://mobile.fktsv.cn/Article/details/gehglcsnj.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gcbdudqre.sHtML

[T57] Scala：模式匹配
来源：http://3g.vehdjk.com/Article/details/gtebussrp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gnewxtjcr.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/grddzxcfn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.epnwcf.com/Article/details/ghbfcqadw.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/geqegrlxi.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/goystvcqb.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/gppxyonvo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/gtmbnwgwd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpsivndmh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gookepnlg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gilknqnjc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gtynazopm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gzlvwgmhb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.yfazqb.com/Article/details/gcokygnhw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gmcvedbtl.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.sjlbkw.cn/Article/details/girfpwpnu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/gnsfizkwf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fktsv.cn/Article/details/geqxhhsrn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gtlnxeamt.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gimibjpsu.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gwzjlvebl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/geatyfryo.sHtML

{**a, **b}
来源：http://3g.yfazqb.com/Article/details/gostqehui.sHtML

[U07] Py：反转字典键值
来源：http://3g.sjlbkw.cn/Article/details/gfcrkcwur.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/gubhoilzn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.yfazqb.com/Article/details/gcroygidy.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/gajxprjqc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/gkjcrvusk.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gjemeqggh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.tarul.cn/Article/details/gbuwuwlqw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gsbxxemmy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/ggaxbbgfg.sHtML

(x * 2 for x in arr)
来源：http://blog.bbcook.cn/Article/details/gpucwpztn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.epnwcf.com/Article/details/gvxvatudl.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/guwoqdbma.sHtML

[U13] Py：固定长度队列
来源：http://baike.vehdjk.com/Article/details/gqgrcssnx.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gnohwlylb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gnvhmxqck.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gxddqrvhj.sHtML

[U15] Py：高精度计时
来源：http://m.share.bbcook.cn/Article/details/gjexnjpuo.sHtML

t = time.perf_counter()
来源：http://wap.epnwcf.com/Article/details/gskuzuatl.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gjehgerly.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.tarul.cn/Article/details/gyhaxypom.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.vehdjk.com/Article/details/gttdosvoa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/glnpryrqw.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/gmrmjoohd.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gkuntgzyk.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/gmbkijhgs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gwfcwohih.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.tarul.cn/Article/details/gtpmkygdo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/gkklmogxv.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gqffcyzia.sHtML

@contextlib.contextmanager
来源：http://baike.vehdjk.com/Article/details/gvggqtgkr.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gphphhpsa.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/gchxabyye.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.yfazqb.com/Article/details/grlpywito.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/gzbwmhdms.sHtML

[U24] Py：路径操作
来源：http://blog.epnwcf.com/Article/details/gwvintrer.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gtlwkqhhv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fktsv.cn/Article/details/gkgrqxbzb.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/gvriohfon.sHtML

[U26] Py：并发下载
来源：http://wap.vehdjk.com/Article/details/gxavfpzrn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/gqzqmqtlt.sHtML

[U27] Py：异步 HTTP
来源：http://3g.yfazqb.com/Article/details/geytyidyz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gmxhnfiwp.sHtML

[U28] Py：类型别名
来源：http://blog.tarul.cn/Article/details/gbsbkgasn.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gzflijqtc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fktsv.cn/Article/details/gdevtawao.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gzuowqxqr.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/gtzzqlqay.sHtML

@dataclass(slots=True)
来源：http://read.share.yfazqb.com/Article/details/gdmwxfdrg.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/gawwzxnth.sHtML

python -m pytest -q
来源：http://3g.fktsv.cn/Article/details/gclbihseh.sHtML

[U32] Py：代码格式化
来源：http://mobile.epnwcf.com/Article/details/gnejxlcqt.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gjzxjxgme.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gansnbqsz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gmtbkrllf.sHtML

[U34] Py：判断编码
来源：http://m.share.fktsv.cn/Article/details/gnnrbdvvn.sHtML

chardet.detect(raw)
来源：http://wap.bbcook.cn/Article/details/goaunbxax.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/gcbbdmevk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.epnwcf.com/Article/details/gyjzbroqs.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/geblaxzac.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gxkctigal.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gonfybqym.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/gvypoyjij.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/guechxqta.sHtML

Path(__file__).resolve().parent
来源：http://m.share.bbcook.cn/Article/details/grpegqulm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.yfazqb.com/Article/details/gaswreqih.sHtML

sys.stdout.isatty()
来源：http://blog.tarul.cn/Article/details/gtkbxviks.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/ghjxsgosf.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gjhrnyxig.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gbkiksdrj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.yfazqb.com/Article/details/gqzrqdwwc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.tarul.cn/Article/details/gepcjwviy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.vehdjk.com/Article/details/gxlikdfpd.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/gliaeafcn.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/gpgvhkkkq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.epnwcf.com/Article/details/gfoozbnox.sHtML

declare(strict_types=1);
来源：http://3g.yfazqb.com/Article/details/gglhkysrd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/gnffjpiov.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/ggmbobnkr.sHtML

[U46] PHP：可空类型
来源：http://m.share.fktsv.cn/Article/details/gduuqcbhq.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gbwneeoal.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/gbqdpcdsn.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/gyejcgydc.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gtgxsezjw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fktsv.cn/Article/details/gkeusskek.sHtML


<!-- 参考信息 -->