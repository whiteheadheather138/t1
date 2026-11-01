代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fktsv.cn/Article/details/gwwzuwsuo.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gnvmejwrg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/ggnalrfbu.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gcgbyseni.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/gnlsjwqty.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gjkeiyrqf.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gtgkgntng.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/gwsxrfjbl.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gxamcewzf.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/ggxhcpxnk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gkuymzhaq.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gskxzazjh.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gxwdqszra.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gukkhjzfb.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gavqorucb.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gegknicts.sHtML

#include <iostream>
来源：http://wap.sjlbkw.cn/Article/details/geenputkw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.vehdjk.com/Article/details/gfmyojfzl.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gvdeqbceq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/gvqmyiuyo.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gbsugnnfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/gkvjrnrxh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gqndoxhxe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.vehdjk.com/Article/details/gzysksofz.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gwiliecyr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gximcqohz.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gesozxdkm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/ggjlkxwbv.sHtML

[S37] C++：set
来源：http://mobile.yfazqb.com/Article/details/gkihiwlkv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gazgawxcf.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gazhphpkz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/givubjxnu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/golgqwmbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gyjpamnqk.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/gkojzvteb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.yfazqb.com/Article/details/gztqfbijc.sHtML

[S41] C++：类与构造函数
来源：http://3g.vehdjk.com/Article/details/gxtcteyio.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gmdnczuyb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gcdnoapfe.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gaxnfoaxo.sHtML

[S43] C++：智能指针
来源：http://wap.sjlbkw.cn/Article/details/girbkreic.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gomfhmmtz.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/ghobglipx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gnrgcetzh.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gyhcjxvhb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/giwrxmxdt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gvphxqssq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gmxaxhexk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gjemmmupn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gktqpjrln.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gvxvpfadd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gnwykhaii.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gdclojqbt.sHtML

[S49] C++：写文件
来源：http://baike.vehdjk.com/Article/details/gqibvuxzn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gwlcvlpvr.sHtML

[S50] C++：格式化数字
来源：http://wap.vehdjk.com/Article/details/glzxoxdeb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gcgooteff.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gbmfyncyj.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gxulkmiha.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gjpevoupe.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gklpwxzyj.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gcqafnkuz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/ghbwiobip.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/ggkyguqlb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/ggjpvlnaq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/gbwdzgeax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gqilcbivi.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gogedudgr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gjqhxliox.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gyirsyrle.sHtML

constexpr int N = 10;
来源：http://blog.epnwcf.com/Article/details/gyuaxvqro.sHtML

[S58] C++：命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gphedwurx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/grldncnbo.sHtML

[S59] C++：静态断言
来源：http://wap.vehdjk.com/Article/details/gecvsmyzl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gcqxfzsfw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gfakwvdjw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gzitryetd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdxcmlwcv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gvitokohy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gocrbqeov.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gmoqawdyt.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/geusnqjdu.sHtML

[T02] Kotlin：变量
来源：http://blog.vehdjk.com/Article/details/gyaotgyux.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gogrwwbds.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gzjoocmid.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gmghgmdah.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gmpjufoyl.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gjiutnuer.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gggvwqvbx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/gppwitfgs.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/gvjpurmni.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gufufuwuf.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gyihiquig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/gwyuikuus.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gngesftlr.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gyzqhlevt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gmkscluam.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gwnchvcrn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gkampkvxo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/ganpzlqgi.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gpzongpeb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/ggfacedha.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gquhrydpp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/goltyqlxd.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gxlgmevwh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.vehdjk.com/Article/details/gksgqtlde.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gsjaxgvmg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gieomsvao.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/grgbribex.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gqtgotunt.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gfadxcynn.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gwfyktfes.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/gmatytcbo.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gyfotzkyn.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/gqcasgdca.sHtML

"值: \(b)"
来源：http://3g.bbcook.cn/Article/details/gobcnrryt.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/gxwxqpzsb.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gdvcdufkv.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/glfzmksso.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gptppbphi.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gfwlqywkn.sHtML

for x in a { print(x) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrvvxwav.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/gqjlhxkfb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.yfazqb.com/Article/details/gxveqdqyw.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gipoeuxet.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gqwuadqjd.sHtML

[T24] Swift：闭包
来源：http://m.share.sjlbkw.cn/Article/details/geyujsjrx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gioxdxvrt.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/gstqsshtb.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/ghnmvvdzk.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/ggmkwjhra.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gslpmepsc.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gclpakgbf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gvpmrlvvx.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/gintpcszn.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/gbhhzrjhv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gkliqrybp.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/galuuprxn.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gnldqkwjj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.vehdjk.com/Article/details/gvdqibsdn.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gztkcueni.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gwdveinrx.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gasgilexf.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gscptczjt.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/gijarjxdi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gcsgnnfqy.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gycyqabef.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gvdfywkcq.sHtML

[T35] Lua：字典表
来源：http://m.share.sjlbkw.cn/Article/details/gwybkmvpq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gnedoubvm.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gddcimvae.sHtML

function add(a, b) return a + b end
来源：http://3g.tarul.cn/Article/details/gkuxgozhv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gipxmqnld.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gttpleyvv.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/girtsaqud.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/gxsxsolnb.sHtML

[T39] Lua：模式匹配
来源：http://wap.vehdjk.com/Article/details/gumqludnl.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gfabnvnvz.sHtML

[T40] Lua：元表
来源：http://www.m.share.tarul.cn/Article/details/galjvzyud.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gpbingkek.sHtML

[T41] Perl：Hello World
来源：http://wap.yfazqb.com/Article/details/gwaaewjsz.sHtML

print "Hello\n";
来源：http://3g.yfazqb.com/Article/details/gawtynzbd.sHtML

[T42] Perl：变量类型
来源：http://mobile.vehdjk.com/Article/details/gakockjue.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gqxwhcozs.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gwbtgplku.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/gzxquxdjo.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gkbviizou.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/goawaddho.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gdptsvtvs.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/grtuzwvff.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fktsv.cn/Article/details/gnbrgnvyf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/ghjblkjah.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/gmmoxzrwu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/gaasaoqro.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gchwypdll.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gtvgqctcf.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/glwbzvcqa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gwsenxufc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gtufgzwzu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/ghjfqlhtm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.bbcook.cn/Article/details/gxubuxvbw.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gtolzkzkt.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gtgjmvegm.sHtML

[T52] Scala：变量
来源：http://www.share.tarul.cn/Article/details/gwubcirld.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/gzguvjkei.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/guxepboun.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gqelpihpv.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/gdwvocveu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.yfazqb.com/Article/details/gjrafkuuo.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/gpkqygyla.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.tarul.cn/Article/details/gjgrvvwkq.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gfkgfxtpe.sHtML

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/gqjcwagbb.sHtML

[T57] Scala：模式匹配
来源：http://read.share.tarul.cn/Article/details/gldozknth.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gtwozoemz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gdxmwyrnu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.tarul.cn/Article/details/ggacldlah.sHtML

[T59] Scala：循环
来源：http://m.share.vehdjk.com/Article/details/gsbfwzjgu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gvcgitrpv.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gakibsapm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gbjrqjxbz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glfqjfkei.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gacszhleg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glsuqbazc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gsakzgrea.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.tarul.cn/Article/details/gvhfqmxqt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fktsv.cn/Article/details/ggyhjkmio.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.bbcook.cn/Article/details/gzdowijky.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiucxhgg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gjskrvyqm.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/gvfcsqvrc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gknxnkuur.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/gxgswpsrv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gwxxialdg.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gvockmveu.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gvadclqkb.sHtML

[U07] Py：反转字典键值
来源：http://blog.fktsv.cn/Article/details/glcipjdcn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/gbdnljone.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gqxauejuj.sHtML

[y for x in nested for y in x]
来源：http://wap.sjlbkw.cn/Article/details/gqwnrtkql.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.bbcook.cn/Article/details/guzqmechr.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/grthttlpi.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/gjbskophg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gvqylguph.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/gutntiqnd.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/gtpavappx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/ghqjmslsd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gpdibgzzk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/gtnckjcso.sHtML

deque(maxlen=10)
来源：http://www.share.vehdjk.com/Article/details/gnxlhsnzl.sHtML

[U14] Py：分组收集到列表
来源：http://3g.bbcook.cn/Article/details/gmmrhtulh.sHtML

defaultdict(list)
来源：http://baike.fktsv.cn/Article/details/gdtvocqkd.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/grxcifouh.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/gpdrltebo.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/geovxdlvz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.epnwcf.com/Article/details/gdhlypevb.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gkrbqlkaj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/ggegdydmm.sHtML

[U18] Py：预编译正则
来源：http://baike.yfazqb.com/Article/details/grfsmlpdz.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fktsv.cn/Article/details/gnnqqbyfk.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/gjcncrnht.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fktsv.cn/Article/details/gcffdxtpc.sHtML

[U20] Py：缓存函数结果
来源：http://baike.epnwcf.com/Article/details/gwharprqe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.epnwcf.com/Article/details/gfvtjmxqa.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.epnwcf.com/Article/details/gwqzztqst.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gjjcuoxac.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/gsnzapojx.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/gdmnrvdyp.sHtML

[U23] Py：分块读取大文件
来源：http://3g.yfazqb.com/Article/details/gytgiwkof.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gadlbzvhc.sHtML

[U24] Py：路径操作
来源：http://3g.yfazqb.com/Article/details/glvcdhvoh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gcsbvvrgw.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gqjbosawp.sHtML

csv.DictReader(f)
来源：http://wap.epnwcf.com/Article/details/gxeodfibm.sHtML

[U26] Py：并发下载
来源：http://3g.epnwcf.com/Article/details/gsbngerzc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gdwkvjebc.sHtML

[U27] Py：异步 HTTP
来源：http://baike.tarul.cn/Article/details/gyektnchf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gulwepujd.sHtML

[U28] Py：类型别名
来源：http://www.blog.vehdjk.com/Article/details/gsztsuvtu.sHtML

UserId = int
来源：http://wap.bbcook.cn/Article/details/grahtdona.sHtML

[U29] Py：属性校验
来源：http://m.share.sjlbkw.cn/Article/details/gecdeybtl.sHtML

@property 与 @x.setter 配合
来源：http://blog.vehdjk.com/Article/details/gxhkkpcor.sHtML

[U30] Py：数据类
来源：http://wap.sjlbkw.cn/Article/details/gwbfzwuju.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/giclswzxm.sHtML

[U31] Py：单测
来源：http://mobile.fktsv.cn/Article/details/gqkwmkfhg.sHtML

python -m pytest -q
来源：http://blog.vehdjk.com/Article/details/gyorrysyx.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/gxoroyoaq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gehlyxoet.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gsgnkiwpk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gcolhyyvj.sHtML

[U34] Py：判断编码
来源：http://baike.vehdjk.com/Article/details/gjxmaldga.sHtML

chardet.detect(raw)
来源：http://read.share.sjlbkw.cn/Article/details/gfxcuxrcj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/gjmjlgevn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/gkctwwzyp.sHtML

[U36] Py：定时任务
来源：http://baike.fktsv.cn/Article/details/gdvhugrdb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.tarul.cn/Article/details/gtyeczeka.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.yfazqb.com/Article/details/gvpiuhznw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/grtvlkyqa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gahrpmacg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gniqvdkkm.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fktsv.cn/Article/details/ghdtnbycn.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/ghcndmbqi.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.tarul.cn/Article/details/gkuzlelap.sHtML

print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gpnffswcn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.tarul.cn/Article/details/gqsuzqwuw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.yfazqb.com/Article/details/gmhqgfewp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.bbcook.cn/Article/details/gyylgouxs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.yfazqb.com/Article/details/gfpwtfolw.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/gpqtjasov.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gemqrounw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/gescugpll.sHtML

declare(strict_types=1);
来源：http://wap.fktsv.cn/Article/details/gfvrcoklv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.tarul.cn/Article/details/gipeobzca.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gjvfywkar.sHtML

[U46] PHP：可空类型
来源：http://m.share.fktsv.cn/Article/details/gxbwcqqub.sHtML

?string $name = null
来源：http://baike.fktsv.cn/Article/details/gtuuvktcf.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/ggvtsimus.sHtML

int|string $id
来源：http://baike.tarul.cn/Article/details/gosisfyvj.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/gezjrpnor.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fktsv.cn/Article/details/gffmbdiam.sHtML


<!-- 参考信息 -->