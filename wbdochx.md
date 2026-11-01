代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/ggdyymzcd.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gwnugvpkj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/gjbwcrmri.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/giruaqscb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gcmvhatyp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gaalsjabw.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gktpawlbu.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gbeohzllq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/gqetjjhmr.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gopsvtsgz.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gkmlblezr.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/ggzaqmelq.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gxkpkptpy.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/glyausvdi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/ghcdvortk.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gvwxbmmov.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gftucqoqs.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/gvibeocwp.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gzbqkbwsw.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gsfiietxk.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gguzrlcap.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gavuhrhnc.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gxlkgskzz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gekemfncl.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gysjhfhhk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/ggfqgzuyo.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gupbphjnd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/goufkmium.sHtML

[S35] C++：map
来源：http://blog.vehdjk.com/Article/details/gzpmwcnwi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gcfzckcps.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gsugyfdfk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gqzzjmsuu.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/gtculsfjv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gfeiyequv.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/gbgnyqhwt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gkvpdqwqq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gwlpjgzkw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/grjljowum.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gnopvrqxe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gxbdgurdc.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gxsrwfrpt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gjvhcakvg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gxronrnuy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.yfazqb.com/Article/details/giefkrgtu.sHtML

[S43] C++：智能指针
来源：http://mobile.tarul.cn/Article/details/gjyhiimbx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gwavujbsv.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/gvuyrsjbe.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/gbdwwvpqt.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gvohdcnqr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/gbmyhodfv.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gplxvktwp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/gudpvaqxh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/gvtxxshat.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gpzvdutum.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gwclpukui.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gayedpckv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gmuyttzxl.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gcfichppf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/goqsejlqe.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gmuafbkef.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gpbgujicw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gspfxwxhv.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/godoyajkd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/ggpernaqs.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/gwvrvjgku.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gfmtjtozu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.vehdjk.com/Article/details/goelrmkgr.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gzhlmsuvq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gxafskbll.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gpuoubtgj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gkalxijgs.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gouprscnq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gjinklrfj.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gejawtuia.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gwlnbmscy.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gtyvcfpny.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.epnwcf.com/Article/details/ggsieghtm.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gjgsoerun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/ggpbdagxq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gogearwim.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gznwcikqt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnvhomlfq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gvcjssnjd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcqbhfbbj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gprhbvjxr.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gckyqqmfu.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gitqrakmt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/grgaeotjb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gjahfctbe.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gisgsuoxs.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gaeatwauk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.bbcook.cn/Article/details/gtkbtroox.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.tarul.cn/Article/details/gttcpkeuz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gsluwpoqg.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gmwoxinrn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gbvfdbsux.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gsljbpdqp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gbcqpcyaq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gjmasplzf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gpiuylhji.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gdofqfvse.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/grcftjika.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gswtsrzdz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gxcmwfoxo.sHtML

[T11] Kotlin：协程
来源：http://blog.fktsv.cn/Article/details/gfeanmwao.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gxxodxkai.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gqsspibcq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gixntluan.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gvndoctae.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gutptcnfc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/glfboxlpw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gbabpjyzp.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/ghyuymree.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gifghfvnt.sHtML

[T16] Swift：Hello World
来源：http://m.share.yfazqb.com/Article/details/gjankjnmw.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gibcsnvqm.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gkcpmmlje.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gqxuyryoi.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/guzfvfslr.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/ggsebcevg.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gnyamahhi.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/goczowiba.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gtjvhwrdn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gdveqdovr.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gyetmvjum.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gkeevoqfn.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/guhpswgau.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/grvekndvn.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gnvzhwkvl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gwepgewcl.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gxtztmlqq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gyvuqnxls.sHtML

[T25] Swift：结构体
来源：http://www.m.share.sjlbkw.cn/Article/details/gviundrfs.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/gnpxtxgdr.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gblaaempg.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gshpngvvn.sHtML

[T27] Swift：错误处理
来源：http://m.share.bbcook.cn/Article/details/gsmqpplzq.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/gjevvlmia.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gssiqtgvl.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gvafduhbo.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gonhgesnf.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gqhkmcuos.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/gpadpopal.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.vehdjk.com/Article/details/glhpivzpc.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/grblisqii.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gyibbnwcc.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/gpewfruyy.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/ghlgkeuvd.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.sjlbkw.cn/Article/details/gktkximng.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/gvglkggzc.sHtML

[T34] Lua：遍历表
来源：http://read.share.tarul.cn/Article/details/gwhklomgb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.yfazqb.com/Article/details/ghztarvfw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/ghvvclifp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gdkbdumcm.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/ggnxguzrw.sHtML

function add(a, b) return a + b end
来源：http://www.blog.tarul.cn/Article/details/gquxlogte.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/gidsmszld.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/gdbzjvfpl.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/gpsfewdrb.sHtML

if x > 0 then print("正") end
来源：http://baike.epnwcf.com/Article/details/gsdykrzub.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/grkhqncge.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gmqzlrmqn.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/grsaaqhwd.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fktsv.cn/Article/details/gakodnyup.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gvhicezrs.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gvavnkdpx.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gjprcrlzk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/geeouhsug.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gtxmbsojg.sHtML

"值: $a"
来源：http://www.share.sjlbkw.cn/Article/details/gmssrzmxm.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gmynxnjyd.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.epnwcf.com/Article/details/gfdbyztdj.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/galuxadbu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.vehdjk.com/Article/details/gkshfiwgl.sHtML

[T46] Perl：哈希操作
来源：http://wap.fktsv.cn/Article/details/gojhjowkb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/govnltdfz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gjkspvhxf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.bbcook.cn/Article/details/ggzjmbvpb.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/gzbzhobfo.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gbmmblomy.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/gwowfuilf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gphgfrwsa.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/glhbvhgun.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.bbcook.cn/Article/details/ghyfsuibk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gnssdmnsi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gxjxwpcpg.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gtnnxzaty.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/ggslxgjeq.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gwmmzehzg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.tarul.cn/Article/details/gjzbjtsrf.sHtML

s"值: $b"
来源：http://baike.bbcook.cn/Article/details/gfdilcgcc.sHtML

[T54] Scala：集合映射
来源：http://mobile.bbcook.cn/Article/details/gsiznavgt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gyzbzifwg.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gabqhhexd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gjuyooqgt.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gmevcqjox.sHtML

case class User(name: String, age: Int)
来源：http://mobile.yfazqb.com/Article/details/gpdksgiju.sHtML

[T57] Scala：模式匹配
来源：http://read.share.yfazqb.com/Article/details/glxwatgqs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gzeqotrzn.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fktsv.cn/Article/details/gpkdtojwd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gynvkcrtr.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gbsxcxwdo.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gxplrejbc.sHtML

[T60] Scala：折叠
来源：http://www.blog.sjlbkw.cn/Article/details/gepwuwdmt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/gtzabract.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghtaoyrxi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gyniqbkjc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/goggflhwa.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/gafczapuk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.bbcook.cn/Article/details/gbbijrzvj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.bbcook.cn/Article/details/gitdbmznd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fktsv.cn/Article/details/gdkuewfuq.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gmcivtunz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.vehdjk.com/Article/details/gjidcphpe.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gjdiwlbqp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gzijjclun.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gmrjhczbj.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gnnemsymx.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gqinfcgku.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/gytlrhmne.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gfqlbhznn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/geaaluzft.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gjzguvftd.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gwdebevkk.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/ghtlurjys.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gdqlgbbeh.sHtML

[U10] Py：按值排序字典
来源：http://www.share.epnwcf.com/Article/details/gytjxhfyc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.yfazqb.com/Article/details/gwowfbmqk.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gyozrdmij.sHtML

(x * 2 for x in arr)
来源：http://baike.bbcook.cn/Article/details/glodfwdwo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.tarul.cn/Article/details/gcdizrtkh.sHtML

Counter(arr).most_common(3)
来源：http://baike.tarul.cn/Article/details/gikprzgge.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/ganpvfdiq.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gypfxicwf.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fktsv.cn/Article/details/ggaeftart.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/ggvpozgnv.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gmznonxxm.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/gwwkewsqd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/gdlckjawe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.yfazqb.com/Article/details/gjsctrntg.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gbiuzmvok.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gmfauzzoq.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/ghudmlolx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/gsfarqqop.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/gpiedprfc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fktsv.cn/Article/details/gfuecehwg.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gurptfvty.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.bbcook.cn/Article/details/gjizljspc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.epnwcf.com/Article/details/gyvanhtvu.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gnakqzjpf.sHtML

[U22] Py：矩阵转置
来源：http://wap.bbcook.cn/Article/details/ghqazzrzw.sHtML

list(zip(*m))
来源：http://read.share.vehdjk.com/Article/details/ggwlztgun.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.bbcook.cn/Article/details/gixhgfioe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gjqrjjcjm.sHtML

[U24] Py：路径操作
来源：http://m.share.vehdjk.com/Article/details/gvruotgbe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gabdipcyl.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/gtfiuhchg.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gsrsdeotd.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gvsgqyjfd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gzghrlipa.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.sjlbkw.cn/Article/details/gppjpynhj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gjiixundc.sHtML

[U28] Py：类型别名
来源：http://baike.yfazqb.com/Article/details/gqeqyxwix.sHtML

UserId = int
来源：http://wap.sjlbkw.cn/Article/details/gnjnoxvvi.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/gpjsktcxx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gcdwqzrnh.sHtML

[U30] Py：数据类
来源：http://mobile.yfazqb.com/Article/details/glrwperwa.sHtML

@dataclass(slots=True)
来源：http://www.share.fktsv.cn/Article/details/gqtllisqy.sHtML

[U31] Py：单测
来源：http://baike.vehdjk.com/Article/details/grgausrwp.sHtML

python -m pytest -q
来源：http://m.share.yfazqb.com/Article/details/gayoqfapx.sHtML

[U32] Py：代码格式化
来源：http://wap.epnwcf.com/Article/details/godfhnjyn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.vehdjk.com/Article/details/gfkvmsnnr.sHtML

[U33] Py：打包发布
来源：http://wap.fktsv.cn/Article/details/gismsafsj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/ganctbcfs.sHtML

[U34] Py：判断编码
来源：http://www.share.bbcook.cn/Article/details/gdidzptic.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/gkvkcfsov.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/gaoozdxgo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/gozbkpxta.sHtML

[U36] Py：定时任务
来源：http://wap.fktsv.cn/Article/details/gftgpbmtk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gljxjdhgh.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.epnwcf.com/Article/details/gpxjsnrom.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/grlbbcxxq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.vehdjk.com/Article/details/gtbssftzj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.tarul.cn/Article/details/gifwlnnqu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/gjkkebuaf.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/gtazvnmso.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.epnwcf.com/Article/details/goflqitdg.sHtML

print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gmulqlrtu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.vehdjk.com/Article/details/gzraqyzmz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.tarul.cn/Article/details/gufuuqxzx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gqtnnsmwo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.epnwcf.com/Article/details/grucagwqd.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gboxgpnuu.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gigkpudtv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.vehdjk.com/Article/details/gjzufepkn.sHtML

declare(strict_types=1);
来源：http://wap.epnwcf.com/Article/details/gkgoyrwoi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gedqouyzx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gnelesxnc.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.tarul.cn/Article/details/gfmqclxgv.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gwolbkksn.sHtML


<!-- 参考信息 -->