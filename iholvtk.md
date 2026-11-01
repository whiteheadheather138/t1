代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/guarwxmzj.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gaizzlwai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gzcfswyok.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/gavrlgclm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gitjjtdnm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gisfvauqo.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/gkogcytzo.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/giomyngoz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/goyrauqec.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gvctzjyed.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/grgongrlw.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gyjlxcozc.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/giitqdful.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gnpttdqiv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gryrcccbj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gbmihhkcv.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gvjlvhncg.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/glvwwwdkp.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gmtzmlihl.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/grlilwcnz.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/gzjalzxds.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/ghkffvxqt.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/gnyeliptu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqfqeeda.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.epnwcf.com/Article/details/guyrfejja.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/ghdntpdht.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/grxawfuyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.bbcook.cn/Article/details/gpcsdoath.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gekngzpxb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gddurwhbf.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gfyhhrpeo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gbmxdyods.sHtML

[S37] C++：set
来源：http://blog.sjlbkw.cn/Article/details/gusjbfdjs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/gtastiwrh.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gdedmujxk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gptpnunvi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gmuihogcb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gqqjfknwi.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/ghxvxllbk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/ghgfonlpi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gmpmpthnk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.vehdjk.com/Article/details/giaeiqgog.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gkrlggbnz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gvxzjbtaf.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/guhhxpnaf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gjodjuvzb.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gnhgxxbcc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gqtleuoab.sHtML

[S45] C++：lambda
来源：http://www.blog.epnwcf.com/Article/details/gcirzemil.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gdctbnfad.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gazlchash.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gvlbbvyys.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/ggvgejblh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gymxjadle.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/grwrvtqtp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gqdlraqel.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/ggemwtiox.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/grmzchppu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/glfsurbrs.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/grflqtrbs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.yfazqb.com/Article/details/gqyqrzxux.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gbzijpkuu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gblamruab.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/guisbivwf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gerbrisqa.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gtasmbxqj.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/greweiksl.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gbontskrj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/golrzcgsx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gxfouzdeg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gvrfuymjs.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gbadiydit.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gazbsmhdq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gwyvcafjh.sHtML

constexpr int N = 10;
来源：http://mobile.bbcook.cn/Article/details/gnrjnrorx.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/grnxpypel.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gfaduiprz.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/gyxuuqrbc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gqtjpekyk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fktsv.cn/Article/details/grrmfjeob.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gbaqjzbwo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grpkcxyup.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/ggndvrpwq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjsrazymf.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ggfhviqnx.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gvyoxxdfd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gojcswssr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/goumkrlyf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gblrhskve.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/grvkntpwo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gnpyhhirz.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gypdilufb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.yfazqb.com/Article/details/gfqwfymnz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/glzwtmajd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gzwqfhftm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.epnwcf.com/Article/details/gnruuglvk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gbikavzyx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gztxwsnes.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gdvtajvxf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gcjzujaac.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gcjwqamnl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gshstuoru.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gkjsulcno.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/gakgelqcr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gqcqsmncl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/giwsvobuu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gmdktserp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gkdepwrkf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/glnyldmiu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/grumjhuac.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/ginneejyn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/grhxlnupn.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gcqudwftp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/gludaznrr.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gcfnbzcxg.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gqhhdxunr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gtkggbrft.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/ggtshjfvw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gxooettdc.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gefsvnfls.sHtML

[T19] Swift：可选绑定
来源：http://baike.sjlbkw.cn/Article/details/golhlbnuv.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/gudhurokf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/giiuolrlo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.bbcook.cn/Article/details/gesfayuvl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gpakmnglf.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/glbrlykzh.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/giszrjkwc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gzmkbarxg.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/gaewxaaxz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/gnkdpxpxz.sHtML

[T24] Swift：闭包
来源：http://blog.tarul.cn/Article/details/ggwixvwlr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.tarul.cn/Article/details/gaxpntwpp.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gvnsdiwlg.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/goegdpfnb.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gluorjevw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.yfazqb.com/Article/details/gwjlggcwh.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/gmpkqvahx.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.epnwcf.com/Article/details/gsryapwad.sHtML

[T28] Swift：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gsoqdvwzs.sHtML

enum Color { case red, green }
来源：http://mobile.fktsv.cn/Article/details/gizpfmbmz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/gwzvgzpye.sHtML

guard let x = opt else { return }
来源：http://www.blog.tarul.cn/Article/details/gpgjysvnb.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gkhopdepf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/gvpgkjwnk.sHtML

[T31] Lua：Hello World
来源：http://baike.yfazqb.com/Article/details/gciyqrxfl.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gtlmrojen.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/grcpvoyzv.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gfmhgeklu.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gifjkhgfr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/gibjfgeny.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/gawvdohfv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/gruxrvliw.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gmpqktggy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gjvxbnpdn.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gjhduskwz.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gpydrjpqj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gjuuuzpaq.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/gulieqqsr.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gkvnkgihg.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gdasmqylg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/ghiphotch.sHtML

string.find(s, "%d+")
来源：http://www.blog.bbcook.cn/Article/details/gugxfooby.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/gxbeikbwj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gxkwrbtub.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/grdqqkrtr.sHtML

print "Hello\n";
来源：http://www.share.tarul.cn/Article/details/gcgmwoboh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gsrigkhos.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/gwgpahhvm.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gkovygeak.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gyhuutnyh.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gwdfkkezb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gdfvepgyg.sHtML

[T45] Perl：数组遍历
来源：http://3g.bbcook.cn/Article/details/ghbilhmyw.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/gvnnndfua.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/ghcvgvzrz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gldglrhtr.sHtML

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/gvtpanmpg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.epnwcf.com/Article/details/gerwjwgoh.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/gqdytgsay.sHtML

$s =~ s/old/new/g;
来源：http://mobile.bbcook.cn/Article/details/gxzvstfrj.sHtML

[T49] Perl：函数
来源：http://www.m.share.epnwcf.com/Article/details/gcknqwmis.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gfittlmfv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gxqclwbfn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhabaupm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/geixsgcll.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/guqyocslz.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/glgjjqsee.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/guxszibvn.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gsiowgzfo.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/glpvubbtc.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gfyobmeah.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gnoidxoum.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gsnzosmkk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/gxipacxzg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/goivlwctf.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gygkbnxjv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gqrycwiro.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/grkmsljbs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gzazqhhcx.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gfzgdjxxy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.sjlbkw.cn/Article/details/gzhmgkxxv.sHtML

[T59] Scala：循环
来源：http://mobile.tarul.cn/Article/details/gebizqcdf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gdtwqfwua.sHtML

[T60] Scala：折叠
来源：http://baike.yfazqb.com/Article/details/gwlpdgwqw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/grgosugkx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzhzdghbh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gaumyiqeg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gundjjcsf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/gikhbiuxe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/gkklypvjw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/gkjnrzxzx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.vehdjk.com/Article/details/ggycgieda.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gqgxlzwjy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.vehdjk.com/Article/details/gfyyilyef.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdhjjjkq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gyaniepnu.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gssbvluev.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gtgenkjgy.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gqmehpueu.sHtML

{**a, **b}
来源：http://3g.fktsv.cn/Article/details/godfgdxis.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/gwzpbkbxg.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.vehdjk.com/Article/details/ghsxdlrtr.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/gphpiamif.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/ghjauypnm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gzxjweppc.sHtML

max(d, key=d.get)
来源：http://www.blog.tarul.cn/Article/details/gixqzjkmf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gvpkfftuw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gbpgckqzw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.tarul.cn/Article/details/gkmedilib.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gltqkpprb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.tarul.cn/Article/details/gzuyaylrj.sHtML

Counter(arr).most_common(3)
来源：http://www.share.sjlbkw.cn/Article/details/gdayvrdsv.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/ghduqwnrj.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxoalfil.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gmqwwmdyz.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gftgiszov.sHtML

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/gprtpzkxd.sHtML

t = time.perf_counter()
来源：http://baike.sjlbkw.cn/Article/details/gkchyeykn.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gznuoaxrd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gcorwcfez.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/gvhojxxje.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/gygukgkza.sHtML

[U18] Py：预编译正则
来源：http://wap.epnwcf.com/Article/details/gqikxwwnm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/gdbucteec.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.sjlbkw.cn/Article/details/gfedboebd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gciixyqty.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.yfazqb.com/Article/details/gmrcyeyxf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/gyaneefoj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.tarul.cn/Article/details/gaslquijt.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/gukejrrim.sHtML

[U22] Py：矩阵转置
来源：http://m.share.sjlbkw.cn/Article/details/gcpqhmhyy.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gqdxbajgt.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/gdfymjoop.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.yfazqb.com/Article/details/gmwuixjpm.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/guxqemtnc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/giinttgtx.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gceebbuar.sHtML

csv.DictReader(f)
来源：http://baike.fktsv.cn/Article/details/grnxvsdum.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/gipkwjeso.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.bbcook.cn/Article/details/gochlejaw.sHtML

[U27] Py：异步 HTTP
来源：http://wap.vehdjk.com/Article/details/ghjdiples.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.epnwcf.com/Article/details/gpqviykqz.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/geflrfyjw.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/grialuduq.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gkoxileqi.sHtML

@property 与 @x.setter 配合
来源：http://mobile.tarul.cn/Article/details/gvnkrmxms.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gfxywifpf.sHtML

@dataclass(slots=True)
来源：http://wap.yfazqb.com/Article/details/guyjsebwq.sHtML

[U31] Py：单测
来源：http://blog.tarul.cn/Article/details/glxdztrmy.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/ghiecxprl.sHtML

[U32] Py：代码格式化
来源：http://read.share.fktsv.cn/Article/details/gvseovxcv.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.epnwcf.com/Article/details/gspvoeekp.sHtML

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gurvltfuj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gitjghnuc.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/gvlmnlltr.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/glcqhrbkd.sHtML

[U35] Py：发送邮件
来源：http://baike.tarul.cn/Article/details/gjbgmapyi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gfrkanhtd.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/gwbxoxvwu.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/gubivptys.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gjqilhled.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.tarul.cn/Article/details/gudpluowu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.yfazqb.com/Article/details/glnqbjyeq.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gsdvxqipt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/ginecugvt.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/gddkjbrab.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/gpmnaoxcd.sHtML

print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gqyqtliuu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fktsv.cn/Article/details/gdiwpgaqc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fktsv.cn/Article/details/gcrecdvyv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/gofdywtgr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/ghdzyvkcz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.yfazqb.com/Article/details/gziebrumk.sHtML

namespace App\Http;
来源：http://3g.tarul.cn/Article/details/gwhhripyh.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.bbcook.cn/Article/details/goghjiqbt.sHtML

declare(strict_types=1);
来源：http://wap.vehdjk.com/Article/details/grqnwcptu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.vehdjk.com/Article/details/gzloxyvem.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gehvnnlcs.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/gaapmuvmi.sHtML

?string $name = null
来源：http://blog.vehdjk.com/Article/details/gpsrfjwah.sHtML


<!-- 参考信息 -->