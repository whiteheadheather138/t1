代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.tarul.cn/Article/details/gppcngxxa.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gwjasoswk.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gnthuhpyw.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gcvbcmvyx.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gphllwfdw.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/grpvnmqsl.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gnslvuhrm.sHtML

[S28] C：静态变量
来源：http://mobile.tarul.cn/Article/details/gvmyztuqh.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/gdhjnojcx.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gnftdslsz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gzdluluts.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gpzimmrdm.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/grgewbdcn.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gdxclsbza.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gvmixmzuu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gdocquxny.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gvyhsjcck.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/gjcwwxlfm.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gkusinttg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gcurbtkqf.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/gydcsyrqr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gqehjcfzv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/grpoidtho.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/ginqvhzvv.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gqqvfhvhi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/geqduutfk.sHtML

[S36] C++：unordered_map
来源：http://read.share.vehdjk.com/Article/details/gaocmrfig.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gwqlfbloq.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gvzjxosuc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/ggekdwyll.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gfrvffnmh.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gsnvzvcvy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/ghirvfdyg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/gvmgwdyzc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gyyukwszn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.vehdjk.com/Article/details/gwykyuczo.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/gvlyztfsc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gycvnqcoh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gluwtjbtd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gzjzozehe.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gdujvsxey.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gcqxfaasp.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/ghgpnuluj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gzuqhqhhx.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/goqlvwkxe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gsodwvsta.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gyoyowvxp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gqbjwqfzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gxymfghoo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/ghevpulqn.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gxeoohfvs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/gvhgfzztn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gvzwkbvth.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/gpywvsqaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gxcofjrgm.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gkizcguwi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/grqgncdtp.sHtML

[S51] C++：显式类型转换
来源：http://www.share.vehdjk.com/Article/details/gbawscrbi.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gbnbowwdc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gkcpylvcw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gmyuwrggq.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gbwgpnizg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/ggewmvjzl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuseufmd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.vehdjk.com/Article/details/gsndasbfp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gcuiazcxu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/genmpmxwe.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gdvrmuyfd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/ghnvmciyj.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/gcxsohkln.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gwhqndahd.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gmqfbvoeg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gkslbddfc.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gunbmhnli.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gmbicyokb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/glucyzcbn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/ggiwfyhhk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtwrcorch.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/gxxkzwmhh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/goowuwcbf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/grtsfkkmw.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gtuhcimyq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/gqsctqwvk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gcuznnnje.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/ggryrquuc.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gkyfptymt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.yfazqb.com/Article/details/gnghgbhtk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gefiwznrd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gtzbyqiof.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.bbcook.cn/Article/details/gftzwwpnc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/glgsvslvl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gctgjtahm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/grxsgchqu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gqeuyexnd.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gyvbjlhmp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/grduxpyoo.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gfbxsthgx.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gincpmjut.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gamaeznjl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gjxvnimvj.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gcuwvaect.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/ggcjseeja.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gsypmemkd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gyjcwjves.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.epnwcf.com/Article/details/ggahcdoda.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/ghrmhfuhy.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/goztygbts.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/guysbbhhq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/guvdgxqim.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gnacfcruv.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gsjsyrzyu.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gaejjfjkf.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gayornsky.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/gspyrmaap.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gsoiijhpk.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/gudqrfpij.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/gwuzudszz.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gwgdlbezv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.bbcook.cn/Article/details/gfytspmzg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/gipyzpxmp.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gcjcbkaed.sHtML

for x in a { print(x) }
来源：http://mobile.yfazqb.com/Article/details/gmjthvyeb.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gbwxqsvdj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/ghsumnuut.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/gblvdulel.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gkbjrruwk.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gkuvwmeck.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/ghgxnrlvd.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gjndiudhl.sHtML

struct P { var x: Int }
来源：http://www.m.share.fktsv.cn/Article/details/guswikmul.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gcigmxnzf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gxtphopzh.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gspfwcdxl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gobgrphdo.sHtML

[T28] Swift：枚举
来源：http://blog.yfazqb.com/Article/details/gmhmwcrsh.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/gptxgtibo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fktsv.cn/Article/details/gsmjpxjuw.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/grdvgjdej.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gumrmurza.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gfoajruvl.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gsbphksnn.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gbgvielxt.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gmvfywong.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gerepajdr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/glrqwljfy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/gikutyubh.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/gwlptolrj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gfoazlzdl.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gdpgfkizs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/gprkwhqsq.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gzghpawkz.sHtML

function add(a, b) return a + b end
来源：http://blog.epnwcf.com/Article/details/gozjmqzxn.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gpayjhmps.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/guvxhwrmj.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/gweuqbgta.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gvwjioikw.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/ggodestil.sHtML

string.find(s, "%d+")
来源：http://www.share.yfazqb.com/Article/details/gomcccwaj.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gxjqwcdrq.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/guszthwns.sHtML

[T41] Perl：Hello World
来源：http://mobile.epnwcf.com/Article/details/ggaoczpfc.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gxrfqiqbc.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/gxuwevwfm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/gfhvnpkcz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gkfomeoqw.sHtML

"值: $a"
来源：http://mobile.sjlbkw.cn/Article/details/gnpbrrisi.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gvljcshgh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gypyrfqbu.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gssfdebwr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gyticiamh.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gybdwmmpg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gbenpbrcc.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gkffkomjl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/gqxustcim.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/gbuquurtk.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/glqtqfzny.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/gljobzwic.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/guhjdvaly.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gaovdpmtf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/gkkrowfzt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gyonzqwdk.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gwfjrobvq.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/ghxrjrezt.sHtML

[T52] Scala：变量
来源：http://read.share.vehdjk.com/Article/details/gifqksngn.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/goytvlsfy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gphcvumvp.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gnvnahsvz.sHtML

[T54] Scala：集合映射
来源：http://3g.yfazqb.com/Article/details/gbxrmuhfe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/govobnkoj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gthtgqrws.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/gppwsumgv.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/geszxgxvk.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/gcjgemsep.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gbteivszk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gjnvwxxof.sHtML

[T58] Scala：函数定义
来源：http://3g.sjlbkw.cn/Article/details/gbmoroabo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gpyfpxokj.sHtML

[T59] Scala：循环
来源：http://read.share.epnwcf.com/Article/details/gqbqmorzp.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gmhoavnbu.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gkejwtfsy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.yfazqb.com/Article/details/gjtstxlbc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjrerqsul.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gwwvkrabo.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gftpbsaps.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/glfsbvake.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.sjlbkw.cn/Article/details/gwxnzgbxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gzlpkxmyf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/gapnbhyij.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gtrnjmnae.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.bbcook.cn/Article/details/gvmxjxacw.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/ggoposfgj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gwkeldoeq.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gaehjepsg.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/ghnajdbqk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gccuyxlsk.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/gtvaciirf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsdrcifl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gyfgpduag.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gylrnwkao.sHtML

[y for x in nested for y in x]
来源：http://wap.sjlbkw.cn/Article/details/gippnamaf.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/gzrgtbwcc.sHtML

max(d, key=d.get)
来源：http://baike.fktsv.cn/Article/details/ghotoevci.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gsmxfhern.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/glzqgsjns.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.vehdjk.com/Article/details/gdycqackb.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/gtdbntluy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fktsv.cn/Article/details/gizjcpfwu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/geuvmrvrm.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/gopwckhfc.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gdrbuxozw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gznccktam.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gncxyhodj.sHtML

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/gzkmooqcs.sHtML

t = time.perf_counter()
来源：http://wap.bbcook.cn/Article/details/gldsdzazj.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/gkxngkjqx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.yfazqb.com/Article/details/gigwkdjjy.sHtML

[U17] Py：初始化日志
来源：http://3g.bbcook.cn/Article/details/gzgjqhnqx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gldtnuada.sHtML

[U18] Py：预编译正则
来源：http://mobile.tarul.cn/Article/details/gskogmhvi.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.vehdjk.com/Article/details/gadkvzxwz.sHtML

[U19] Py：正则替换带回调
来源：http://wap.bbcook.cn/Article/details/goqtltalv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/govjgkrdg.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.tarul.cn/Article/details/grjjcvgjn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/gbouymnrv.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gsgkfwxus.sHtML

@contextlib.contextmanager
来源：http://3g.yfazqb.com/Article/details/gneddgwbn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fktsv.cn/Article/details/gjcywcsuz.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/giaaaktxe.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gxswbhuzv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.vehdjk.com/Article/details/gxusxhdem.sHtML

[U24] Py：路径操作
来源：http://read.share.tarul.cn/Article/details/gfxaflcpr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/giqmxtokv.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.bbcook.cn/Article/details/gqbxqeasa.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/graladywv.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gqssekaty.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.vehdjk.com/Article/details/grpapydib.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.bbcook.cn/Article/details/gflpmgaxl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.vehdjk.com/Article/details/gkgkjtvnb.sHtML

[U28] Py：类型别名
来源：http://baike.epnwcf.com/Article/details/geuhleukk.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/geuccgchh.sHtML

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/gdrxocdtw.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/gndfgyrrr.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gyzhqbkdf.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gyuxziylc.sHtML

[U31] Py：单测
来源：http://3g.vehdjk.com/Article/details/gyobcvivl.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/goezyjghb.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/ggzammgrb.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqwkpqvc.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/gnrugthpk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.yfazqb.com/Article/details/garvduvih.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/gzazabtvk.sHtML

chardet.detect(raw)
来源：http://3g.bbcook.cn/Article/details/gsqryjtmf.sHtML

[U35] Py：发送邮件
来源：http://blog.epnwcf.com/Article/details/gtbwjtitt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fktsv.cn/Article/details/gurlzfmgo.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gebzdzlxc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.yfazqb.com/Article/details/guvraeekt.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gmrcuveol.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.tarul.cn/Article/details/gteuclobs.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.sjlbkw.cn/Article/details/gjjaqbung.sHtML

Path(__file__).resolve().parent
来源：http://wap.bbcook.cn/Article/details/gzpxjufhl.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.yfazqb.com/Article/details/gehiuhfcz.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gjfiugszh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.bbcook.cn/Article/details/gegdfgher.sHtML

print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/guryqojqc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/gcgutjide.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gjfkxnony.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.yfazqb.com/Article/details/gtuqfjyhe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gibsmurux.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gygxywfoq.sHtML

namespace App\Http;
来源：http://blog.bbcook.cn/Article/details/goayaormu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.yfazqb.com/Article/details/gbjgozifz.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gvsbovcpl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/gdczwlrql.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gvwppzzks.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gvopymyzb.sHtML

?string $name = null
来源：http://www.blog.vehdjk.com/Article/details/gbkrygads.sHtML

[U47] PHP：联合类型
来源：http://wap.vehdjk.com/Article/details/gdkxyqyhx.sHtML

int|string $id
来源：http://wap.tarul.cn/Article/details/goutqzour.sHtML

[U48] PHP：纯枚举
来源：http://mobile.vehdjk.com/Article/details/gbhjpnzsl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.sjlbkw.cn/Article/details/gaebutnwr.sHtML


<!-- 参考信息 -->