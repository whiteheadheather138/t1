代发 wailian999

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gjocygoaw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gpofulpjn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gfbijigle.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/gxxgexgmn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.bbcook.cn/Article/details/gbmuhflzj.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/grrqygqwa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gduuxyvwa.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gfcjupbyj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gbepofrwo.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gciijcxzn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gaoafedee.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gfvfysstn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gdnqcdmea.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gdymjgspr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gskpsvdus.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/geaixzpxy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gackeksxf.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gvfjgwbbq.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gydzntscm.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gyaxhvutm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gxxnqjoqp.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/gvnbsbboy.sHtML

const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gozbnrvgy.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/ghfeyefhp.sHtML

static int counter = 0;
来源：http://www.blog.vehdjk.com/Article/details/gbjsznrht.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/guykwaccm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/gpzimbpon.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gtkfamelg.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/giwocaooh.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gisnqwwtr.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gyjfteooo.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gojqhgpkj.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/gypcyosag.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gkzpwpnwm.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/grletgekr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gtsfyeplj.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gjirlwmzz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/grvvruguq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gompkwqxz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gosvhtvsu.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gzrbuouqx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gmduqqdzs.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gtezbcthe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gukzixhux.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/ggrehwydr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fktsv.cn/Article/details/gbefxqzlu.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gbrphbugf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fktsv.cn/Article/details/ghdiickkl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.vehdjk.com/Article/details/glifncazv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gihvzurgc.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/gqdkiuzic.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/gqwvangrm.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gpkqdvbwe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gjizeehyu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gktahlqxa.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gghdnuxwx.sHtML

[S43] C++：智能指针
来源：http://3g.vehdjk.com/Article/details/galirshdw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/gnubxpesp.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/goftwzftb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gqpfatcpc.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gcptennxt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/gnjloelcz.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gktxpwpuu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gfddpvizp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gucpcryvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/grqpsmmef.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gzbjdudir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/ggsdwrqdm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/gmbnicmmo.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/ghkjrctpq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gyxcinpvl.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gwhmzoigf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gxeglxxbr.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gymfxybtn.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gbepzbyhx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/glfvzqgjx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gqffwqymy.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/gdfivlyak.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/goimjthoe.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gmkngagyv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gphdlpttd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gbnidqvuq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gzhdkdwxk.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/goyjnpsnf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gypfsdwcs.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gtnufdcai.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/grpmviabm.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gfpovdbiz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/gmvouiypz.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gqyjtbwoa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gxqgtuxup.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gsbgzjarp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/gcbtlkxqa.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/givcvpnji.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gvquhoujy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfnpccpwn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gnbkqrclp.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/ggbcfyqbb.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gotouxesq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gduyvhhbx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gdzmotvjs.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gcoacpyfs.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/giavtybaa.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/guwouyvsq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gpusbtdle.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.sjlbkw.cn/Article/details/gruuiobgl.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/ggtwrwyyu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gragboizs.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gdoufbqcu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gyxevvmzd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gqjfpiawc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/govrwcoep.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/glaglygig.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/ghncganeg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/ggnehzayf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gvxlxziel.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gxobitzbg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/grmgxtubt.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gyfdvpegw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gbnuadsrx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gzjbgizpy.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiieeuyj.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gyqvysbza.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gcswzwyrd.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gvfkeqktp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gsultniej.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gxxegumgv.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gzeshlwet.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gfbkyykro.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gxzhqmdku.sHtML

[T18] Swift：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gqkuoktrn.sHtML

"值: \(b)"
来源：http://blog.tarul.cn/Article/details/gmskoyvtx.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/grugavymc.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/ghjnqogrp.sHtML

[T20] Swift：数组操作
来源：http://blog.tarul.cn/Article/details/gnqbvcwac.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.vehdjk.com/Article/details/gldwgfrll.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gqgebbwwy.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gnciasuxy.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gtwwfhnjt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/golrjsrry.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gwqppwgvl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/gwskepahn.sHtML

[T24] Swift：闭包
来源：http://www.blog.tarul.cn/Article/details/glhvjjlza.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gmhqqideg.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gyzryyncj.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/gvmnuntjh.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/glyxyqjpt.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/ggmtfiept.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gelrrqmii.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/giguwenae.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gvbshefws.sHtML

enum Color { case red, green }
来源：http://mobile.fktsv.cn/Article/details/ghpajtemx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/gvhctdbiz.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/ghpangvex.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gvzvyzxbf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.tarul.cn/Article/details/gmxtowhha.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gaipoaqid.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gjuiyptxe.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gqnosfifq.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/gwnzqrvcl.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/glhjwdmcz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gbiugpkup.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gszuactnm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/gnksezbmh.sHtML

[T35] Lua：字典表
来源：http://3g.vehdjk.com/Article/details/gowsyyqjg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gqnzkescj.sHtML

[T36] Lua：函数
来源：http://3g.bbcook.cn/Article/details/glwkautiz.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/gmvpmypjg.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gvqxzlhxq.sHtML

"a" .. "b"
来源：http://wap.sjlbkw.cn/Article/details/gpitsazru.sHtML

[T38] Lua：条件
来源：http://www.blog.tarul.cn/Article/details/gqhnonfku.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/gfjrecnav.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gzcazdjeq.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gzqewnjfm.sHtML

[T40] Lua：元表
来源：http://www.m.share.vehdjk.com/Article/details/gniuruelc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.bbcook.cn/Article/details/gzpebijni.sHtML

[T41] Perl：Hello World
来源：http://mobile.epnwcf.com/Article/details/guvumvfex.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gnbglnmxb.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gdhpvrbse.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/gtuvpgakm.sHtML

[T43] Perl：字符串插值
来源：http://blog.bbcook.cn/Article/details/gahnlowpr.sHtML

"值: $a"
来源：http://www.blog.epnwcf.com/Article/details/gtcusuplk.sHtML

[T44] Perl：条件
来源：http://blog.yfazqb.com/Article/details/gvdnwojay.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gwjlayfkr.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gzjksggge.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/gvzkhbuun.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gmfdbxqpm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gvyrmqgxt.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/gttrsiuhm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gcrsmeuvh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gwbsgbsla.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gzurlnjbd.sHtML

[T49] Perl：函数
来源：http://3g.bbcook.cn/Article/details/gcruukllv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/geilofqkd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/ggjfqbbqh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gtbzqcbpx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gttterxia.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gypiuespf.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gnhoycbyi.sHtML

[T52] Scala：变量
来源：http://www.share.fktsv.cn/Article/details/gowfknrtu.sHtML

val a = 1;  var b = 2
来源：http://read.share.fktsv.cn/Article/details/gahjzhksh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gajqjbijj.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gcwqgglgq.sHtML

[T54] Scala：集合映射
来源：http://m.share.yfazqb.com/Article/details/gpnyoxgtl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/gpmmekbsu.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/gdnycnkts.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gybluehtb.sHtML

[T56] Scala：样例类
来源：http://blog.vehdjk.com/Article/details/gwykkfczl.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/gdikhqney.sHtML

[T57] Scala：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gkhtwmckm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gyhrxsxet.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gqeswjiay.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.bbcook.cn/Article/details/gsmlgblbq.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/ggcvubofq.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.bbcook.cn/Article/details/gabbgytac.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gpkkbboez.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/gtwdjxaaz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtuenorcg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/glrtznipa.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfqwdydmo.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fktsv.cn/Article/details/gsqfkkszx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gxgkhfjbr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.yfazqb.com/Article/details/glsqyqxxm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/gnfttzxyu.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gaopgqrrm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/gmzrkqgfx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.yfazqb.com/Article/details/golljagrf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gpzdcwbst.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gavbumdrq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gzrzrxjkq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/gmazllfxc.sHtML

{**a, **b}
来源：http://baike.bbcook.cn/Article/details/gejzmrwlc.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/gcfkouipd.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.bbcook.cn/Article/details/gxhqpmhbp.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gushhnojn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/gdmavexpd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.sjlbkw.cn/Article/details/gkgqanhjq.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gqblhfzlm.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gobolvwaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fktsv.cn/Article/details/gusyojwkk.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/gchlsjtgc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gxkhfoygc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gzkqdyxuo.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fktsv.cn/Article/details/gvqqbpcpf.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/gofanmlms.sHtML

deque(maxlen=10)
来源：http://www.share.yfazqb.com/Article/details/gfgksihxj.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gfsewzagn.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/gzppgbend.sHtML

[U15] Py：高精度计时
来源：http://baike.fktsv.cn/Article/details/gwwsjuljb.sHtML

t = time.perf_counter()
来源：http://www.blog.fktsv.cn/Article/details/ghisybxxb.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gqfatmxmy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/glqoojldb.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/gbeexivcn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.epnwcf.com/Article/details/glydjjuqx.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gkqxnukmm.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.yfazqb.com/Article/details/gakfsyact.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/genxbimug.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.yfazqb.com/Article/details/gvxixwtbt.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gpuvyyexj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.bbcook.cn/Article/details/gdncxdxqx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.epnwcf.com/Article/details/ggvvlripb.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/gcibagatd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/gntxkuuqy.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/glzohazxz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gdkudnfks.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.epnwcf.com/Article/details/gmnjgvlyl.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gkihzfhte.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gbaogtvpv.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.yfazqb.com/Article/details/gyxchfsnz.sHtML

csv.DictReader(f)
来源：http://wap.epnwcf.com/Article/details/gwkmjmlkx.sHtML

[U26] Py：并发下载
来源：http://www.share.tarul.cn/Article/details/gnvdgtkjm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/gspymevtv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/gxdabndxs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/gmzaxfvtq.sHtML

[U28] Py：类型别名
来源：http://www.blog.vehdjk.com/Article/details/gyonlqwfw.sHtML

UserId = int
来源：http://blog.fktsv.cn/Article/details/gzojxrboy.sHtML

[U29] Py：属性校验
来源：http://baike.bbcook.cn/Article/details/gjxrtxwbs.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/ggenbmlis.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gywrujxdw.sHtML

@dataclass(slots=True)
来源：http://blog.bbcook.cn/Article/details/gsxcdeyoj.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/gzzzzehjx.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/gfnxjoxby.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/gbaqqdnyf.sHtML

ruff format . && ruff check --fix .
来源：http://baike.epnwcf.com/Article/details/gudetjqxz.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gbfgurdqo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gzvdvavgv.sHtML

[U34] Py：判断编码
来源：http://blog.sjlbkw.cn/Article/details/gywbrtput.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/ginxaetrn.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/ggyyifihg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.sjlbkw.cn/Article/details/gkquzjdfx.sHtML

[U36] Py：定时任务
来源：http://blog.epnwcf.com/Article/details/gkjdkdoqe.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.yfazqb.com/Article/details/grcevckqd.sHtML

[U37] Py：读写 Excel
来源：http://www.share.tarul.cn/Article/details/gsfdjbfhv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.tarul.cn/Article/details/gskgnlixg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gzprpdlgt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gfmbhbesw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.epnwcf.com/Article/details/gzifzwjxp.sHtML

sys.stdout.isatty()
来源：http://3g.vehdjk.com/Article/details/gqnpgmqoy.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/gvtscgnji.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gzwxhfacm.sHtML


<!-- 参考信息 -->