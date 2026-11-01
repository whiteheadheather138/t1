代发 wailian999

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gexphjfcd.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/gomhxsuir.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gxdonsgoa.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/giedirwal.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/gjpvuhuee.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gnmrolsxf.sHtML

#endif
来源：http://wap.fktsv.cn/Article/details/gyqyepsbi.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gzzpwgbjk.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gpgbsmyds.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxwrocxhm.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/guqglytkh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gbwjnrvvc.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gbncyqfwu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gpeycxzhz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/ghyuqednw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gwashnscm.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gysvuiznz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gsbftyjhf.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gkyhssfnv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gyggddpfn.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gyaaqheyc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gbiyimbii.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gamslrlmd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/gekmhpbdl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gjzboktsu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/gonvtjfpk.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gaifwefec.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/ggicqocmq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gvftkuobw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/govqbgmje.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.vehdjk.com/Article/details/gqjsqyprt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/gksbwpvml.sHtML

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/gpbcdgyel.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.yfazqb.com/Article/details/gbcndkdvn.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/gwzedwiri.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gmfernhcm.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gojhtnyup.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/geaqdnmtf.sHtML

[S46] C++：函数模板
来源：http://3g.yfazqb.com/Article/details/gayethmpw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gxxxmopav.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gbtdphlvz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gsmxvpowa.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/grigtuhfo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.yfazqb.com/Article/details/gfmkjppsj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.yfazqb.com/Article/details/gtwlykkhp.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/gnuosvcqz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gyukszopq.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/glgydkzwz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gamuumhvx.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gmohmxtxc.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gqahzoboe.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gfyeogpng.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/guwzjrxmh.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gchdpwuam.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/grusegvbm.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gsqjwngua.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gudcwsloy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/grccnpghx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.tarul.cn/Article/details/gwzgromzu.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gjvznzdbi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gkuppvnye.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gwscusibk.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gcvngtyuj.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gpblqlfwo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gdqucdxsz.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/guirskdst.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gtwjxoxcu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gcltpmitj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/grcdhedkv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpgvyhamt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gmhnzdmwl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goygmmoss.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gfzzrczry.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gjbnvvilj.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gaoqihybn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gpuwgwwol.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gfocacswj.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gxbwtzsyz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gbxmdrtdw.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/gqagseare.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gvcxpasej.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gtzhiugsq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gcefnidkr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gpihseyhr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gxhuxxxhr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.yfazqb.com/Article/details/gvlplfcov.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gihrjdwtq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/ggyqbkabx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gtprtyxia.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gijdmzjvn.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gqmjwants.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.bbcook.cn/Article/details/gpdbkjmag.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/gwxppksvq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gwhcdbjhk.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gdciupjux.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/ghglsligb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/giwfsvseo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/gkfnvtmgd.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/gwrqvdunx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gnurukymv.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gnpmbqfwk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/grvejfppx.sHtML

[T16] Swift：Hello World
来源：http://3g.fktsv.cn/Article/details/gopcvfony.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gnidbtvhu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gyfuzjifd.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gqgopzimc.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gidnbiven.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gjedgtrhz.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/gnymysfld.sHtML

if let n = opt { print(n) }
来源：http://www.share.sjlbkw.cn/Article/details/gtxdwpkyw.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gbgsrftst.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/geugzcich.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gpntwkjmb.sHtML

for x in a { print(x) }
来源：http://read.share.bbcook.cn/Article/details/ghtyalsiw.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/gsatpdqku.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fktsv.cn/Article/details/gmvisgzaj.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gfixlggfk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/gvocyxnzd.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gflsepqlt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gqsiysyxf.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gxlbctoql.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gaxxhpmaz.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/gstjmvmbx.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.vehdjk.com/Article/details/gwnbnxsnt.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gcaazogap.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/goffgkyil.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gseijlekm.sHtML

enum Color { case red, green }
来源：http://www.share.tarul.cn/Article/details/gphguizwu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/gzeqsqnfv.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/ggcsfspfk.sHtML

[T30] Swift：协议
来源：http://m.share.yfazqb.com/Article/details/gentuvlph.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gwbmpinfi.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/grmygmvwt.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gzmftxycq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gyvtiowej.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gveezltbh.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.epnwcf.com/Article/details/gnhxdkvza.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gejhylbuw.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/geluskmdw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gmzcfjfwb.sHtML

[T35] Lua：字典表
来源：http://www.share.bbcook.cn/Article/details/grnrozqxb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/gvidazakc.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gfudxevzx.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gglgqknac.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/geossgetx.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/gweoiivip.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gjjfcwudx.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/gujfnvjvh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gqegvbbqp.sHtML

string.find(s, "%d+")
来源：http://3g.bbcook.cn/Article/details/gbremrftd.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gcvnyrhpz.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gxirxffbb.sHtML

[T41] Perl：Hello World
来源：http://read.share.epnwcf.com/Article/details/ghrertgob.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/ggukzgeue.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/geskfsbhx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gyurtaacg.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gwgwavmaw.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/gpkvnqyyo.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/gdtecbabw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gbcbjninc.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/gpftkuzns.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gjoemgbnv.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gftqmwxus.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gydlhlnfs.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/ghcfyvdct.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.sjlbkw.cn/Article/details/gnvcusqgs.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/gczoqaczo.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gezexyxmx.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/glcitjqxk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gilvejpyd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gijkixaoc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gzzyvrhje.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.yfazqb.com/Article/details/gbhltcbgk.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/gtwsvbxqy.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gytscbxxy.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gbzogdsdt.sHtML

val a = 1;  var b = 2
来源：http://blog.bbcook.cn/Article/details/gaagscdjm.sHtML

[T53] Scala：字符串插值
来源：http://baike.epnwcf.com/Article/details/gstcprots.sHtML

s"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gouqavneq.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/genwdlxzp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.tarul.cn/Article/details/guomdnuzt.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.yfazqb.com/Article/details/gsrwbvrfn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.epnwcf.com/Article/details/gqdxajdyo.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gjhzutiog.sHtML

case class User(name: String, age: Int)
来源：http://blog.bbcook.cn/Article/details/gjpzwxjqq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gyvbhfhrr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gfxvxotnl.sHtML

[T58] Scala：函数定义
来源：http://m.share.yfazqb.com/Article/details/gvupjkktd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.yfazqb.com/Article/details/gtemzhrpz.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gsgvxyyhe.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.vehdjk.com/Article/details/gvrajymil.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/gvqdudtdc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.bbcook.cn/Article/details/gcpbqrjll.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvufaopxk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gdxowmvct.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcuhvbzbh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.vehdjk.com/Article/details/ghgcchuds.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.sjlbkw.cn/Article/details/gzibhyleg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.bbcook.cn/Article/details/gdxmqkcek.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.bbcook.cn/Article/details/gkicsnxel.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.bbcook.cn/Article/details/glozyqjbh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuwchomd.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gevkghdrx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.sjlbkw.cn/Article/details/goyvykuov.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.tarul.cn/Article/details/gvajuosvq.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gbcjesduj.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gggnvtmmw.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gxdqlcvaw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/gwowabunu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.sjlbkw.cn/Article/details/gbpamcfju.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/gkjpkrzap.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/ggxrrunkw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.tarul.cn/Article/details/gvtvqaprv.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/gssukbiyj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.epnwcf.com/Article/details/gffsgggtv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.vehdjk.com/Article/details/gcxydqute.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gmhkexbzo.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/ggcmcssrv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gmoqlrjwt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/geoeipqdz.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gseqiumga.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/gsshlzdrf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/ghbcgrlqh.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gunvzrzth.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/gfycoyzbo.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gcohupzwr.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/gcryzlgik.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/grtkkurnk.sHtML

[U17] Py：初始化日志
来源：http://mobile.bbcook.cn/Article/details/gydkjadfi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gcbirzhbi.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/gdtkejtfk.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gzhlnsotu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/gqvqhoekc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.tarul.cn/Article/details/gbhwjwjtr.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/garbwrbju.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.sjlbkw.cn/Article/details/gbwnerxmi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gayfctvsn.sHtML

@contextlib.contextmanager
来源：http://wap.sjlbkw.cn/Article/details/gqsrliomp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrchnjxi.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gwchtfdyu.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/gojjzmtyx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/gpcrdjbkz.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gkjjsyawp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gibcpqpev.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/gbcaovfic.sHtML

csv.DictReader(f)
来源：http://www.m.share.epnwcf.com/Article/details/gyakidgol.sHtML

[U26] Py：并发下载
来源：http://3g.epnwcf.com/Article/details/ghppzkjte.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/guqhckwgr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.vehdjk.com/Article/details/gihvfzevy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fktsv.cn/Article/details/gypyladkz.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/glndmqjym.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gwtfnmrtm.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gmozpyeis.sHtML

@property 与 @x.setter 配合
来源：http://m.share.vehdjk.com/Article/details/gobwslait.sHtML

[U30] Py：数据类
来源：http://mobile.vehdjk.com/Article/details/gzafjwlnf.sHtML

@dataclass(slots=True)
来源：http://mobile.tarul.cn/Article/details/gmooiuekr.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gnzsysipn.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/gyojtjgxc.sHtML

[U32] Py：代码格式化
来源：http://www.blog.epnwcf.com/Article/details/gvsqckjsf.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/gtqymzned.sHtML

[U33] Py：打包发布
来源：http://read.share.tarul.cn/Article/details/gnyrsxtlz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gchbwpkvr.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/gdawpgzwf.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gcniwakgc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvpucjcw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gewnezqii.sHtML

[U36] Py：定时任务
来源：http://3g.fktsv.cn/Article/details/gkgvinhsd.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.yfazqb.com/Article/details/gulvtxpli.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/gtdxyerch.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/ggafgvrgv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fktsv.cn/Article/details/gkkzhoyqj.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/gwrbpjqux.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/glejhzcpu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/geyjrkvmb.sHtML

[U40] Py：打印到标准错误
来源：http://blog.bbcook.cn/Article/details/gkxqejlvb.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/grpuxhgeq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/gzdlicuiu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/gsybzkadj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fktsv.cn/Article/details/gahugkbfo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.tarul.cn/Article/details/grhzcgvjs.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fktsv.cn/Article/details/gxrwphfnc.sHtML

namespace App\Http;
来源：http://baike.vehdjk.com/Article/details/gerptjqqy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.vehdjk.com/Article/details/gchlfxihi.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gtctegsrw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/gxgmywpnx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gxdlxypvn.sHtML

[U46] PHP：可空类型
来源：http://3g.epnwcf.com/Article/details/gegvlyhzf.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gfzttrpqf.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gjrcfecri.sHtML

int|string $id
来源：http://www.blog.vehdjk.com/Article/details/gfysoksfo.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gtqgmhawz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/gqhjnfspi.sHtML

[U49] PHP：只读属性
来源：http://wap.fktsv.cn/Article/details/ghjhavpbe.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/girjjzfud.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.epnwcf.com/Article/details/giaqrofnr.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.tarul.cn/Article/details/gbsbmnaop.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gqfpjvurh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.bbcook.cn/Article/details/gxkkozrdh.sHtML

[U52] PHP：箭头函数
来源：http://wap.tarul.cn/Article/details/gajhfwdhc.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.sjlbkw.cn/Article/details/gyxmzsfle.sHtML


<!-- 参考信息 -->