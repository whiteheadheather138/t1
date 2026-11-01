代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gffspnznj.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gqcjmykgl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gosncecjj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gmlafbzio.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/ggchsfkwu.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gflxiqzix.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gyordxpyo.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gkstaweuu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/ggfmamxnk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/goqizeuvg.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/ggfikepju.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gkaupovww.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gxkqoitmz.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gdgezjzsu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsgmebln.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/grruhfmkg.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gawibmywd.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gocdcpbet.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gkmviqcju.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gdjcgxzdc.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/gdgupaccc.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gzbfgmizw.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gjsytnukf.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gcpdprkcu.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gvheaqugb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/ghqfygxij.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/ggdowqdiw.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gafiezmcb.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gfeknqmqd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gfothwiwl.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gxvmvwifg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/gwdugwgtb.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/gkluvjziu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gdrtjwusp.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gbcdegcts.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/greasdhxx.sHtML

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/gnszhbezo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gmteqnhwf.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gglfwzyzc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gykzdwcon.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gdsdrdpmm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/glfsotssv.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gzwyjkhlo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.sjlbkw.cn/Article/details/gforihrkb.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/ghhsrvjub.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gacccidjt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gmzlpaoxw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gjbvtvsic.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gfcivgbnr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gvpznwmag.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gswkhltwc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gprbppvbt.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gljthgggf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gdvfksoji.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/ggxegrwol.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gelbynrgi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/gtplhobrw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/glznykijr.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gdrlbvtxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.tarul.cn/Article/details/guigdjatm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gfjzaismn.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/ggiieirwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.tarul.cn/Article/details/givfrcvfy.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gizosvhvy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gozbepcrf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gkufwfkhj.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/goopbfrgh.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gmomzirob.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gpapwmyai.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/ghlscvoua.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.yfazqb.com/Article/details/gpyfsumie.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gavgdynnm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gmudjwgie.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gwxkxszhv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.epnwcf.com/Article/details/gomhebriq.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gkrqtdcsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gszlajyul.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gzzsusdms.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gqptxcaln.sHtML

[S58] C++：命名空间
来源：http://3g.yfazqb.com/Article/details/gprlwlfuq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gszetbzfk.sHtML

[S59] C++：静态断言
来源：http://wap.fktsv.cn/Article/details/gjhukekqr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/gxofmjumg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gzydmfkpp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gimgjnonr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gohjyfqcr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/ggukyncxs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfkdfkrvf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gbivrncwh.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gjudyscbu.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gpwhvllgc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gfrvkdknf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gpymlweuu.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gbkhfmpyn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/gytqqhxqg.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gmxujmcvc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gedrlzjvs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gfppuvcql.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gjnpcfbri.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gudhhjacl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gjwiugwmw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/guxpgmhlp.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gqpyzjege.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/giubovasp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/grsskgfpf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/gdbaozego.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/ghmzcpgfu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gcsvgwuel.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gmdesgknz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gbxufljea.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gjybptcqp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/giogyitoj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gbwehpswx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gxvwjvtwr.sHtML

[T14] Kotlin：循环
来源：http://3g.vehdjk.com/Article/details/gryneodvt.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gedlyhglg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/ghslpcjwv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gtmiyzfjm.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gpedjlsqe.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gkbvhtops.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/grbnjkpxy.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/guiqazjgj.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gtmveibpy.sHtML

"值: \(b)"
来源：http://m.share.epnwcf.com/Article/details/ggwybtnnb.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gkjcnkokq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gsqhxagbu.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gwlgigcdi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gwxgzkajz.sHtML

[T21] Swift：遍历
来源：http://3g.sjlbkw.cn/Article/details/gwaaoobed.sHtML

for x in a { print(x) }
来源：http://www.share.yfazqb.com/Article/details/gaskknhbp.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gaqvifxaa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fktsv.cn/Article/details/gpfnaejxl.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gwnxqqxvm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/ggmibtqbo.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/gdrlwtufr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.tarul.cn/Article/details/gwusoqeyh.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gnkvskatd.sHtML

struct P { var x: Int }
来源：http://baike.yfazqb.com/Article/details/gqlvylile.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gisptxdpz.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gecjhmrix.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gwkohemsr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gnfcyjjhm.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gklylckoy.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gfuhbmebr.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gxgknhdzp.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gvimkvcij.sHtML

[T30] Swift：协议
来源：http://www.share.fktsv.cn/Article/details/gmcgmgtgx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/godmdfndz.sHtML

[T31] Lua：Hello World
来源：http://wap.tarul.cn/Article/details/gysagohvy.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtjzbrlp.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gxeoeafef.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gjjxgskzx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/geohborik.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gbegpcgob.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gekpggpaf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gynthogfd.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gvzxecshh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gqfprrwlk.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gmtcepuwd.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gwjvjlzvn.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gjoqehvmv.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/ghtfgzuft.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gmikzfdxs.sHtML

if x > 0 then print("正") end
来源：http://mobile.sjlbkw.cn/Article/details/gnfzjkamd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gtkackmzb.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gtnfxliak.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/gtlingioa.sHtML

setmetatable({}, { __index = base })
来源：http://blog.bbcook.cn/Article/details/gillotlpd.sHtML

[T41] Perl：Hello World
来源：http://baike.fktsv.cn/Article/details/gqvtiazqp.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gcapbldee.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/gwacgqpcv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/goouwkcyr.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gkaczslaq.sHtML

"值: $a"
来源：http://mobile.fktsv.cn/Article/details/gftagzznf.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gcjlwnbst.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fktsv.cn/Article/details/gtihqnimn.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gjzgvxlqr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gwsatcern.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/ghystowwo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gonwyxnuu.sHtML

[T47] Perl：正则捕获
来源：http://wap.tarul.cn/Article/details/gcxiiuwkk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gkqrvtjyl.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/getiqjrpw.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/gipabhgkw.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gqkhnmgtj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/grwrkeqhd.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gfdlgotvw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gpjtzztrz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.epnwcf.com/Article/details/gkfkjqpuq.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/griddrlon.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gdmrizafe.sHtML

[T52] Scala：变量
来源：http://3g.vehdjk.com/Article/details/guueqoyvh.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gpceoasdq.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gzmczzdiu.sHtML

s"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gskdelwwl.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/ggtkdnqxv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gnojsnjma.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gfjgebckq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/ghpritgrh.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/gamsukdgn.sHtML

case class User(name: String, age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gwozcuzqq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gczyctarw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.tarul.cn/Article/details/grlfvhpeg.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gumfrzyry.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gcjcmhhud.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gczjsirns.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.tarul.cn/Article/details/gnweuopqr.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/ghrnfriox.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/gkvxunfon.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsghwsvlq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/givomgbmc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfqehpwvj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/ganlwkyts.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.yfazqb.com/Article/details/greelepld.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.yfazqb.com/Article/details/gxvgxdtfl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/gsslncfup.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.sjlbkw.cn/Article/details/gwitrzmac.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gcviuspjv.sHtML

[U04] Py：变量调试打印
来源：http://mobile.sjlbkw.cn/Article/details/gfgjsxwoj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/guqhenilm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/ghxoiqoqw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gharhsnme.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.tarul.cn/Article/details/gtpfyqwsl.sHtML

{**a, **b}
来源：http://wap.fktsv.cn/Article/details/ghexcorht.sHtML

[U07] Py：反转字典键值
来源：http://blog.fktsv.cn/Article/details/gncmojhvr.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/ggjdykyjv.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/ganxmampn.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/gtqianxuy.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.epnwcf.com/Article/details/gsbebzhpf.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gheypjaqj.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/glidhivki.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gsnjkqyel.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gdnyiuxcs.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/ggajsuwnr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.epnwcf.com/Article/details/gofrdgpjk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gsejdxjqc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/graooeyph.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/giyqocvuq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/gvilsyceg.sHtML

defaultdict(list)
来源：http://baike.tarul.cn/Article/details/gjpohetxg.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/gitqheovq.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gpflwduov.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/goqyayeqs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gjlkeesap.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gpufbcohf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/gamrhalui.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gkhiqkbxe.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gxiuuexfw.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/guqqnxwov.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.vehdjk.com/Article/details/gilnbicua.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fktsv.cn/Article/details/gzmosqvbx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gvrtgmhjm.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/gcvknfnqg.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gtykqxzuq.sHtML

[U22] Py：矩阵转置
来源：http://wap.yfazqb.com/Article/details/gttrmympk.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gvjabvjtb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.bbcook.cn/Article/details/gfbjrcyva.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.yfazqb.com/Article/details/gfcazbhsk.sHtML

[U24] Py：路径操作
来源：http://read.share.fktsv.cn/Article/details/gceelekdz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gmggselci.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.yfazqb.com/Article/details/grkbqmfpj.sHtML

csv.DictReader(f)
来源：http://mobile.sjlbkw.cn/Article/details/gyerwlehu.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gkuapfile.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.bbcook.cn/Article/details/gdkufdier.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.tarul.cn/Article/details/gvgdkdntj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/ghykgjtku.sHtML

[U28] Py：类型别名
来源：http://mobile.sjlbkw.cn/Article/details/gyuwwivkg.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gqftqqoze.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/gibjnbnlt.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/gwyfpdgux.sHtML

[U30] Py：数据类
来源：http://m.share.yfazqb.com/Article/details/gmjeaefew.sHtML

@dataclass(slots=True)
来源：http://blog.bbcook.cn/Article/details/gpyeqwett.sHtML

[U31] Py：单测
来源：http://mobile.fktsv.cn/Article/details/gsuqjdsub.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gsoxqdezf.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gpttkksbe.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/gvimnnaqi.sHtML

[U33] Py：打包发布
来源：http://mobile.bbcook.cn/Article/details/gutetczbq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.vehdjk.com/Article/details/gmbridloo.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/gijxlyjpv.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gfqohjpwd.sHtML

[U35] Py：发送邮件
来源：http://read.share.epnwcf.com/Article/details/glpdfudab.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.vehdjk.com/Article/details/gcgqrdbec.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gkpusdtge.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.bbcook.cn/Article/details/guuqwpgzu.sHtML

[U37] Py：读写 Excel
来源：http://m.share.vehdjk.com/Article/details/gzkhawmph.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.vehdjk.com/Article/details/gyeqjxvkr.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/gveubhlby.sHtML

Path(__file__).resolve().parent
来源：http://read.share.epnwcf.com/Article/details/gunoiswsu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fktsv.cn/Article/details/gwvspghxw.sHtML

sys.stdout.isatty()
来源：http://blog.yfazqb.com/Article/details/gzzydsaho.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gqxoixvly.sHtML

print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gizmhwqwl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.vehdjk.com/Article/details/giupolxns.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.tarul.cn/Article/details/gcolxyawe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.epnwcf.com/Article/details/gmrmhreyk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.epnwcf.com/Article/details/gwnbycami.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gvnneihyl.sHtML

namespace App\Http;
来源：http://www.blog.vehdjk.com/Article/details/gurwlyeqq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.bbcook.cn/Article/details/gzgxtshxm.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gwaylvefd.sHtML


<!-- 参考信息 -->