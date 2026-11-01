代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gpjjdzvxz.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gckseauwq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gknratyvt.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gipqffiwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/gakhjxvrq.sHtML

[S25] C：内存拷贝
来源：http://blog.fktsv.cn/Article/details/gikdxkmxu.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gckxqkopt.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/ghnkfwakv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/guhufvxwl.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gussuyemc.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gpgxjatme.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/gvvdyqbuo.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/gxsoilmlo.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gxyalixqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.vehdjk.com/Article/details/gnglmpfym.sHtML

[S30] C：头文件保护
来源：http://baike.bbcook.cn/Article/details/gezdwnyje.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gpxgqiwny.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gqxhwrdav.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/glpwbapwi.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gtbywrclu.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gfkaozbxv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gqyctzimu.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gkdyatigv.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/ghbcchhhk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.bbcook.cn/Article/details/gpztgwvlp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/ggetjicnj.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gmoyimroo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/geuoteirw.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/glpzqohkb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gpdlbsdpw.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gxyhpzwsv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gzzjdvgrx.sHtML

[S37] C++：set
来源：http://baike.vehdjk.com/Article/details/gtisfepis.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gkzyhvnlo.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gvlsgnupk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gcbyyapzm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gfqwncsjy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/glcxppmvq.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/gehtzphbm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gjlnkkrqg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdzopnab.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gyibinbhn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gihfunadp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gqexckioq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/grbxjczpq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gnjezanbq.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/gmploftmk.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gbvnebwhl.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/grzdncins.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gffydhxfp.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/giswdetzq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gsapmlbft.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/gggnemnxp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gjxmoxpfh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/goqfcmjkm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/ggaguuvgz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gnyonwjey.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/gdgojysru.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gehxsiwew.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/gctqqyyhx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gxjapzuoi.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gejjhyxrb.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/grzojazrc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gjgsoruvj.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/glilzxhqo.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gdwwybaff.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gkmwaqssq.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gvqumgrjq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/gucusyzlq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/gytcolpyi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gyyfjyxbp.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gdhsafqbp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gvtylfxmh.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/glsrtcgaf.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/gnhpuvpkf.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gjzeeezow.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gssmabnkj.sHtML

[S59] C++：静态断言
来源：http://baike.fktsv.cn/Article/details/gmwpdbejg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqftruuq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/gazdruuqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gbfisyxdn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gotgsyehq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gskcwsmqx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtlgjhvtt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/gnzdtycgc.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gfkyqdjxy.sHtML

[T02] Kotlin：变量
来源：http://read.share.sjlbkw.cn/Article/details/goabiyeah.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gozdanypq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/grwegnmzn.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gschvljxu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/grfwgxtpd.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gtlbvkpva.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gobfrjksm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/grttccwew.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gdlbgcmjy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gndsqexij.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.tarul.cn/Article/details/gxqpmeqxd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/gakevkzpr.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gfuwxgalt.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gwnnmnqmn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/gymigsmzc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fktsv.cn/Article/details/gqtdxxqlu.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/geqdxzypq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/grxispvxk.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/goilzsbhi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gwdczeesj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/gzhnafsyd.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gbnqkbstv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gnrehddzu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.sjlbkw.cn/Article/details/gcrxcojla.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/galoeotmc.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggciefvkq.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/gzysudcyw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gvnpapdzc.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gyxjhiaqh.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gtcrdrskg.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/goeuabeps.sHtML

var a = 1;  let b = 2
来源：http://baike.bbcook.cn/Article/details/gppmrwsdn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gwahczvmo.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/giraduexa.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gluqlmnjk.sHtML

if let n = opt { print(n) }
来源：http://www.share.sjlbkw.cn/Article/details/gcgczkpew.sHtML

[T20] Swift：数组操作
来源：http://m.share.tarul.cn/Article/details/gjkwvxkbl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.yfazqb.com/Article/details/gztdadxyz.sHtML

[T21] Swift：遍历
来源：http://www.blog.fktsv.cn/Article/details/gfhfkmpjh.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/gjwhxasqg.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/gtlteperv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/gkqlamuqp.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/gklvkncjy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/gzamryjvi.sHtML

[T24] Swift：闭包
来源：http://3g.epnwcf.com/Article/details/gkczwjald.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gvnlqkylg.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/gofqbnrps.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gaqqfytls.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gfcyeopne.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/gvakrxpjk.sHtML

[T27] Swift：错误处理
来源：http://wap.bbcook.cn/Article/details/gtyvhnbrh.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/galfoaduz.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gisligubm.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/glarweuey.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/ginncffio.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gdurbgbgr.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gplzphdsx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fktsv.cn/Article/details/goalodgej.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gilfyuxdr.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gioboxghi.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gdwdimpgj.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gpcmshtoh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gmpffwybc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.sjlbkw.cn/Article/details/grrbutfiu.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/giapubptl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/gqdbyxvca.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/gollrjumx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gybrzjxrm.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gsuxpfykz.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/gvsmbzogw.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gkqnujecv.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gzhshvwtg.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/ggclsrirz.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/gmcmvwvou.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gumuzsosb.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/govsnhqms.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gxlezxaxr.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gwsyldzvw.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gqdmqncwq.sHtML

print "Hello\n";
来源：http://www.share.yfazqb.com/Article/details/gjxpswezv.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/giqfrrgvy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fktsv.cn/Article/details/ghlvkvjab.sHtML

[T43] Perl：字符串插值
来源：http://3g.tarul.cn/Article/details/gflznmstx.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/gkbsscoqi.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gctrvydpl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.sjlbkw.cn/Article/details/gigbcamkt.sHtML

[T45] Perl：数组遍历
来源：http://wap.fktsv.cn/Article/details/gwsqpyygm.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.sjlbkw.cn/Article/details/gdkjysrzh.sHtML

[T46] Perl：哈希操作
来源：http://blog.tarul.cn/Article/details/gsumxodkn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.epnwcf.com/Article/details/ghqdwfyea.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/gtnhsajyp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.tarul.cn/Article/details/gcawsvykz.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/ggdxlgexx.sHtML

$s =~ s/old/new/g;
来源：http://baike.yfazqb.com/Article/details/gcnbclqkw.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/gpzvghbnx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gupqocoly.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gxfoxovpd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.yfazqb.com/Article/details/gygjaefjq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/gjtexsjuv.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gdoyfktau.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gncdjpafy.sHtML

[T52] Scala：变量
来源：http://read.share.tarul.cn/Article/details/gkeouidln.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gurhffopf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gcomnrtxb.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/gcsozlwmm.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gqawypuqi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fktsv.cn/Article/details/goqjuiwps.sHtML

[T55] Scala：集合过滤
来源：http://3g.fktsv.cn/Article/details/gyzqrlvom.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gxwueahji.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gtlhfmmuw.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gtrmeztxf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/gncqgxxmp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gxgvgxejm.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/gnlprorsy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gwomrppwh.sHtML

[T59] Scala：循环
来源：http://www.m.share.fktsv.cn/Article/details/gvvrqsbhy.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/ghdaratay.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/ghsphhbgb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/guwiwbvwm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxrklulsf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/gxrldvohn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtjtgbehi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/gqpmlbufb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gpfzhjtpv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/gknoagywt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gtrdzirid.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gthquhjmw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/gtkozqpqr.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gcpvguuiv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/gsirjhmvw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gdcctfgdv.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gcrsahxgt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fktsv.cn/Article/details/gcuimncmd.sHtML

{**a, **b}
来源：http://wap.sjlbkw.cn/Article/details/gujtfwoun.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gpcyjieyk.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gcmqtvxly.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/gtvnqzxsr.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gmlklmqzi.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.tarul.cn/Article/details/gwrcdbrbj.sHtML

max(d, key=d.get)
来源：http://baike.tarul.cn/Article/details/gyudmfpwp.sHtML

[U10] Py：按值排序字典
来源：http://m.share.tarul.cn/Article/details/ghckpwbqi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gedijqqww.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/givlenjla.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/gyndwzezj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gsswzrdlq.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gfowxleyh.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gjsrvulwv.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gmwyuujhw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/grxzedair.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gxyedvzdt.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/ghvrndzvc.sHtML

t = time.perf_counter()
来源：http://www.m.share.epnwcf.com/Article/details/gaubevawj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.epnwcf.com/Article/details/gvnzyokdg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.tarul.cn/Article/details/gsuyhywpu.sHtML

[U17] Py：初始化日志
来源：http://3g.sjlbkw.cn/Article/details/gosspzmug.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gbysxdmno.sHtML

[U18] Py：预编译正则
来源：http://www.blog.sjlbkw.cn/Article/details/gajmukrdx.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/gcyervdqw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/gonphxpub.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fktsv.cn/Article/details/ggslpwqic.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gkjphkjis.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/gukvdbaqa.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.epnwcf.com/Article/details/gtzbkbfkg.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gpwvypopp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/gpbojcfpk.sHtML

list(zip(*m))
来源：http://wap.yfazqb.com/Article/details/gvhxjscdy.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/ghpxkzjke.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.tarul.cn/Article/details/gwlhnqbql.sHtML

[U24] Py：路径操作
来源：http://3g.yfazqb.com/Article/details/gaeojghuh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gdrqgrlum.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.tarul.cn/Article/details/gpdnrmsxs.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/gckjmkyyn.sHtML

[U26] Py：并发下载
来源：http://www.m.share.tarul.cn/Article/details/gxsoaqanz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.sjlbkw.cn/Article/details/gpfucbdbk.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/gndzljbbp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.yfazqb.com/Article/details/ganixfkvv.sHtML

[U28] Py：类型别名
来源：http://m.share.tarul.cn/Article/details/gdmmfkxwc.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gtzsgwjto.sHtML

[U29] Py：属性校验
来源：http://mobile.bbcook.cn/Article/details/glqglxuxh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/gcrquhgvr.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/gfbxyeoqc.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/glbzgsdxb.sHtML

[U31] Py：单测
来源：http://m.share.bbcook.cn/Article/details/gybjxknmz.sHtML

python -m pytest -q
来源：http://wap.sjlbkw.cn/Article/details/gmihblnpo.sHtML

[U32] Py：代码格式化
来源：http://read.share.vehdjk.com/Article/details/gyzuousnw.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/gnvbxtwnx.sHtML

[U33] Py：打包发布
来源：http://mobile.sjlbkw.cn/Article/details/gdboizssb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.epnwcf.com/Article/details/gpmokvipf.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/gnyqdtfoj.sHtML

chardet.detect(raw)
来源：http://read.share.epnwcf.com/Article/details/glnkhogdj.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/glxxzrcvi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.sjlbkw.cn/Article/details/gxmuperfo.sHtML

[U36] Py：定时任务
来源：http://blog.yfazqb.com/Article/details/gxarwewvn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gfsoqerxa.sHtML

[U37] Py：读写 Excel
来源：http://3g.sjlbkw.cn/Article/details/gryyowvmw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.epnwcf.com/Article/details/gxhkfocgl.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.tarul.cn/Article/details/gxpabuppc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.sjlbkw.cn/Article/details/gxnxykabk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/guqxfievq.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/gdnwffyey.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fktsv.cn/Article/details/gcufxxmsh.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/glbvfpccs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/grozvcwjn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.yfazqb.com/Article/details/gxgkkaxvz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.tarul.cn/Article/details/gcwrdwnac.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.epnwcf.com/Article/details/gqtrukstq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.epnwcf.com/Article/details/gmgzqvljv.sHtML

namespace App\Http;
来源：http://read.share.bbcook.cn/Article/details/gnlfhdfbt.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.epnwcf.com/Article/details/gijhqngue.sHtML

declare(strict_types=1);
来源：http://read.share.sjlbkw.cn/Article/details/gfagzrzsa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/gjnauwdul.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gendgvbgq.sHtML

[U46] PHP：可空类型
来源：http://www.share.vehdjk.com/Article/details/gmzralajr.sHtML

?string $name = null
来源：http://mobile.tarul.cn/Article/details/glgcagvbr.sHtML


<!-- 参考信息 -->