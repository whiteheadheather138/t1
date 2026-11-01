代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/grtktfesd.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/ghkcgfuzi.sHtML

memcpy(dst, src, n);
来源：http://blog.sjlbkw.cn/Article/details/gpolzczog.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/ggfqrebkg.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gtjplzozv.sHtML

[S27] C：定义常量
来源：http://3g.yfazqb.com/Article/details/gjbiccgtt.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsqjgbcc.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/geornfhan.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/glwxkpbmy.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gpwjutwuy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gbeegapix.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/grsjzofjy.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gxfalnavu.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gcnpvnfgu.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gjzomkwmv.sHtML

[S31] C++：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gegxkbcmz.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/grzswcfwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gxevccpla.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/golulqaah.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/ghpzgsrrq.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gfjkxpuln.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/ghqyomwdu.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gkxgyfeqt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.yfazqb.com/Article/details/grppbacop.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gtapukptr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gcnurquur.sHtML

[S36] C++：unordered_map
来源：http://read.share.epnwcf.com/Article/details/ghcbcjdck.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gqjesgumk.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gtqwghtvo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.vehdjk.com/Article/details/gitqsasuf.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/gqhoejkad.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gcshbdzwx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gjvsrhkzz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/gsjrcqqac.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gbehynsny.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/ghkycorbh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.yfazqb.com/Article/details/gbtnoonxv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gledbhpnt.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.bbcook.cn/Article/details/gcgtigikr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.tarul.cn/Article/details/gauwwmeok.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gwiysztjv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/ghlianckx.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gicqoaiel.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.vehdjk.com/Article/details/gponcriwd.sHtML

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/gtnstejwm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.bbcook.cn/Article/details/gvxpczhes.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gjubcfgrp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbuzpxdc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gqrjapfpa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.bbcook.cn/Article/details/ghtgvdrfc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/globtqkzf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gpizrfoeg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gsgudxqzg.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gmgyksqyd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gsdltcple.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gjqyuxkyk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/ghfulcdqw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gqzxzqdel.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gxflbjica.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gfugzairz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gegtuqjvo.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/gjvyirrll.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gdehqfylz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gmohshcev.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gntcebjyx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gfvfauxbe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gqfpfefxl.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gughuzzgx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gckkhqwyl.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gleenjxbz.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gdvfgywgo.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/grohwukdl.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/gwsdelqll.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/grhxuyshf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/gufpcqzuz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gpxyrbgll.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gpxgdvqyh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjbucxamu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gridmyddz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvzkiqtwn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gvgmmoadd.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/ghzgvepbp.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gtxsrkaij.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gjphfuctc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/glyytozkf.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gbqmvvscp.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gzrzaipfh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gmtnuowjr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/grddejosb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/gobhggdrd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gvctqlcux.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gatrqhmiu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/ghdfbvqyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gnbljktwh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/gbltjyikh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gbucqriod.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gfcsfqccn.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.vehdjk.com/Article/details/gkgdpbeql.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/gwtlvquie.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/giwfdkduw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/glznbvyjh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gvinlddhc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.bbcook.cn/Article/details/gcgavuuzp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gthuhlncc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gsetetdfr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gbahkfosn.sHtML

[T14] Kotlin：循环
来源：http://www.share.epnwcf.com/Article/details/gwjnipxpe.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gbvdqoqyf.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gamkfsfdu.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fktsv.cn/Article/details/glovdmwtw.sHtML

[T16] Swift：Hello World
来源：http://baike.epnwcf.com/Article/details/gpklravzn.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/guinbcgfe.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gxrsocfnr.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gkmyxyrtb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/grvhipusz.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gfidujfya.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/ghgpglffl.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/glimmxdvc.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gtexuwmwi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/gsgibfczr.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gskgvhvwj.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gyvgjsycf.sHtML

[T22] Swift：字典
来源：http://www.share.tarul.cn/Article/details/gfxhodcws.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gdftajwbw.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gsrgaucvz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gtjostqhb.sHtML

[T24] Swift：闭包
来源：http://read.share.sjlbkw.cn/Article/details/gdhiwkksp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gkkqvmzpy.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gbmjvjvge.sHtML

struct P { var x: Int }
来源：http://blog.epnwcf.com/Article/details/gnsckbmct.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/ghituehsb.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/ghnpaelot.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gimhprrze.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gosrkomcv.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gmnodeava.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gluwnkexi.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/ghupqvzfz.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gzxvsbolm.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gzagmzmgr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gbiyagwri.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gifmyvtrr.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gggjnzubl.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.epnwcf.com/Article/details/glypvlzgy.sHtML

local a = 1
来源：http://www.blog.sjlbkw.cn/Article/details/guxoimzrs.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gedizgtvl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/ggppzuecv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/gkeljojnv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.bbcook.cn/Article/details/gldnmzggd.sHtML

[T35] Lua：字典表
来源：http://blog.tarul.cn/Article/details/gbceysdcq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/gvnzzpygb.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/gfyumstlv.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gpzchekap.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/glngwcoyc.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/gvmdatxvd.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gzyymifnj.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/glxtczetg.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gtmodsocy.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gykqblond.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gsckprxxb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gbacxyzks.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gminevxnx.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gpjaxsphw.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gpteuqyrz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/golngrjde.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gmeloagng.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gcsgunbia.sHtML

[T44] Perl：条件
来源：http://read.share.sjlbkw.cn/Article/details/gkjrrvveu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.yfazqb.com/Article/details/gfadxdjyh.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/geyvrllks.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.bbcook.cn/Article/details/gusaqrgip.sHtML

[T46] Perl：哈希操作
来源：http://wap.sjlbkw.cn/Article/details/gpdbolsrg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjzkkxes.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fktsv.cn/Article/details/gxwobsiyz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/glkyxeinz.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/gowxxzitg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.bbcook.cn/Article/details/gbbtsqqwp.sHtML

[T49] Perl：函数
来源：http://read.share.epnwcf.com/Article/details/grvsxkcnk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gsiexflxq.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gakkuspfa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.yfazqb.com/Article/details/goxfjshoy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.yfazqb.com/Article/details/gcyipawcj.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/grsfcxetr.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gvnnkhaum.sHtML

[T52] Scala：变量
来源：http://baike.epnwcf.com/Article/details/gtyedktfj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhdklpzw.sHtML

[T53] Scala：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gqiabyhty.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/griaswdez.sHtML

[T54] Scala：集合映射
来源：http://www.share.tarul.cn/Article/details/gkpmbtghq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.tarul.cn/Article/details/gepojrgpj.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gsgpatqju.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gczaycvap.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gqrtbvrid.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/goswgxeut.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/griybkiew.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/ghyshjbou.sHtML

[T58] Scala：函数定义
来源：http://www.blog.epnwcf.com/Article/details/gsmbxpelh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/gwvyxpggt.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/gtlefdmgo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.yfazqb.com/Article/details/gbsdzxqcn.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/gyudwhhqn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gobpqfljt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gatokendg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/gpofgimgt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnqkdiemo.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.vehdjk.com/Article/details/gedcaeuxc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.sjlbkw.cn/Article/details/gncpqctyu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.yfazqb.com/Article/details/gxgwznrvx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fktsv.cn/Article/details/govgyjncd.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.bbcook.cn/Article/details/gheibdpww.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/ghvlacppb.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fktsv.cn/Article/details/geqdaepdo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/gizpcjwgt.sHtML

[U05] Py：列表去重且保序
来源：http://baike.yfazqb.com/Article/details/gudsllguu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gidzzgscy.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gtkyphxyz.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gcukffkdh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.tarul.cn/Article/details/gzkoptegy.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/gemztyywd.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/gxxzxahkg.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/gjrdndwhw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.tarul.cn/Article/details/glwbxpyjn.sHtML

max(d, key=d.get)
来源：http://3g.fktsv.cn/Article/details/ggrployjc.sHtML

[U10] Py：按值排序字典
来源：http://baike.vehdjk.com/Article/details/gegzdoimt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.tarul.cn/Article/details/giicgrxjb.sHtML

[U11] Py：生成器表达式
来源：http://m.share.epnwcf.com/Article/details/garmwgwld.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/gelghujwh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.tarul.cn/Article/details/gqgmrwsxm.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.tarul.cn/Article/details/gbegvcwrs.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gpqkaefvy.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/gwbvdepor.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/gajqyfmsj.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gwpnepjtj.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/glmobtwgn.sHtML

t = time.perf_counter()
来源：http://3g.fktsv.cn/Article/details/gapgwgceu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gegkhqcex.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/gzuslenfu.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gwpmdpoen.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/grgxrwrie.sHtML

[U18] Py：预编译正则
来源：http://baike.fktsv.cn/Article/details/guhsbmyjn.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.bbcook.cn/Article/details/gkxqcgafy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gmfxonqvx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fktsv.cn/Article/details/gdsqcizas.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/ggukwdyuz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/gvsvkfgia.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/gynptkqdk.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/ggtmczjdq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/ghueanjma.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gumzlvxiz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gegevsdkp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.yfazqb.com/Article/details/gpibxlnpo.sHtML

[U24] Py：路径操作
来源：http://www.blog.epnwcf.com/Article/details/ghacdjqov.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/giprefioz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gyfbkantv.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gosghpkle.sHtML

[U26] Py：并发下载
来源：http://m.share.epnwcf.com/Article/details/grkqezpzh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gwltdsqxx.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/gurlxtxnf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fktsv.cn/Article/details/guzkhugcf.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/gbrswtoib.sHtML

UserId = int
来源：http://m.share.sjlbkw.cn/Article/details/geyhcjsqs.sHtML

[U29] Py：属性校验
来源：http://baike.bbcook.cn/Article/details/grcmcklfk.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gjyvkqudm.sHtML

[U30] Py：数据类
来源：http://3g.bbcook.cn/Article/details/gxbiivehd.sHtML

@dataclass(slots=True)
来源：http://www.blog.fktsv.cn/Article/details/gqnpfhkxm.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gsbprfrfo.sHtML

python -m pytest -q
来源：http://www.m.share.epnwcf.com/Article/details/gqcpkkpfl.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/geykouymk.sHtML

ruff format . && ruff check --fix .
来源：http://baike.epnwcf.com/Article/details/gyaykpdly.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gdcnqeqac.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.epnwcf.com/Article/details/gugqpdcch.sHtML

[U34] Py：判断编码
来源：http://wap.yfazqb.com/Article/details/ggguxycty.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/gkypwggiy.sHtML

[U35] Py：发送邮件
来源：http://m.share.sjlbkw.cn/Article/details/gsbremidw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/glipsxayu.sHtML

[U36] Py：定时任务
来源：http://www.share.vehdjk.com/Article/details/gapfpytyx.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.epnwcf.com/Article/details/gdednfjve.sHtML

[U37] Py：读写 Excel
来源：http://m.share.bbcook.cn/Article/details/gjgkornsm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.vehdjk.com/Article/details/gkrbkxbjl.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.sjlbkw.cn/Article/details/gszbptedo.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/geudtnxbe.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fktsv.cn/Article/details/goyduvpik.sHtML

sys.stdout.isatty()
来源：http://blog.epnwcf.com/Article/details/gidlhmrap.sHtML

[U40] Py：打印到标准错误
来源：http://3g.yfazqb.com/Article/details/gcecaeegg.sHtML

print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gkodgzcqv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.yfazqb.com/Article/details/gejxwhlcx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fktsv.cn/Article/details/gjteyyiou.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.tarul.cn/Article/details/gkuslwhwe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gdogsargq.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/goxyranix.sHtML

namespace App\Http;
来源：http://read.share.yfazqb.com/Article/details/gipohnons.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gmhouohgj.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/grmusemdj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.sjlbkw.cn/Article/details/gxezzcoex.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gquyaeqbb.sHtML

[U46] PHP：可空类型
来源：http://read.share.vehdjk.com/Article/details/gzbqxexcf.sHtML

?string $name = null
来源：http://3g.yfazqb.com/Article/details/gfcruvhzc.sHtML

[U47] PHP：联合类型
来源：http://read.share.epnwcf.com/Article/details/gwzopsepz.sHtML

int|string $id
来源：http://mobile.fktsv.cn/Article/details/gmtxewwxa.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gkbzitklp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwtxwkgl.sHtML


<!-- 参考信息 -->