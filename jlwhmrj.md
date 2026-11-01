代发 wailian999

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/gufneysiu.sHtML

[S29] C：变参函数
来源：http://www.share.fktsv.cn/Article/details/gwgkspruf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/gvialfthc.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gubdemxsm.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gqpttofla.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/glrjpowwk.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gfjghthpr.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gceyruzdm.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/guqvftspa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fktsv.cn/Article/details/gicxujobp.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/goxurxlav.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gqvlznnvx.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gbnvjqqoi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/gncmlqmpw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gosltruoc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/glkftcksj.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gevoumvvt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gbkvqgpty.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gvbtkhcpv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gwwyjxnoo.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gkcdinkrn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gfpqrgetb.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gtfoujxmz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gewatinvt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gwrizkhnp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gjuzkmbwe.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/gvvycowjv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/guzbfupxk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gmqkbjunz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gvxindxen.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gstwavdkv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gmacsoenb.sHtML

[S43] C++：智能指针
来源：http://baike.bbcook.cn/Article/details/gptcocarz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxvsoyij.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gtymrwfma.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gvhvgnnsg.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gpprnstkk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/gvccgscrd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gjpmqxvwi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gaubdcpqk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gpvkspyeh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gyerpbore.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gavmpntyl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gqqehquyw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/gwolqnjqh.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gccmmmouv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gyvxeldqu.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/girlziapq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gifdejxtw.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/gpftehjtr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/geutibwql.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gpmekeimz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gngfcgpoz.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gqcqbskiu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/gwegusuqx.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/ghgghfpce.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gmkctljrj.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gkclnaciw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/grmjatqsg.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gmkfqxynr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/ggdvsvzbm.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/gtmdagzqx.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gsejrohga.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gjqrgaoqd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gbgilvdci.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gfxyurliy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/glzghinud.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gmotqvveu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gaucfqabr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gukknpgbh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gdvethttu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqieuhryx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtwwnpqox.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gdgushxpd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gjmcjuzzf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gedwbzaqg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gtspqioxl.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gwpufzaix.sHtML

[T04] Kotlin：空安全
来源：http://baike.bbcook.cn/Article/details/guvlcwlem.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gtdjamnvv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gjdjxmjcu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gpdsirgel.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gegqgjddo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/glxvuvorz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gxgduowty.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.yfazqb.com/Article/details/ggoofwifv.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gqzkxhovi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/ghfuaeduc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gilutugpt.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gfoerayst.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gkfscqksj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gdwumhroe.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gyibwxskn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/ggeoziclg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gsrxokfjl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/gpauvhisk.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/glqulalzj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/glsxjhtfa.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gsgositbz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gieqjvdzi.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/ghnxhxhjz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/ggtiwzcql.sHtML

[T16] Swift：Hello World
来源：http://3g.tarul.cn/Article/details/goqrvpfgy.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gcvpipptj.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/gjnhzoobc.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/gwdinnlvb.sHtML

[T18] Swift：字符串插值
来源：http://blog.tarul.cn/Article/details/gwxvkdqay.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gbdxduadw.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gujwicuek.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gurvzvdfs.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gjpzwhdsb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.yfazqb.com/Article/details/gfufzmnhq.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gomxbcshe.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gxevnyoqy.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gigjhnqbo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/gzfijfrxf.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/gxqrvomqo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gyxmlhpii.sHtML

[T24] Swift：闭包
来源：http://read.share.sjlbkw.cn/Article/details/giqojsctg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.tarul.cn/Article/details/gvcawyeqc.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/gzhswatsg.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/gvvtcmozp.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gfuikhrbs.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/gkjbrgzgr.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/grpigusxs.sHtML

do { try f() } catch { print(error) }
来源：http://wap.epnwcf.com/Article/details/gcugfbtqg.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/ghrqtfzfh.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/gqhheewge.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.vehdjk.com/Article/details/gbcyzoxcd.sHtML

guard let x = opt else { return }
来源：http://m.share.yfazqb.com/Article/details/goxkccsls.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gmitxvigx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gigvesymy.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/gvtwnlhip.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gkjwcymjo.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gcvijyoai.sHtML

local a = 1
来源：http://mobile.vehdjk.com/Article/details/gpfpsiniv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/gneqvevkp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.epnwcf.com/Article/details/gnvbxviof.sHtML

[T34] Lua：遍历表
来源：http://3g.sjlbkw.cn/Article/details/gxuxvhywn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/gpqosjfez.sHtML

[T35] Lua：字典表
来源：http://blog.sjlbkw.cn/Article/details/gbfrswwzv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.vehdjk.com/Article/details/gqrewqfqc.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gsglfmfop.sHtML

function add(a, b) return a + b end
来源：http://read.share.tarul.cn/Article/details/gajjuseou.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gdjmowjal.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gzwcwdypu.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gfzrxvwjw.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/giwwnmkba.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gjwpywleq.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/gkhzwpodi.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/gdmnovgsx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gkyucgnpb.sHtML

[T41] Perl：Hello World
来源：http://wap.vehdjk.com/Article/details/gyhwgywfr.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gxqlikecd.sHtML

[T42] Perl：变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gvkjznvpt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.tarul.cn/Article/details/gdokyzntz.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/gjfhqkpnj.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gqbeauzbh.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gtfprnwzw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gzxgsolbv.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gnzxiyghk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gkuxbzfht.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gglxdxhgc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.bbcook.cn/Article/details/gsmgilmmb.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/gbgerbmfg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gglxzlktt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwyfaszx.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gzjwwrwuf.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/gwulfcdjo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gsnwsanhe.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/ghvyyuryi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/grrgqqcda.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/glcwqfybg.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/gcquyuled.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gtpkqlncw.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/gqvgllhjm.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/ggnolnyob.sHtML

[T53] Scala：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gqchksvbl.sHtML

s"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gqqkdgugf.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/gxrysmjnr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.tarul.cn/Article/details/gwitiuoeu.sHtML

[T55] Scala：集合过滤
来源：http://3g.fktsv.cn/Article/details/gxotseulb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/ggbhjrsep.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/gifhsshud.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gjlxqpynb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gheuvszjo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gumhvonos.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gaohlnjig.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/guzrwwswu.sHtML

[T59] Scala：循环
来源：http://www.m.share.fktsv.cn/Article/details/gaxbbchlu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gfzxdhnix.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/ghvcbraak.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gejbshaps.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtvmtkqwu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gozoyfcui.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjnmuhzut.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/gutfdskaz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/ggnozxcyw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.yfazqb.com/Article/details/gesncxink.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/grzkdgztn.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gdphnzgdk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gwxavttqa.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gcrfzpokc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/ggwoxokhn.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gudrqixyz.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/goahexlps.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/glaolczhz.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gzgrsdxbv.sHtML

[U07] Py：反转字典键值
来源：http://blog.bbcook.cn/Article/details/geexukdbe.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/grfvwktag.sHtML

[U08] Py：展平二维列表
来源：http://blog.sjlbkw.cn/Article/details/guolichcf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fktsv.cn/Article/details/gheocvkbn.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.sjlbkw.cn/Article/details/gcciirgke.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/gjumensrq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gxxiuehmu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gpcdnxcfo.sHtML

[U11] Py：生成器表达式
来源：http://3g.yfazqb.com/Article/details/gqglrbgzy.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/gswylufon.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.yfazqb.com/Article/details/gzmjtyviu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gxrnpxgkh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/giukokcwn.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/guqnevzqy.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gdtorzboc.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/gkokkallj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/gpkznwukd.sHtML

t = time.perf_counter()
来源：http://read.share.fktsv.cn/Article/details/godfdfyug.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/geuavoddr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.sjlbkw.cn/Article/details/gjfgogkmr.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gsxoiciqb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/gredqaxpm.sHtML

[U18] Py：预编译正则
来源：http://www.share.yfazqb.com/Article/details/geceldigw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.yfazqb.com/Article/details/gxraamzij.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gedgapzzs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gggijijzl.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gbvmasass.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gwggrcvcq.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.yfazqb.com/Article/details/gvtagppuk.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/gesknratm.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/gqhhlmjug.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gjsghldbz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.tarul.cn/Article/details/gyacksmyy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.tarul.cn/Article/details/grkjjbadi.sHtML

[U24] Py：路径操作
来源：http://m.share.vehdjk.com/Article/details/gnfuayjxh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gptqvpfag.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/grkabobcx.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gxnxnycac.sHtML

[U26] Py：并发下载
来源：http://read.share.fktsv.cn/Article/details/gxzlrvufo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gguaiygxd.sHtML

[U27] Py：异步 HTTP
来源：http://baike.yfazqb.com/Article/details/gybzqfptm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/glqtaldpx.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/ggubgwulb.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gfgdbmwdy.sHtML

[U29] Py：属性校验
来源：http://3g.fktsv.cn/Article/details/gdcrdyhru.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gwbknielu.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gngwumdvs.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gkzfmynhq.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gfuwxkopi.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gpcgrmzqt.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gsrfjwoix.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.tarul.cn/Article/details/gdaqfqbik.sHtML

[U33] Py：打包发布
来源：http://www.share.sjlbkw.cn/Article/details/gwcnfdknd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gajbbzitv.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/glrtxvzdc.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/gyvlphhhj.sHtML

[U35] Py：发送邮件
来源：http://wap.sjlbkw.cn/Article/details/gwjnqahwv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.yfazqb.com/Article/details/gompibvpb.sHtML

[U36] Py：定时任务
来源：http://3g.fktsv.cn/Article/details/gffelvuye.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.yfazqb.com/Article/details/gambzgxvw.sHtML

[U37] Py：读写 Excel
来源：http://3g.epnwcf.com/Article/details/gxljvrfwn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/gklfezkxw.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.bbcook.cn/Article/details/gnroiwuqh.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gggpdnano.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.yfazqb.com/Article/details/ghiyogtwo.sHtML

sys.stdout.isatty()
来源：http://blog.tarul.cn/Article/details/ghxudgtth.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/ggxipovdn.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gvdqgpbyv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.tarul.cn/Article/details/gaiaibvjo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fktsv.cn/Article/details/gcqojbpmq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/gxptqizjh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.vehdjk.com/Article/details/gkgqmitzr.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.bbcook.cn/Article/details/gggwyickf.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gjrdunnbw.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.bbcook.cn/Article/details/gmmggjvlo.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/gkzjckzaf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.bbcook.cn/Article/details/gskzedeyj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gqcganmii.sHtML

[U46] PHP：可空类型
来源：http://www.share.yfazqb.com/Article/details/gdwnkofhh.sHtML

?string $name = null
来源：http://www.m.share.bbcook.cn/Article/details/gkhxfmgip.sHtML

[U47] PHP：联合类型
来源：http://www.blog.epnwcf.com/Article/details/gvupxotlm.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/ghqgfniiu.sHtML

[U48] PHP：纯枚举
来源：http://3g.sjlbkw.cn/Article/details/gkxwedycq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/gxubasfhg.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gnlodgmcc.sHtML

public readonly string $name
来源：http://read.share.yfazqb.com/Article/details/gunsogwof.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.epnwcf.com/Article/details/ggvssygaw.sHtML

public function __construct(private int $id) {}
来源：http://wap.vehdjk.com/Article/details/gqjavybqq.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gogxradfz.sHtML

[$a, $b] = $arr;
来源：http://read.share.sjlbkw.cn/Article/details/gzasguxie.sHtML

[U52] PHP：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gvaxemkvw.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/glmzsywhc.sHtML


<!-- 参考信息 -->