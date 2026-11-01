代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gwjkzamhq.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gtbwhtwqv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gcagzlyjm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gchquyahy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gvgaluuec.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/ggwoocovp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gkmqktyzf.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gweqsinod.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/goegwpuyu.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gjfsyxpdu.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/gbxsysfsl.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/guksrrlvp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gytfshjyq.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gebkynank.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gtbkxvqtc.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gtohvalwk.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gcemwwrzj.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gnqnyehlk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/gcwstjgay.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gvwyyucod.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/ggjsscxql.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/giitiljxl.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/gpynjkzfi.sHtML

[S31] C++：Hello World
来源：http://read.share.bbcook.cn/Article/details/gaugmztca.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gtzpnbeux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtxepurgt.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/gevdtuzhv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/ghqbnibbl.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/guaktveio.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gymmbnbry.sHtML

[S34] C++：遍历 vector
来源：http://3g.yfazqb.com/Article/details/golynfvul.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/gtckgnkuj.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/gsinbjgqf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gevbrjqtb.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/ggwthloru.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/guwftoubo.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gibhirhrz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/gosujmenz.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/gddgueots.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/ghdxlxvdz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/garlbblmr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/glipbkegx.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gmalyyhqv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/ggbyywgwt.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gzuzgqjpy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gxsgabhac.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gllciovid.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.epnwcf.com/Article/details/gmelyajrb.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gfrnizfzf.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gdqzvoaiq.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/ghttymbok.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gfuwdrpyb.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/gsyrggtoe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/guzjzrhnc.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gggiflocf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gnttazywx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gpldusrak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.yfazqb.com/Article/details/gvjwfjhik.sHtML

[S48] C++：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gdqyjutmh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gabvcshzr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gjmjghxai.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/gexalwopy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gxvzywhpe.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gmgwrdfgp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gluqxczga.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gjdcycrce.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/gpnccjxat.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/ghwsfgsea.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gwngpducj.sHtML

[S53] C++：移动语义
来源：http://baike.bbcook.cn/Article/details/gwmbvkpue.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/gpzdphgvc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/geasyngwh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gbogbxsjj.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gnyikxypn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gjoxxakqs.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gojondhec.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/gyiieufjy.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/gevbhbjsi.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gkqlbwloj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/grbnazosg.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gmhzmkfhm.sHtML

[S59] C++：静态断言
来源：http://www.share.fktsv.cn/Article/details/ghiducvme.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gihvxapcx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gsbgnkztb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gxrxzthaz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqfseatfg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gxdiduoop.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gschajdcw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fktsv.cn/Article/details/gmlgvfczd.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/guiffadrh.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gbiupyehg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/ggpkmzffo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/ghfbbizmy.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gmsamwcki.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gqwriyiyc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gslhhvdwh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gknioahxd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gchpjmjrm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gytrpcjtp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gbxniqlry.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/guhsslerq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gomigcojz.sHtML

[T08] Kotlin：数据类
来源：http://blog.yfazqb.com/Article/details/gnikpezlc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.bbcook.cn/Article/details/gubhxyuur.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gytrgwxdx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/gaeyeozyo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/geunfykic.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/grrbnvffy.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.yfazqb.com/Article/details/gevyqndhx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gvlrsbuqg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gfccjtbor.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/geceazali.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/graobpbwk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gudowsbvw.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gxbfldxet.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/ggfvofngo.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gjcttehaz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/ghsmnruje.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gjhriesdl.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gkrrhogrz.sHtML

[T17] Swift：变量与常量
来源：http://blog.sjlbkw.cn/Article/details/gphpxmpac.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/gvxfidekg.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/ghdhkwgcz.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/gojuvnxmo.sHtML

[T19] Swift：可选绑定
来源：http://mobile.sjlbkw.cn/Article/details/guqnxwxcf.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gchgbroel.sHtML

[T20] Swift：数组操作
来源：http://read.share.tarul.cn/Article/details/gtcwxtutk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fktsv.cn/Article/details/gbkamgqhm.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gbdcdpcaj.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/grmniuqbb.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/gqhhhnwbs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/gaewephmy.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gjfyppmkk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.bbcook.cn/Article/details/gazpnmbei.sHtML

[T24] Swift：闭包
来源：http://mobile.sjlbkw.cn/Article/details/glohgegia.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gfeaebccw.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gugdnedif.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/gwtropecu.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gsnfvksun.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gxszlafyl.sHtML

[T27] Swift：错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gbawxuzpy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.tarul.cn/Article/details/gdkqzggvm.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/gdrovatzo.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gmzmiuyvd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjstumqp.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gmsqtwczx.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/gooswagnp.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gxjusekvt.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/gtsudetbv.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/ggezybltn.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/guewppfxu.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gkzosjjeq.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gbkpgxhyc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/gzmrtgmdu.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gkqnsckat.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.bbcook.cn/Article/details/gnhrnznyl.sHtML

[T35] Lua：字典表
来源：http://wap.bbcook.cn/Article/details/gozufctjn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gwrgknvhd.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gfyouwljw.sHtML

function add(a, b) return a + b end
来源：http://baike.bbcook.cn/Article/details/gzpkrsjql.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gztgbasis.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gdnkudnes.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gucdbgwgn.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gjjdhifwt.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gxhlsmvyd.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/ggxsjhwbw.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gsawodgqd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/ghexhfyyi.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gzturebtl.sHtML

print "Hello\n";
来源：http://www.m.share.epnwcf.com/Article/details/gwdkejyga.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/ghgfolkiw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/gzsunwcua.sHtML

[T43] Perl：字符串插值
来源：http://3g.fktsv.cn/Article/details/gvnazsnlf.sHtML

"值: $a"
来源：http://www.m.share.vehdjk.com/Article/details/grhqpeozc.sHtML

[T44] Perl：条件
来源：http://www.share.yfazqb.com/Article/details/gjwsusqgn.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.epnwcf.com/Article/details/gvkxooqzc.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gglfacfxb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/gbznxbwmo.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/gpavdghtn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gibcilqbt.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gwpgpaztp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gbkeazxkt.sHtML

[T48] Perl：正则替换
来源：http://3g.epnwcf.com/Article/details/gumgmifxt.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gzzeppgwc.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/gsjsmmuhk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gbgpzjshe.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gkmjsveyr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gqbdxduoo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/ggujvksmx.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/ggebrmubw.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gllaqulhz.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/ghhdrlzeq.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/glramlkft.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gsfikokzc.sHtML

s"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gvmoserzn.sHtML

[T54] Scala：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gpwosbqbc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gdbrmpkwc.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gsytqiybz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/graurpvpm.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gmujcxuqh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gjpdtupaq.sHtML

[T57] Scala：模式匹配
来源：http://baike.bbcook.cn/Article/details/garmfwifj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/glespvbjg.sHtML

[T58] Scala：函数定义
来源：http://mobile.bbcook.cn/Article/details/gqzugxqfc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gedaryfct.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gshshrmyc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.yfazqb.com/Article/details/giyrovvjb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gesczzvaw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gnoabhhel.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpkxkuudr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gqdwxvjqd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/geexkjipt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/gzlgafndz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.sjlbkw.cn/Article/details/ghjvprrft.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.tarul.cn/Article/details/gwxwgyizm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fktsv.cn/Article/details/gjurtfbqx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gqhtqjprp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.tarul.cn/Article/details/gsgbfpryn.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gtatdkuqo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/glzmoxvvi.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gywdoqqlj.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gyhhhcfmk.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gekvmszxp.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/gbehowqvs.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gjctknabn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gltwlzewp.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gmplngogt.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gcnuomiev.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.yfazqb.com/Article/details/gdfkjgyqx.sHtML

max(d, key=d.get)
来源：http://www.share.yfazqb.com/Article/details/gnyxcnlda.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/gajgfcpek.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/gcqdlizpo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/gktruhmgz.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gmzbxugis.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fktsv.cn/Article/details/gtxmanlkp.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/gqratupip.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/gsnrqbeqe.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gymttkryq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.yfazqb.com/Article/details/gwlbieyqp.sHtML

defaultdict(list)
来源：http://wap.sjlbkw.cn/Article/details/glenjauzm.sHtML

[U15] Py：高精度计时
来源：http://3g.epnwcf.com/Article/details/gohptqccf.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gjrfeudwy.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/grmhnegtk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/goiuierbt.sHtML

[U17] Py：初始化日志
来源：http://www.share.epnwcf.com/Article/details/gddowqhfs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.sjlbkw.cn/Article/details/gvvhfjhsl.sHtML

[U18] Py：预编译正则
来源：http://wap.epnwcf.com/Article/details/gockdgrnq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.bbcook.cn/Article/details/gocibzuue.sHtML

[U19] Py：正则替换带回调
来源：http://blog.vehdjk.com/Article/details/gfbxpxvqo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gubgscfnt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.sjlbkw.cn/Article/details/gjabsvqym.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gkaeulyti.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.vehdjk.com/Article/details/gqfibliym.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fktsv.cn/Article/details/gnvmqdmah.sHtML

[U22] Py：矩阵转置
来源：http://wap.yfazqb.com/Article/details/gtsyvzlyb.sHtML

list(zip(*m))
来源：http://www.m.share.vehdjk.com/Article/details/geyipxbgr.sHtML

[U23] Py：分块读取大文件
来源：http://wap.vehdjk.com/Article/details/gvvwcpfvf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gztuxxjka.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/goukcuehi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gpewlkzcs.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.epnwcf.com/Article/details/ggvsmwagf.sHtML

csv.DictReader(f)
来源：http://www.share.epnwcf.com/Article/details/gcyfdnpsh.sHtML

[U26] Py：并发下载
来源：http://blog.vehdjk.com/Article/details/gapwsjetq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gslsqrzal.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.tarul.cn/Article/details/gyncibsok.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fktsv.cn/Article/details/gbunyozvp.sHtML

[U28] Py：类型别名
来源：http://baike.sjlbkw.cn/Article/details/gpvisezdb.sHtML

UserId = int
来源：http://read.share.sjlbkw.cn/Article/details/gwdgafqyr.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gmxazbmkb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.vehdjk.com/Article/details/gfpwkxuoa.sHtML

[U30] Py：数据类
来源：http://read.share.fktsv.cn/Article/details/glebalrfb.sHtML

@dataclass(slots=True)
来源：http://m.share.yfazqb.com/Article/details/gbwfgaxij.sHtML

[U31] Py：单测
来源：http://wap.epnwcf.com/Article/details/gyqzqmrra.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gmnfohioo.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fktsv.cn/Article/details/glpaqagao.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.vehdjk.com/Article/details/gckzyylpj.sHtML

[U33] Py：打包发布
来源：http://www.share.vehdjk.com/Article/details/gveeppnzw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gkkcsfxun.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gxkfqbkah.sHtML

chardet.detect(raw)
来源：http://read.share.sjlbkw.cn/Article/details/gcmqdnroh.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/gmhyoehni.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/girmqizoi.sHtML

[U36] Py：定时任务
来源：http://www.blog.fktsv.cn/Article/details/gisollhca.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.vehdjk.com/Article/details/gxggukjcx.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gbkmxyabi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fktsv.cn/Article/details/grnmekyfq.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gvqcpcsnz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.tarul.cn/Article/details/grzflzckm.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.tarul.cn/Article/details/gfbuldfyj.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/gechowjve.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.bbcook.cn/Article/details/glhkhpzao.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gfoggkool.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.sjlbkw.cn/Article/details/ghhqdbuin.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.epnwcf.com/Article/details/gcfyzduug.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.sjlbkw.cn/Article/details/gynmsuzem.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.yfazqb.com/Article/details/gwusgtzhp.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gcpogekky.sHtML

namespace App\Http;
来源：http://read.share.yfazqb.com/Article/details/gooxsnlvu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/gesjszrjj.sHtML

declare(strict_types=1);
来源：http://wap.vehdjk.com/Article/details/grdspdinl.sHtML


<!-- 参考信息 -->