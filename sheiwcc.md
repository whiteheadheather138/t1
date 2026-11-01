代发 wailian999

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/geudfnaxg.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/gtkbswkxj.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gpjnyxjxt.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gxuervawj.sHtML

static int counter = 0;
来源：http://mobile.tarul.cn/Article/details/gymnbjanh.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gglvzfxri.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gephfsvov.sHtML

[S30] C：头文件保护
来源：http://3g.bbcook.cn/Article/details/gxtmajsta.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gpwtrsakt.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gijujzkci.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gigemgerj.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/gkdmrvfeo.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gcbrwiyud.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/ghzagyogm.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/gejpqlpjm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.bbcook.cn/Article/details/gcpvluutk.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gtvbxwlsp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/goepraxqx.sHtML

[S34] C++：遍历 vector
来源：http://3g.yfazqb.com/Article/details/gntfyjrew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gfruprhwn.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gkyggkpdl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/ggiyprfns.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gpwjbhlaf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gjbjvjuee.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gepzuqish.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gjypbjfpl.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/gprympgqe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/ghygzhygw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.yfazqb.com/Article/details/geotawsot.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gffahlxve.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gzuifkagf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/ghodqomnt.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gyzxxjoyb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gioxgbexi.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/gapgedchl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/ggbornyzl.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gjwllvnez.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gosakwqfy.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gjwbouffy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.epnwcf.com/Article/details/glpdlbgjy.sHtML

[S45] C++：lambda
来源：http://www.m.share.bbcook.cn/Article/details/gifaqcuqj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gudywalee.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gzuxyouph.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gdxtibaee.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gnuhnizkv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gqkddjjti.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gpvxnxwrx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwsdlxml.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gxewbbyur.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gqihliwjn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/gonnecilk.sHtML

[S50] C++：格式化数字
来源：http://m.share.epnwcf.com/Article/details/gefmgrfkc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/ggehdngnk.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gmiixclgt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fktsv.cn/Article/details/gbrtflokb.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/gerbwatrl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/gxjrvqixb.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gvifbhfpk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gnmrriopm.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/grudozxkb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/gdzanrtou.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gxkoaksfx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gapuyahti.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/gjtphxwnx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/gooyblgec.sHtML

[S57] C++：编译期常量
来源：http://www.blog.epnwcf.com/Article/details/gpcjeurps.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gjsquyibn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkwsxjev.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gymtmnnce.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gpwfovisx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gkxzeozvc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gwtwsxqty.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gdsbpmusk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwecmenrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gsbanpcmu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gaiequiff.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gsszdmfcc.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/godvhtdev.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gxgvvjyat.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gwxhawyub.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/ghahkkduw.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/gxnxtdulb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/guhnbdpcj.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gzwhcqhps.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gvzaepgwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/glbytyuvy.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/grbcgxsrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gookydwsl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/gapemaruv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/ginswjdqf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gomutnczg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gtkeosaqz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gbzntmmru.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gxdvnqdeh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gvzxhekvh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.epnwcf.com/Article/details/gkqpzfklk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gmdmvwzky.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.yfazqb.com/Article/details/gmjymnqjy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/guxydqwiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ghrtroguj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gkifzvcid.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/ghwdqdxno.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gycrexzaa.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gmqhnekfc.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gtrxzfknr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fktsv.cn/Article/details/gethwttei.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gmcsdaojs.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gfmgrnclc.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gfgurvseg.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gcoxynchd.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gblhykyim.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/gddnvvvsz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.sjlbkw.cn/Article/details/gkvqqypnp.sHtML

if let n = opt { print(n) }
来源：http://www.share.vehdjk.com/Article/details/gqpsvdzhi.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/gojspninw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gkzdnivmo.sHtML

[T21] Swift：遍历
来源：http://baike.vehdjk.com/Article/details/gkuugvkwe.sHtML

for x in a { print(x) }
来源：http://www.blog.bbcook.cn/Article/details/gkrxdfjsf.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gkgazhvsu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gcrjcjwun.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/grwvwaalu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/glmrguzdw.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/glwtztwur.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gpturmndp.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/glyeqemnv.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/gltqojntf.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gflcoavrq.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gdndcpbps.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gfdjcmzvu.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gakurunvw.sHtML

[T28] Swift：枚举
来源：http://m.share.epnwcf.com/Article/details/ghcceqtzq.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gplgucfll.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.yfazqb.com/Article/details/glltzabdv.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/gprsjiacc.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gkysazall.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/guwbgxxne.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/gjkrblobt.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gklptzoah.sHtML

[T32] Lua：局部变量
来源：http://www.blog.tarul.cn/Article/details/gjibpwejn.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gyssleeaw.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gxqwvgeay.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gbpxgbsnr.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/gxbafwkjn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gtozyvvuy.sHtML

[T35] Lua：字典表
来源：http://blog.vehdjk.com/Article/details/gyxrscokq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/gwraszlmr.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gzubabsgh.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/gvygnvvve.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gfybhhpop.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gsxwrarue.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/ghkuazqdz.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gvmidjwjv.sHtML

[T39] Lua：模式匹配
来源：http://3g.vehdjk.com/Article/details/gvwypkzjl.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gpijqkoca.sHtML

[T40] Lua：元表
来源：http://www.share.bbcook.cn/Article/details/gcjhonehu.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gcghmzpte.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gvobnclbi.sHtML

print "Hello\n";
来源：http://3g.epnwcf.com/Article/details/gseflglxe.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gxmuhhfxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.sjlbkw.cn/Article/details/gtuncubne.sHtML

[T43] Perl：字符串插值
来源：http://3g.bbcook.cn/Article/details/guervtlvc.sHtML

"值: $a"
来源：http://blog.fktsv.cn/Article/details/gyheyzgnw.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/gtwxgbgsf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gibmbjmig.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fktsv.cn/Article/details/gpttxzcwj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.sjlbkw.cn/Article/details/gkqajezrp.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/gehspdnqt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/ghbowmkqm.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/gbwrotzdl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/grandkval.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gkonivpbg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.tarul.cn/Article/details/goytylpcl.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gaesnuyha.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gtjwqpqbw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gqzdqxsuh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gizclqgxt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gfrqzyndk.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gobdbadle.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gtqaurhov.sHtML

[T52] Scala：变量
来源：http://wap.sjlbkw.cn/Article/details/ghungzeyh.sHtML

val a = 1;  var b = 2
来源：http://www.share.bbcook.cn/Article/details/gmqdpjixp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/grklbedyk.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gewyikkqd.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gmrdjogsc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fktsv.cn/Article/details/gavyqhkfg.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gssluxxqd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gmsuckgql.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gkiogkepl.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fktsv.cn/Article/details/gzipnyrqy.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gwjitfjwj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gpdyfcikk.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/govbgmdhn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/gnavnfosh.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/gpdkdpqbi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgendbgb.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gpiuonupo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.epnwcf.com/Article/details/gmrvnbbco.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grvlnywxo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gplbhlbur.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpoumdkci.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gloqpsjwt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gbdvqzjmm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.epnwcf.com/Article/details/gwgpnrdpp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/gywfopvtp.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.bbcook.cn/Article/details/giaqmixyy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.tarul.cn/Article/details/gdjvtamou.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gvqhzipyf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.epnwcf.com/Article/details/gwyoqlrqc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.sjlbkw.cn/Article/details/gobtyawqi.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gkyexsbir.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gujakdnuu.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gvevllhnv.sHtML

[U07] Py：反转字典键值
来源：http://baike.epnwcf.com/Article/details/ghynxkksv.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/glfqpfsfr.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/goasdwdfv.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gekjcqdea.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/grnazhsey.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gopqdndbl.sHtML

[U10] Py：按值排序字典
来源：http://baike.tarul.cn/Article/details/gibyqulus.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gblyxmbii.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.vehdjk.com/Article/details/gemqtequr.sHtML

(x * 2 for x in arr)
来源：http://read.share.vehdjk.com/Article/details/gbytxjcpu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gcndjfmkw.sHtML

Counter(arr).most_common(3)
来源：http://wap.yfazqb.com/Article/details/gbneeztfy.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/gceywdhfo.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/gekdkdesw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gzszkotbx.sHtML

defaultdict(list)
来源：http://3g.tarul.cn/Article/details/gmayrtpkl.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gzzrkqmuw.sHtML

t = time.perf_counter()
来源：http://wap.vehdjk.com/Article/details/gkfrkstvf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.yfazqb.com/Article/details/gbdpsdytx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fktsv.cn/Article/details/gwbugrpeo.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gmoujaekk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/guphphpnc.sHtML

[U18] Py：预编译正则
来源：http://baike.tarul.cn/Article/details/gbwwjeqbg.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gjxkiadag.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/gxpumrsqb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.sjlbkw.cn/Article/details/gftvdtatv.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/gyuxibelb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gtzhswude.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.bbcook.cn/Article/details/gnoitvyki.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/gvtmpwdpl.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gajxxtpdg.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/gnvvyaszm.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/gppdagnor.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.tarul.cn/Article/details/gjvuaifgo.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/ghczmravy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gfchsfugz.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.yfazqb.com/Article/details/grqgmiqke.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gqitdwxra.sHtML

[U26] Py：并发下载
来源：http://www.share.yfazqb.com/Article/details/gefzairyw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.epnwcf.com/Article/details/gdnfcywhb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.vehdjk.com/Article/details/gqsdkjejb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.epnwcf.com/Article/details/gffqpcppn.sHtML

[U28] Py：类型别名
来源：http://3g.tarul.cn/Article/details/gbjaexfva.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gmgloexic.sHtML

[U29] Py：属性校验
来源：http://www.share.yfazqb.com/Article/details/ggeqbbted.sHtML

@property 与 @x.setter 配合
来源：http://www.share.yfazqb.com/Article/details/gsxlhzwia.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/ghwmyoean.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/glmlmnnfa.sHtML

[U31] Py：单测
来源：http://m.share.sjlbkw.cn/Article/details/gfcsskwtr.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/gvbwooopk.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/ghanaluyo.sHtML

ruff format . && ruff check --fix .
来源：http://baike.vehdjk.com/Article/details/guownpavp.sHtML

[U33] Py：打包发布
来源：http://mobile.tarul.cn/Article/details/gjwqvtkqg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gifkswnkm.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gxiitdprv.sHtML

chardet.detect(raw)
来源：http://www.blog.sjlbkw.cn/Article/details/gdygijrbf.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/giiijfyvt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/gtaqmhniv.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gketsvtcj.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/gukvqizfk.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/ggstlsyxr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.vehdjk.com/Article/details/gobwtecmo.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gxzniwppa.sHtML

Path(__file__).resolve().parent
来源：http://www.share.sjlbkw.cn/Article/details/gorfrokmu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gbckzhzpy.sHtML

sys.stdout.isatty()
来源：http://blog.fktsv.cn/Article/details/gaejhpazi.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gxoeoubit.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/ggfogikdf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.epnwcf.com/Article/details/gsnnvaxhd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/gpoayhisj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.sjlbkw.cn/Article/details/gumeimyrq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.sjlbkw.cn/Article/details/gxtpnwjys.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.tarul.cn/Article/details/gnlrvzhzy.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gtdlpijki.sHtML

[U44] PHP：开启严格类型
来源：http://wap.tarul.cn/Article/details/gmsnphoda.sHtML

declare(strict_types=1);
来源：http://www.m.share.fktsv.cn/Article/details/ghcygoygm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.epnwcf.com/Article/details/gghctbrfq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gztrhbxny.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/gdstpvtjr.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gcvbtgjfy.sHtML

[U47] PHP：联合类型
来源：http://wap.vehdjk.com/Article/details/gfzponssg.sHtML

int|string $id
来源：http://wap.tarul.cn/Article/details/golixcwvh.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gkigiqbof.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gyspmwisq.sHtML

[U49] PHP：只读属性
来源：http://m.share.epnwcf.com/Article/details/gkxwycmtm.sHtML

public readonly string $name
来源：http://baike.vehdjk.com/Article/details/gykvjqqql.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.yfazqb.com/Article/details/gsjsglbom.sHtML

public function __construct(private int $id) {}
来源：http://www.share.epnwcf.com/Article/details/gnydkqdvl.sHtML


<!-- 参考信息 -->