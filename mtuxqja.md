代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gudmjtvqh.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/grphrjphr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gkztomjxx.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/ggpktuhbs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gqgqznhff.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gljwzgsdd.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/ggywpiriw.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gbpoecawp.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/goiaayolx.sHtML

[S27] C：定义常量
来源：http://baike.fktsv.cn/Article/details/grbtzgqhw.sHtML

const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gosbhnrny.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/garejhljy.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gvddemllr.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gjwqztnjq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gurvldwjr.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gtsflrwhk.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/grmwsxxpn.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gctevtzew.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/gzlyyljra.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gzgcwzamp.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gzzugqmka.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gzbtjsdls.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gbfxpgoyl.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gbuwauzno.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/gmqvtpcbs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gycjdnjqq.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gwodogqqf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gtmbxxgpw.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gcsfxxull.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gvswraxcq.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/goorugbhr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyikynfyv.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gkdtihzzw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gaxfdpvrx.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/ghzsklikv.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gelcxxuby.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/goecgousk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/gnwhlthbe.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/ggqyqpokz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gzbzhvktm.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gvdjriona.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gvxxvrdqz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.tarul.cn/Article/details/ggwudkbnn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gduptwjpp.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/gipuvwnzz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/goskiqavh.sHtML

[S44] C++：引用传参
来源：http://www.share.yfazqb.com/Article/details/gnsrkedfc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gkroddxfh.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gyzmshvfq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/goqbfdcpm.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gxxhjcfsw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gzycyzezf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/glkebrdlr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gaqulaoos.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gpzbkdzdl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.tarul.cn/Article/details/gslhpojhf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fktsv.cn/Article/details/gmuiaoziz.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/ghmlkoauc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/griskoyvs.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gccmkmgoh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/gakdbncfp.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gryilczed.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/gksnncboi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/giynmwqph.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/grqhgswau.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gwygiascu.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/ghbcrsyfh.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gkzkqsmfm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.tarul.cn/Article/details/gnufsplca.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/gkyfdnpfb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/geoaopmyx.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gebufkmgp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gaeulxeku.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/grqmdcqxs.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/guaxwgefz.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gorofimcm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gcfiwmhux.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/gqnwzheuf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gnksddlpm.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gwvwyydgh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gvpzyffbl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcvxybffi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/goxjrkovb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkzquhddb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gdcugqxyo.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gfojusual.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gcaxhwwci.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gdcukmuky.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.sjlbkw.cn/Article/details/guetmzqun.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gxfolaxxw.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gitqcpyhx.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/ghrwxunvz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gojkhkyor.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gfyrpnzvz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/gfqggaqdd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gsxpmuuyp.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gfoehyuhx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gjckaprsm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gnzzpnfmj.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.vehdjk.com/Article/details/gmxgsoluo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.vehdjk.com/Article/details/goengxlsa.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gxqhldjea.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gocdfjcuu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gaxlozpzu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/glyagtaxy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gknqlzmqv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gluduqlcr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gfhyiyhtm.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/gpmpuzpxu.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gkyidicyt.sHtML

[T14] Kotlin：循环
来源：http://wap.yfazqb.com/Article/details/gjqbzdjky.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gzgmjyrgb.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gufnsinlh.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gfbhzammk.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gclbamkyb.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrcgcfev.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gyxyoqiyt.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gtmylhehw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gdgearrge.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gmwelhmdd.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/grlyfrnox.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/gmbgnwdbu.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/goiuzftke.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gphqdchex.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gvtwzbslv.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/gmmtbjmho.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/gjvhtllwr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.bbcook.cn/Article/details/gzmllxxrh.sHtML

[T23] Swift：函数
来源：http://3g.epnwcf.com/Article/details/grdmumtjz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gvpalfdao.sHtML

[T24] Swift：闭包
来源：http://read.share.sjlbkw.cn/Article/details/gqvwiqykx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gqowonqar.sHtML

[T25] Swift：结构体
来源：http://blog.sjlbkw.cn/Article/details/gbqwkujja.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gjptdujaw.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/grwwgmuwr.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gudndpjqx.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/gyzhlnqlr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.epnwcf.com/Article/details/glyemgyym.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gzkayhysq.sHtML

enum Color { case red, green }
来源：http://www.share.yfazqb.com/Article/details/gzseoblvg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.bbcook.cn/Article/details/gkyziobov.sHtML

guard let x = opt else { return }
来源：http://3g.yfazqb.com/Article/details/gwmssmhsh.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/gmhfpsrlp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/geeqzivyd.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/guljjwcgd.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gwyzddees.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gwxuwxhgh.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gmhzdcbin.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/glfjwyaif.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/gsbjsfzlz.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/gfgciwuze.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gzrobhbmp.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/gkfllftyw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.epnwcf.com/Article/details/gotsvpmyc.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gfoqulqmt.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/gufzobeqa.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gdobkekxk.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/gwguifyui.sHtML

[T38] Lua：条件
来源：http://mobile.epnwcf.com/Article/details/gwltwgfox.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gddhdjxdv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/ggeiomupu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/gqvjtrbmr.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/gwcnkljix.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fktsv.cn/Article/details/gnystvssd.sHtML

[T41] Perl：Hello World
来源：http://wap.tarul.cn/Article/details/gglmmhism.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/geizdeelq.sHtML

[T42] Perl：变量类型
来源：http://3g.yfazqb.com/Article/details/gygosoyht.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gttklortx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gzkyxwgku.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/gpvypjcea.sHtML

[T44] Perl：条件
来源：http://blog.epnwcf.com/Article/details/gaqfuopwn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.sjlbkw.cn/Article/details/gfhylvnpo.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gmatovump.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.bbcook.cn/Article/details/gomnyehpz.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gwqbqwodx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gfhvrjgju.sHtML

[T47] Perl：正则捕获
来源：http://www.share.yfazqb.com/Article/details/gjexswbto.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.epnwcf.com/Article/details/gptluqymx.sHtML

[T48] Perl：正则替换
来源：http://read.share.epnwcf.com/Article/details/gkmwlpknt.sHtML

$s =~ s/old/new/g;
来源：http://baike.vehdjk.com/Article/details/goxunfrob.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gflenwnio.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gqyrzzyuy.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gwpaavpny.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/gvoyrrhsg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.bbcook.cn/Article/details/gvnoyislm.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gnmxisayw.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gwyqgcguw.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gakomahwz.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gpcfzgpvc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gmohjgfrr.sHtML

s"值: $b"
来源：http://blog.epnwcf.com/Article/details/gmbmeeycx.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gsmycdcpv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.epnwcf.com/Article/details/gvsuxvcee.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gltadfwgo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gtcgcjpbd.sHtML

[T56] Scala：样例类
来源：http://3g.tarul.cn/Article/details/gaseocbxw.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gxmofdnut.sHtML

[T57] Scala：模式匹配
来源：http://3g.tarul.cn/Article/details/gfaqvnbrh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gipcehagd.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/gkzpkggyt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gjxnqhxpn.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/grfobxwqv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fktsv.cn/Article/details/ggqoytelu.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/glmbolnlx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.sjlbkw.cn/Article/details/gdamxqwoz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwqjarypx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gnaqkkdlu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/guvzhtrwa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fktsv.cn/Article/details/gyzwradxy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.sjlbkw.cn/Article/details/gmuafcrxk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/ggxldzgpt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gazsapcks.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.vehdjk.com/Article/details/ghrkfmkpt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gkmhmqcig.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.epnwcf.com/Article/details/gnjdbmzks.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gubcubjpk.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/gotuaahqc.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gzooepwch.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/glrtvuoen.sHtML

{**a, **b}
来源：http://www.share.fktsv.cn/Article/details/gzxvlmlea.sHtML

[U07] Py：反转字典键值
来源：http://3g.yfazqb.com/Article/details/guzprhqwh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gibckdtlt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gfxrgpcsx.sHtML

[y for x in nested for y in x]
来源：http://blog.fktsv.cn/Article/details/gyfqwjzuu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.sjlbkw.cn/Article/details/gbqgnqxik.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/goczaqgnk.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gvbfrqstb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gdnwyddcv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.epnwcf.com/Article/details/gxgmolvkb.sHtML

(x * 2 for x in arr)
来源：http://wap.yfazqb.com/Article/details/gnrckqrqt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gnwingsmg.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gahrrjdoq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/goetavdon.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gyffzwpbe.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gswqcbvyg.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/gzfpepjqh.sHtML

[U15] Py：高精度计时
来源：http://www.share.yfazqb.com/Article/details/goccocmot.sHtML

t = time.perf_counter()
来源：http://3g.fktsv.cn/Article/details/gdnavqjyn.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/gpugplnwz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gpefbsoeo.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gkncznzlm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/gachbavja.sHtML

[U18] Py：预编译正则
来源：http://blog.yfazqb.com/Article/details/guxyssyzz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gxfuvhzqg.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/gkovmmkiu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gbmzduyml.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcqvifdq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.epnwcf.com/Article/details/gwzlvrqdq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/ghclkgxtr.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gbwnrfkoy.sHtML

[U22] Py：矩阵转置
来源：http://blog.epnwcf.com/Article/details/gyxbqgrix.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/gpoqppins.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/gcrrihjpy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/goaujuwmv.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gpwbyihtc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gtdyodgyg.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.tarul.cn/Article/details/godritpim.sHtML

csv.DictReader(f)
来源：http://www.share.bbcook.cn/Article/details/glosoipmv.sHtML

[U26] Py：并发下载
来源：http://blog.epnwcf.com/Article/details/gwkbpxgpb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.vehdjk.com/Article/details/gfjkiauej.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/ggiollwxc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.bbcook.cn/Article/details/gczptnllc.sHtML

[U28] Py：类型别名
来源：http://mobile.tarul.cn/Article/details/gnoujmolb.sHtML

UserId = int
来源：http://m.share.sjlbkw.cn/Article/details/gtyabycpd.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/gqtsudqxp.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gbvpsqmfn.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/geehansox.sHtML

@dataclass(slots=True)
来源：http://baike.epnwcf.com/Article/details/goowdpdkp.sHtML

[U31] Py：单测
来源：http://www.m.share.sjlbkw.cn/Article/details/gefvahvup.sHtML

python -m pytest -q
来源：http://baike.yfazqb.com/Article/details/gxsdgthiw.sHtML

[U32] Py：代码格式化
来源：http://read.share.fktsv.cn/Article/details/gtpyjekfn.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gpehdvxab.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/gtyvklqii.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gwmvasosn.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/gehmkplij.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/gzusntygz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.tarul.cn/Article/details/ggdlhoeeq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.tarul.cn/Article/details/gnttwfoft.sHtML

[U36] Py：定时任务
来源：http://mobile.bbcook.cn/Article/details/gjczrjkwv.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fktsv.cn/Article/details/guoxpdpqu.sHtML

[U37] Py：读写 Excel
来源：http://blog.epnwcf.com/Article/details/gyeclummr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/gphmmdaux.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.tarul.cn/Article/details/ggjkzqacd.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.sjlbkw.cn/Article/details/guvdrjmbt.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/gzfycemhd.sHtML

sys.stdout.isatty()
来源：http://3g.bbcook.cn/Article/details/gpwtfzbbc.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fktsv.cn/Article/details/gzhdmtmbe.sHtML

print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gbakybdzw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.tarul.cn/Article/details/grfoabzmh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/grwmhlwye.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.yfazqb.com/Article/details/gjrwizcrb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/gfvzqxvtt.sHtML

[U43] PHP：声明命名空间
来源：http://blog.yfazqb.com/Article/details/gddzkstrx.sHtML

namespace App\Http;
来源：http://www.m.share.vehdjk.com/Article/details/gzqoulnpp.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gldsajadp.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/gxlmqmizt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.vehdjk.com/Article/details/gckfwqpvp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gzkcctpos.sHtML

[U46] PHP：可空类型
来源：http://read.share.vehdjk.com/Article/details/gvwcdpdjj.sHtML

?string $name = null
来源：http://baike.vehdjk.com/Article/details/gomxhlpjb.sHtML


<!-- 参考信息 -->