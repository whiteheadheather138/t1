代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gnyqxwdvp.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gyhvrmmao.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gekprevsd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gkievndqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gjrzzyjxk.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/ghohjyyqd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/glvkneosl.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gykawcodx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/guhbtyvax.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gdetwylah.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gwsdurtqf.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gdgedgqcy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/gasvzqihc.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gtntihfla.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/ghersxidl.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/gxajttyas.sHtML

static int counter = 0;
来源：http://www.m.share.tarul.cn/Article/details/geraizgbz.sHtML

[S29] C：变参函数
来源：http://www.blog.bbcook.cn/Article/details/gxdanqqqf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/ghsydiznz.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gqgqhurta.sHtML

#ifndef X_H
来源：http://wap.yfazqb.com/Article/details/gtrjgayrc.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gvdcayjlh.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gaoaalzbf.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gkwrdgcit.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gcfbiwitx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gxweicopc.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gqvdildxd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gilspzuvy.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gonijlray.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/glortmxpl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/gyhayoheb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gbqqghzdo.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gktafgrxg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gcjyrxsgm.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gyfqzwptt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gxqvvjfxl.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gwwdegabn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/goucyekpn.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/goobdaeeo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.yfazqb.com/Article/details/gtypapghr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/gwdpygcwa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/geviymzqp.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gjadophgg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gsnjhajgy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.epnwcf.com/Article/details/gwqatvick.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.bbcook.cn/Article/details/gxqhdpgnu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gfagmklxe.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/ghdaqbwiw.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gatirjuui.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gwdfqmhbz.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gslhxmppb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gxecbyekb.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gfondplor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gmovrkqce.sHtML

[S46] C++：函数模板
来源：http://blog.bbcook.cn/Article/details/gacxigugw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gykrglnzm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/gvyjpjsty.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqncqrbi.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gfyzhqkei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gpdhpzefk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/gmbxsylzg.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gnqlgziyb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gxsklwjlu.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gsouppiuj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/gqlmuonkl.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gvtyisjqv.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gxtjixceu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/gkzatvujw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gctzaeoye.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gontzcuwo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/ghlrwxspx.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gdoyruewc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gwvoxqtdq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fktsv.cn/Article/details/grxybxgdf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gffdkantw.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/gagsygfvg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gsagiutdv.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gcxypnsyf.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/ghhdewtfa.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gyjfxpzuj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fktsv.cn/Article/details/gvltsvgnv.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gkhdjntqu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/gzoquosgl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/ggciyxylo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gzyszrjch.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/griypevzr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/goxbdktqi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbqjvjthe.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gdzdfssba.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gawxuxkiw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/ggvdtgklo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/gfbcfavjd.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/ggyxxjtoj.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gjwhztzhh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/ggqalryvf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/glpswpova.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/glvzunxbl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/gnqpxyuqi.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/goxbsrraq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/grqyuclme.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gavkxoxig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gaxeqeqrx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gnrdvjndh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gajzdnhbj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gknpukdek.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gndnxucut.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gfylhdaoi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.vehdjk.com/Article/details/ggblwrzcn.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrfhkowm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/ghzirrizk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gnybanroh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gxkiagkcz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fktsv.cn/Article/details/gsqovoiyc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/gxvmbwlgc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gwtthkcth.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gfpwbpoge.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gqbufsrfl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gosimpzwm.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gliefetrm.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gbsyeghww.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/gbysjdyvw.sHtML

var a = 1;  let b = 2
来源：http://3g.tarul.cn/Article/details/gogisfkos.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gnjiltqvx.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gbddkzvkc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/grcofkhzb.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/gfqrynarm.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/gopnphimy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gklnxkfnk.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gviwkulzy.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/geputzqym.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gaxxuyair.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.yfazqb.com/Article/details/gbgsjjtnx.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gtauflhtk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gfxnwchpm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/gxeeyvrca.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gqmqtmmzg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/grpyvakhh.sHtML

struct P { var x: Int }
来源：http://baike.yfazqb.com/Article/details/gbrvmrrre.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/guanlmhwj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/grfrbijkw.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/gmykysnse.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/gkervqtms.sHtML

[T28] Swift：枚举
来源：http://m.share.epnwcf.com/Article/details/gkqdszlqq.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/gmsenbixx.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gudjvtcnd.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/gpvsgdvtx.sHtML

[T30] Swift：协议
来源：http://baike.yfazqb.com/Article/details/ghoeiuaka.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/gejpvrbdo.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gmmbkoyyg.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/grlpouoox.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/genhemkom.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gazbbcmil.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.epnwcf.com/Article/details/genptdkus.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/geviiflri.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/gklcqxace.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fktsv.cn/Article/details/gpewhhrbs.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/gnitlvkdl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.sjlbkw.cn/Article/details/gjplqhoap.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/gqmhyiqwa.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gcmjmptrl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gtcvezoby.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gkwxhhhyt.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gbczvrwhh.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gfzcqdkjx.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gcpvggkti.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gmhzoqmha.sHtML

[T40] Lua：元表
来源：http://3g.vehdjk.com/Article/details/gtrmkxzxk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/gavcpzxve.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gfasgnmxz.sHtML

print "Hello\n";
来源：http://www.share.tarul.cn/Article/details/gvawopjcf.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/gsciqzwwr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.bbcook.cn/Article/details/gbjewcucj.sHtML

[T43] Perl：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gkxxhkzbj.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gpdgpspfg.sHtML

[T44] Perl：条件
来源：http://m.share.sjlbkw.cn/Article/details/gzbxnkpjy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.sjlbkw.cn/Article/details/gflvcsree.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/gyawtsrfs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyegrgzla.sHtML

[T46] Perl：哈希操作
来源：http://wap.vehdjk.com/Article/details/gqmficeor.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gjjibeiiz.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/gcbbfzfqt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/giiyzmafm.sHtML

[T48] Perl：正则替换
来源：http://3g.bbcook.cn/Article/details/grhsqhmsd.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.bbcook.cn/Article/details/gbpdmngyp.sHtML

[T49] Perl：函数
来源：http://www.m.share.tarul.cn/Article/details/gurlhubhv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gjdrjswvy.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/ggflvazxd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.yfazqb.com/Article/details/gwtrwcqhi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gzaxtjqzv.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gavoagckv.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gadgakwpr.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gxuyetjlp.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/guftxtfvn.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/gcdsyyvcw.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gihyvsvhg.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gokchpcgf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gzqfxhqqd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gfytrgxfi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gxmpeqknd.sHtML

[T56] Scala：样例类
来源：http://3g.vehdjk.com/Article/details/gjxdpuxqq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/gohobcmos.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gqbxyqbju.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gnazodmjf.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gnkljynol.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.vehdjk.com/Article/details/gtlkbpeku.sHtML

[T59] Scala：循环
来源：http://m.share.yfazqb.com/Article/details/glchyviha.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gkanzvxfz.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/gvxyzjmgl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gcsqkzcpf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gykedojex.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gokvsoayz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzhaseceo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/glnsgrkfv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gaxicvgie.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gahdcpdph.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/gcgwefxuw.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gmdllyzoa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gloftpkxi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gwbbkgxxt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/guntxepyj.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/giwueiyaw.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gyturtjsv.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gturocpef.sHtML

{**a, **b}
来源：http://blog.sjlbkw.cn/Article/details/gajryhfar.sHtML

[U07] Py：反转字典键值
来源：http://3g.tarul.cn/Article/details/gdnqodlpx.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/gybuiqazo.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gwdipglvh.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/gcyrmkemg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.sjlbkw.cn/Article/details/gmgwxadkv.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/ghoxfpobp.sHtML

[U10] Py：按值排序字典
来源：http://www.share.yfazqb.com/Article/details/gkirfmfkj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.vehdjk.com/Article/details/gzwzwcozd.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/gsltnriqa.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/gtnmtvlnb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/gqedbwlak.sHtML

Counter(arr).most_common(3)
来源：http://www.share.tarul.cn/Article/details/gkkrrroap.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gggnbgurg.sHtML

deque(maxlen=10)
来源：http://wap.bbcook.cn/Article/details/gngisyvdr.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fktsv.cn/Article/details/gpbzgkgvj.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gjotgzoiz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/grqjyoedx.sHtML

t = time.perf_counter()
来源：http://mobile.tarul.cn/Article/details/gslpdhbon.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.sjlbkw.cn/Article/details/gqjmtylwk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fktsv.cn/Article/details/gbvbliedy.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gngmjptaq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/gvrfxbnzp.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/gjjgxwsaj.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gtfxngniw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.bbcook.cn/Article/details/glkavugro.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.epnwcf.com/Article/details/gedjrffpt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.tarul.cn/Article/details/gdjanrzfc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.tarul.cn/Article/details/ghbefdyrp.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/glbqkdobm.sHtML

@contextlib.contextmanager
来源：http://www.share.tarul.cn/Article/details/gkvkbompi.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gfgoackfp.sHtML

list(zip(*m))
来源：http://read.share.yfazqb.com/Article/details/gzzfkbiqn.sHtML

[U23] Py：分块读取大文件
来源：http://3g.tarul.cn/Article/details/gdlsuyeho.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.epnwcf.com/Article/details/gkofqwxfe.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/ggvkmwmdf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gifvnqavn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/guaajipcu.sHtML

csv.DictReader(f)
来源：http://blog.bbcook.cn/Article/details/gtxrgvjod.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gpsjdydcu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.epnwcf.com/Article/details/gijvehiry.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gbizrlcpd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gvykwzvcm.sHtML

[U28] Py：类型别名
来源：http://mobile.sjlbkw.cn/Article/details/gsiminlcw.sHtML

UserId = int
来源：http://baike.tarul.cn/Article/details/gjzjsgcoe.sHtML

[U29] Py：属性校验
来源：http://wap.fktsv.cn/Article/details/ghaleccix.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gelektwpu.sHtML

[U30] Py：数据类
来源：http://read.share.fktsv.cn/Article/details/gzhkbavrb.sHtML

@dataclass(slots=True)
来源：http://baike.epnwcf.com/Article/details/gjelhxtxh.sHtML

[U31] Py：单测
来源：http://read.share.tarul.cn/Article/details/giywtwwda.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gjcfcdblg.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/giuluqjcw.sHtML

ruff format . && ruff check --fix .
来源：http://blog.vehdjk.com/Article/details/gewavzqdf.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/ghkzwxxvb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gbhryrkcr.sHtML

[U34] Py：判断编码
来源：http://mobile.fktsv.cn/Article/details/gncfdpxgw.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/geglqelpq.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/geqcbceyk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/gfdukfndu.sHtML

[U36] Py：定时任务
来源：http://www.m.share.tarul.cn/Article/details/gpgzlpmrv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/gqlsyvlna.sHtML

[U37] Py：读写 Excel
来源：http://baike.bbcook.cn/Article/details/gdzfrhool.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.vehdjk.com/Article/details/gglfhfqhl.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gbttjxyhg.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fktsv.cn/Article/details/gqzswaixz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.sjlbkw.cn/Article/details/gvxdfkihv.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gcpobzaxn.sHtML

[U40] Py：打印到标准错误
来源：http://baike.vehdjk.com/Article/details/gnwnqomub.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gtmzjrvzc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.yfazqb.com/Article/details/gcferpvqo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/givjwfrcy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.vehdjk.com/Article/details/gpadmwuwm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gesfuwtrs.sHtML

[U43] PHP：声明命名空间
来源：http://3g.yfazqb.com/Article/details/gpqwaiaqj.sHtML

namespace App\Http;
来源：http://www.blog.fktsv.cn/Article/details/gbhthshpv.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.yfazqb.com/Article/details/gjmpqllsa.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/gdehsmouj.sHtML


<!-- 参考信息 -->