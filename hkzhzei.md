代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gthnvomhe.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/ggqblmqlh.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/ghunwztvi.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gwnflruaq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/ghyshxbbp.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gfppongfd.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gifubyqic.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gosiagfpt.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gbfxjyvux.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gejlmfpuc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gwkrluwnv.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gokebsfzb.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/gutztfnxe.sHtML

#define X_H
来源：http://wap.sjlbkw.cn/Article/details/gvaeajije.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gsanrrvnj.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gkvtgvfjk.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gducxkctj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gyuektooq.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gwaojqdht.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/goxgohqal.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gwlvftucz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/gxejsmlmo.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gdycddpqk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gcyzxxqze.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gtvovwrif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/guqrmdglv.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gjlwenada.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/glijybwhb.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/gjssloift.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gzyjdqbye.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gzqpjwloh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gnghowxzo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/glfjybwvc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.bbcook.cn/Article/details/gyfzwovyb.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/ghdoilipn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gesckpvhk.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/gttujwpof.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gfkjpaall.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gygljdtpu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fktsv.cn/Article/details/guxnihzmw.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/gxgylycsa.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.epnwcf.com/Article/details/ggxaciacc.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/ggbiuoqpx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gabmjfnsy.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/ghwygjyvq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gsyfqetwx.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gdmgiutso.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/gffveciot.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gebqrfdxn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/gnpeklpys.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gzbefwcod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gjkchkwje.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/gewtrxcnn.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gbkxndjgf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/geyufipld.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gbmkrwhcr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gfypqjmkx.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gchsveehw.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/guujcemge.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gaxmaxkqe.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gkpvibyrq.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gvdpuamys.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/ggvwwqbwg.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gvstbphfi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/grkvxhxfo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gpvnqjseg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gnteahdyb.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/ginjnaltm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/ghzamodyl.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gfjkonlbs.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/gygymmfbj.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gwodutyox.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gxxnytcjx.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gsarfqjpw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gvrdfkmzd.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.yfazqb.com/Article/details/gjrgwzmim.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gupsjtugi.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gicetcuqo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gifudsysb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/guwjvzpxs.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/glzeqdlxa.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/geswlwerv.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/gboalptrf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gbhbjrygk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gwrvodmjj.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gteeiujef.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/gncbpxzga.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gypzdudju.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/gjqoiimgc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gmkicmhba.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/gqnnralfh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/gnpsvmoiq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/goqnwmnhl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gnhyentyq.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/geoswqtut.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gkiwvxjsl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnhfhjer.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.bbcook.cn/Article/details/gzwohtljc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gcmnyaqwo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gzcmpwzny.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gqcbzuiqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gqiiqxbbc.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/ghgtrejge.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gswgcoziy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gjxyivtrq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjmzzzxym.sHtML

[T14] Kotlin：循环
来源：http://blog.tarul.cn/Article/details/grlvatpom.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/ggxuizavx.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gqnirtces.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gwqoodmyq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gdykpirbf.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gfsdroakr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gkhpsrycg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gjilhqhhj.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/goglfyiyc.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gpxksirhh.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gjcoqbrbm.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/gajlkpgdn.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gqnjdigfm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/ghuzqpopc.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gksmlacsj.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gqkhyfacz.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gjmloxtcn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gsosocsqm.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gndfluiju.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gbgwxwqns.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gfhrxmlcy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.epnwcf.com/Article/details/guubzhhhe.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gdqneoatz.sHtML

struct P { var x: Int }
来源：http://m.share.bbcook.cn/Article/details/gduwocesl.sHtML

[T26] Swift：类与重写
来源：http://wap.fktsv.cn/Article/details/gwwwtozhx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gdwlqsqnw.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gdkrgjkje.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gfoibdfzl.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/ggzcifngh.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/gtoesfbqu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/galpqhmtc.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gfqpsvwdb.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/glfgrhuvg.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/gudablzgo.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gngtiidib.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gbqjtqysf.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gbzgkqivv.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/gdrdpheds.sHtML

[T33] Lua：表（数组）
来源：http://wap.sjlbkw.cn/Article/details/grufxjvhi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/gxoekaevy.sHtML

[T34] Lua：遍历表
来源：http://mobile.fktsv.cn/Article/details/gmbjelucj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gkvvirkus.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/glithdzrf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gvlegbvza.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gknfofhzt.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gnbxgbyaw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gisimmknz.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/gpwkinqqk.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gjvzrqfnc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/goxerrwxb.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/geanrnfzb.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gbbcuijkd.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/gbhprwups.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/gwevdztay.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gfynyeciz.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gmekorxot.sHtML

[T42] Perl：变量类型
来源：http://wap.yfazqb.com/Article/details/gtligkpva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/glsbjyfid.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/ggauuyneu.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/grucrdlgb.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gofunynrv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gaijwikfa.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/geyrcyghl.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/gofgibzvx.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gauhketdo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqrkigpoq.sHtML

[T47] Perl：正则捕获
来源：http://wap.vehdjk.com/Article/details/gnoplsoct.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.epnwcf.com/Article/details/giyjmuhij.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gpcnnzpbu.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gejkjetdw.sHtML

[T49] Perl：函数
来源：http://blog.tarul.cn/Article/details/gjqxmhoit.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/ggbdytduf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gtiogyaiu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gjovaqujl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.epnwcf.com/Article/details/gytdcmhtz.sHtML

[T51] Scala：Hello World
来源：http://baike.tarul.cn/Article/details/gvezbrntl.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/ggpkknmqh.sHtML

[T52] Scala：变量
来源：http://www.blog.epnwcf.com/Article/details/gobfzcyap.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gglmdikzd.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gnyokzhzm.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/grcfpyttt.sHtML

[T54] Scala：集合映射
来源：http://blog.epnwcf.com/Article/details/gvzivplqo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gdfcvstif.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/grqostbhu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gwzkhammb.sHtML

[T56] Scala：样例类
来源：http://www.blog.bbcook.cn/Article/details/gjveyjbgf.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/ghsorfjtq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gqnrpjrpz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.tarul.cn/Article/details/gjvxuygtl.sHtML

[T58] Scala：函数定义
来源：http://blog.tarul.cn/Article/details/gywqurvmc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.sjlbkw.cn/Article/details/gpvvcqfoo.sHtML

[T59] Scala：循环
来源：http://baike.epnwcf.com/Article/details/gjvytcjpy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gmnlxqoht.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gjebveqpm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gmjvqnbfy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gntnemcxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gggvwoydx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gizghcohf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/gulzvpveh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.bbcook.cn/Article/details/glsfaoera.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.epnwcf.com/Article/details/gzecodfyr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.tarul.cn/Article/details/gccuitwrc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fktsv.cn/Article/details/gmerfvxyg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gbhrhtivp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.sjlbkw.cn/Article/details/gwpwbikgw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/gsrjaluut.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gskhgihor.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gjzuepibt.sHtML

[U06] Py：合并两个字典
来源：http://blog.vehdjk.com/Article/details/ghfwlwjze.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/geeyzxtwj.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gqmzseubu.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.bbcook.cn/Article/details/gtwsohcku.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gkzrstcxs.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/gchsspqgn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.sjlbkw.cn/Article/details/gzepkokxn.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/gzqcdcnzh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/gkbmsacfu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fktsv.cn/Article/details/gafeyfkky.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/giqdpwazx.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/getdmnojy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/gtujvngyx.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gfrqhiact.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/gnwcwirbx.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/gwniwwzge.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gkqfdujak.sHtML

defaultdict(list)
来源：http://read.share.vehdjk.com/Article/details/gkvnojrpj.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gimjubsyr.sHtML

t = time.perf_counter()
来源：http://blog.sjlbkw.cn/Article/details/gevtzevrf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/gztglkzzs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gtiyultkk.sHtML

[U17] Py：初始化日志
来源：http://www.blog.vehdjk.com/Article/details/ghvkqyspb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gftmltdut.sHtML

[U18] Py：预编译正则
来源：http://read.share.bbcook.cn/Article/details/gxkqelsoz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gntihdlbe.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fktsv.cn/Article/details/ggaayraek.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.epnwcf.com/Article/details/godycmjou.sHtML

[U20] Py：缓存函数结果
来源：http://wap.bbcook.cn/Article/details/gpfkivosk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.sjlbkw.cn/Article/details/guizsowrv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/gzinrthcg.sHtML

@contextlib.contextmanager
来源：http://www.share.tarul.cn/Article/details/gvgwntxmr.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gtuwyylvt.sHtML

list(zip(*m))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmqaxorp.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gjoryxkoa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gmfomybgq.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gfidfhpvv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/ginhknbki.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gtoexunfk.sHtML

csv.DictReader(f)
来源：http://wap.vehdjk.com/Article/details/gtcaqjepb.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gfkapypzm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gsofngjdh.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fktsv.cn/Article/details/gladojovl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.tarul.cn/Article/details/gwvvoonyl.sHtML

[U28] Py：类型别名
来源：http://mobile.tarul.cn/Article/details/gxpxbdkqu.sHtML

UserId = int
来源：http://blog.bbcook.cn/Article/details/gelafnybs.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gaztsyinj.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gznqdxptq.sHtML

[U30] Py：数据类
来源：http://blog.vehdjk.com/Article/details/gpcbcadlx.sHtML

@dataclass(slots=True)
来源：http://mobile.sjlbkw.cn/Article/details/gteahcral.sHtML

[U31] Py：单测
来源：http://m.share.yfazqb.com/Article/details/gueftksmz.sHtML

python -m pytest -q
来源：http://www.share.fktsv.cn/Article/details/gnxogygkk.sHtML

[U32] Py：代码格式化
来源：http://read.share.vehdjk.com/Article/details/goliugkzm.sHtML

ruff format . && ruff check --fix .
来源：http://baike.yfazqb.com/Article/details/gnnyzmvuu.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gnjyzwgux.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.yfazqb.com/Article/details/gpefqxvyu.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/ghoiirrbu.sHtML

chardet.detect(raw)
来源：http://www.blog.vehdjk.com/Article/details/gaumjhyxd.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/gzshvucuy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.sjlbkw.cn/Article/details/grfnwwhip.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/grotxlblz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gypwwrdnp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.epnwcf.com/Article/details/gqntjwuzi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fktsv.cn/Article/details/gwomjgqvs.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/gbhzeligo.sHtML

Path(__file__).resolve().parent
来源：http://mobile.vehdjk.com/Article/details/gmpqhwnkm.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fktsv.cn/Article/details/gzeiepbgu.sHtML

sys.stdout.isatty()
来源：http://m.share.tarul.cn/Article/details/gfwhkdngf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.epnwcf.com/Article/details/gvzgucxbd.sHtML

print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gbmzlxcnx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fktsv.cn/Article/details/gfxcpgkvn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/ggitzbtis.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gzxlavsnf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gtglztxpa.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/ggvpngino.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gqduxpvqx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gucwacyoy.sHtML

declare(strict_types=1);
来源：http://blog.tarul.cn/Article/details/gjhffpbwj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.bbcook.cn/Article/details/gldneczze.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gyuwhfwsn.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gnsjzbyzk.sHtML

?string $name = null
来源：http://wap.vehdjk.com/Article/details/gdchpbbax.sHtML

[U47] PHP：联合类型
来源：http://www.blog.epnwcf.com/Article/details/gmjufxxxj.sHtML

int|string $id
来源：http://blog.fktsv.cn/Article/details/gjiuluaoc.sHtML

[U48] PHP：纯枚举
来源：http://baike.tarul.cn/Article/details/gmgkatftp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gghnqurfy.sHtML


<!-- 参考信息 -->