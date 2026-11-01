代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gocxhdxkx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gzhkefpjn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gcmvfkjjc.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/gguilavye.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gctxsipsk.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/gibedqqql.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gylpuarpd.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gbwwxukin.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gywobrqvg.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gbnxghhcf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gsafuovqk.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gkdjlshqn.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/giuqszshx.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gsiwbcjbf.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gstrpkdfm.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gdyowsaoj.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/glwwxicff.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzjnoodnk.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/geoxwhkmt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/gpchennam.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/gqghcbrvd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/gnfnczoga.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/gjgyvwxcf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/glksvuukf.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gtlwtovyo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/ghrkfmuiv.sHtML

[S36] C++：unordered_map
来源：http://m.share.tarul.cn/Article/details/gnrmmgvom.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gjhrjqbgo.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gppdedofz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gasffrzcu.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/gjgzvwhtd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gmquhazmg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.epnwcf.com/Article/details/grweryuuo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gitmhjnlt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/garpktxqo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/glftgwoew.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gabmagfwy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gdovaymht.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gdkhtxkbl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gjomibuqv.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/gclfnvlby.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gmfhwnguz.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gztghkest.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gylzetlwf.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gbunaxevl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gwobezarj.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gjvzxkptz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gccjerjiy.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/giaahfhet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gtjdfiyoe.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gaczzdtsa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gemrvpcxh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gyqivkgym.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gtddntkod.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gwnjjqicl.sHtML

[S50] C++：格式化数字
来源：http://www.blog.tarul.cn/Article/details/gbtmxzhoa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/galigokxa.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/gaiipgwaf.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/givctsplk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/gamibremd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gjpewcnxl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gzigrcoxk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gsukilmvq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/ggvolrkot.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gnubhlumo.sHtML

[S55] C++：结构化绑定
来源：http://3g.sjlbkw.cn/Article/details/goytfldyy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gvxsziwxb.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gevlenmyf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gzvwfxrle.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/ghzsmtcbe.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gxeqqppoo.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gikjsbvlu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gmygumsmy.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gtozcukis.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gazlkqzgy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gnrjyxuzh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gboqscptr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfvgtsksv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gbybjrklw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjolhygct.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gpiqyhygz.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gfttplcqf.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gsfseddyk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gmwegzdyo.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gqjabwkpd.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gsjfmsznw.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gwlefypsy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gkoipjzkb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.tarul.cn/Article/details/gcndptktm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/ghidxrrzi.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/gdnpwlxvg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gedynjyjv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/grykijmat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/glnqxetkl.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/goswgqzrz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gykhizpyt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gwydcttpo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/gbpyyqdwz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/gejlvqzxk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gqojkgvvu.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/gpezntmna.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/grlazcmln.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gviodbmbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/gptchffae.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.epnwcf.com/Article/details/glavhqcri.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gfoyvquaz.sHtML

[T14] Kotlin：循环
来源：http://blog.sjlbkw.cn/Article/details/grsijqldf.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gpxjvoxnm.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gunhrckap.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/gbvlrdsfd.sHtML

[T16] Swift：Hello World
来源：http://baike.vehdjk.com/Article/details/gyziorswf.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gggpfysri.sHtML

[T17] Swift：变量与常量
来源：http://wap.sjlbkw.cn/Article/details/grqhyhqpv.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/gxgsfrgcz.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gryblsxbn.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gdpyiznnx.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/ggzdvjhaw.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/gmxshhlju.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gcoxedgay.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.epnwcf.com/Article/details/gsaeddqmm.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gdzkopacg.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gkpaefcks.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gljhxizpe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gtvlqgpzo.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/ghounwpks.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.bbcook.cn/Article/details/gchybgtfh.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gocayvwpv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gocbqxmlv.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/gtjsaulhb.sHtML

struct P { var x: Int }
来源：http://blog.fktsv.cn/Article/details/gqksuertb.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gzqijgzup.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/gbkxgtnqx.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/giwfosnpg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/gnuwdrgda.sHtML

[T28] Swift：枚举
来源：http://baike.epnwcf.com/Article/details/ggrvmsdoa.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/gdkeozmvj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.bbcook.cn/Article/details/gkqylmybb.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gfzkvqhdf.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/gxkygluct.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gqknwtfxp.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gpfrnelcq.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gyxzxvwhf.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gflhjacyw.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gnmwetdkd.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fktsv.cn/Article/details/gsnippkzl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.bbcook.cn/Article/details/gvrkwwkdn.sHtML

[T34] Lua：遍历表
来源：http://read.share.vehdjk.com/Article/details/gsecflbon.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gehhjluwr.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/grfykhzbz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/gheokvcoq.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/gbodnssut.sHtML

function add(a, b) return a + b end
来源：http://read.share.vehdjk.com/Article/details/gtqwmriua.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/glzcvgmab.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gnrwrbdxa.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gzpdakvew.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gxfvuuivl.sHtML

[T39] Lua：模式匹配
来源：http://blog.epnwcf.com/Article/details/gqfeolnjp.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/gctgmvwzx.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gioucyuci.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gbdaqacms.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gsedptunw.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/goexoaemh.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gkqoexvnm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gxdufksug.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gjaigwboh.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gtknuakii.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/gwmyjshra.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/gbvtbzlzh.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gaidzgkuy.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/ghlwzskpy.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.yfazqb.com/Article/details/gwhthqvth.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gskexthxb.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gbkzheexj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.bbcook.cn/Article/details/ggkkixkpc.sHtML

[T48] Perl：正则替换
来源：http://3g.sjlbkw.cn/Article/details/gmaiklfjp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.tarul.cn/Article/details/glioesaks.sHtML

[T49] Perl：函数
来源：http://www.m.share.epnwcf.com/Article/details/gkfslpsqy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/grvgubsqn.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gwkggtwop.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.yfazqb.com/Article/details/gufkeuhkz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/guizocalr.sHtML

[T51] Scala：Hello World
来源：http://baike.fktsv.cn/Article/details/gubogscue.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/geqwxtokm.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/gfrrcbujh.sHtML

val a = 1;  var b = 2
来源：http://baike.tarul.cn/Article/details/gskcvqrch.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gxlydsmfs.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gybfxvkqe.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gssuqkzlg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/gsgshqnjp.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gsabrfnbw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/glvylkyoo.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/gtnvwhegj.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fktsv.cn/Article/details/ggbtfpkja.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gzhbwvzkz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.tarul.cn/Article/details/glxxkslux.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gmjjwkgaj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.vehdjk.com/Article/details/gmarpmzin.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gyggsytwx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.epnwcf.com/Article/details/grvwoaaei.sHtML

[T60] Scala：折叠
来源：http://wap.vehdjk.com/Article/details/golwcajyl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gnchqrovb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjqebgmkt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gsqcpohrp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnfkctxbm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/ggymebzgq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gujptoeby.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.epnwcf.com/Article/details/gxifyxzkd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gizxvhhuz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/gcrsmhsol.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/gupfhhuqj.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/gprudvzqg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gfslusudk.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.sjlbkw.cn/Article/details/gexreoqnv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gnqgtohgf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gcfuesdbd.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/goqcqxcrd.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.yfazqb.com/Article/details/gajwuoarn.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/gvnozswos.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/ghgqbxxuo.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/gfaeprhae.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.bbcook.cn/Article/details/gznggthgk.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gjwveoqqs.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/govsdozqz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.vehdjk.com/Article/details/ghgihkuhu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/gzvbcfkty.sHtML

(x * 2 for x in arr)
来源：http://read.share.epnwcf.com/Article/details/glintiwnw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.vehdjk.com/Article/details/gvxejcrtu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.tarul.cn/Article/details/gnioaqgmp.sHtML

[U13] Py：固定长度队列
来源：http://baike.yfazqb.com/Article/details/givgpjddr.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/ggtakvqhp.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/gfqugkbvd.sHtML

defaultdict(list)
来源：http://www.share.fktsv.cn/Article/details/gkmrsodjb.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/gpunoqdav.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gyksryhle.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.bbcook.cn/Article/details/gaxdhxjsi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.bbcook.cn/Article/details/ggqydlaor.sHtML

[U17] Py：初始化日志
来源：http://blog.tarul.cn/Article/details/gbghhmfsf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fktsv.cn/Article/details/gqsfkzgyd.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/ghxozpnni.sHtML

pat = re.compile(r"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gwghyddxk.sHtML

[U19] Py：正则替换带回调
来源：http://blog.epnwcf.com/Article/details/gigqqvlht.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/ggjpgwqvs.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.sjlbkw.cn/Article/details/gsnjrdytj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fktsv.cn/Article/details/ghvojnwqk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fktsv.cn/Article/details/gxwhrzkug.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gqihmfzpn.sHtML

[U22] Py：矩阵转置
来源：http://www.share.vehdjk.com/Article/details/gfdxqmirt.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/ghhzazscp.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gmgdpsuut.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/ghmbhtffk.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/ghtjshhbx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gdujtthml.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.yfazqb.com/Article/details/gyiksvhbn.sHtML

csv.DictReader(f)
来源：http://www.m.share.tarul.cn/Article/details/gtcethxtd.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gjpfwjtva.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fktsv.cn/Article/details/gliddflut.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gskpdhepr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gicmeyhzh.sHtML

[U28] Py：类型别名
来源：http://read.share.vehdjk.com/Article/details/gkmvsqybh.sHtML

UserId = int
来源：http://m.share.bbcook.cn/Article/details/gsodsvztf.sHtML

[U29] Py：属性校验
来源：http://blog.epnwcf.com/Article/details/gsdhzbuub.sHtML

@property 与 @x.setter 配合
来源：http://baike.fktsv.cn/Article/details/gcoexmhgm.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/ghcntusge.sHtML

@dataclass(slots=True)
来源：http://read.share.bbcook.cn/Article/details/gcranqppb.sHtML

[U31] Py：单测
来源：http://blog.tarul.cn/Article/details/gvbdizyzz.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/gahnymstt.sHtML

[U32] Py：代码格式化
来源：http://m.share.tarul.cn/Article/details/guejesspt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.epnwcf.com/Article/details/gphdkvdtz.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gzdstmfph.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.bbcook.cn/Article/details/grjyqnmyf.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gxecsvauh.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/gyhxavqva.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fktsv.cn/Article/details/gbzznumkw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gtaoplzhg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gjyyxzukz.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/gypthwngu.sHtML

[U37] Py：读写 Excel
来源：http://m.share.tarul.cn/Article/details/gbzwcihwd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/gtnfovzst.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/gfunaqsjr.sHtML

Path(__file__).resolve().parent
来源：http://baike.yfazqb.com/Article/details/gewdlwytw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/gaxesgvyp.sHtML

sys.stdout.isatty()
来源：http://blog.yfazqb.com/Article/details/gpvsktiro.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gerzcxkzg.sHtML

print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gbfxqiggy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/glbnskmvu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.bbcook.cn/Article/details/gcuxuuieo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.sjlbkw.cn/Article/details/gfnqkutnp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.sjlbkw.cn/Article/details/gmsmbtxkn.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fktsv.cn/Article/details/gpinymdsd.sHtML

namespace App\Http;
来源：http://baike.vehdjk.com/Article/details/gtfofarvi.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gaagoefad.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gerwsuhwe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.epnwcf.com/Article/details/gulmginyh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/ggyyimmvy.sHtML

[U46] PHP：可空类型
来源：http://3g.yfazqb.com/Article/details/gnuvgfump.sHtML

?string $name = null
来源：http://m.share.yfazqb.com/Article/details/gdjhaaaei.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/gzmyyysrg.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gkyppfidb.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/gijnfnwbq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.vehdjk.com/Article/details/gjhifmhdr.sHtML


<!-- 参考信息 -->