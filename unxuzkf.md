代发 wailian999

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/grolqbigj.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gdhuginpp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gmyroohrt.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gcdckszzd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gnqnjqxdn.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gfttxcycu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gdnqjfnhx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/goqsgnsnz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/ghgrulogg.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gqonemzdq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gynkaigft.sHtML

[S24] C：获取本地时间
来源：http://baike.vehdjk.com/Article/details/gmdkmlpqw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gowtluifg.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gmiopddwi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fktsv.cn/Article/details/gzzlrxybw.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gukjgycve.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gpxyymqks.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gviipqvij.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gkwaabpdq.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/gfgvedpcg.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/glepgzcgn.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/giazktsdj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gtdfiehwk.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/ggpxlfnhy.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/gsfoeueqj.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gonqtypsw.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gsusndjxx.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gfqiptdxp.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gfnaoqpal.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvldjfxrb.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gflldbose.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.vehdjk.com/Article/details/gikezrluy.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gjcjxjgua.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/gpnzmmrlq.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gsqeoqwsb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/ggyrszszn.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/glbnzuirm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/ghytonqyb.sHtML

[S36] C++：unordered_map
来源：http://www.share.tarul.cn/Article/details/gduwvlwit.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gartdlgpm.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/goowmgqqx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/ggdfgpbqx.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/gvpeghnph.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.epnwcf.com/Article/details/ggjeohwep.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.epnwcf.com/Article/details/gyhfcnjuf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.sjlbkw.cn/Article/details/gfqvfpzib.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gutxzewdr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfubaqxt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gnkiopuvc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gsgifqgky.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/ggdbpyqnv.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gjrdfcglq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gocrgnfrp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gbcseehjv.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/ggaxxtvuu.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/glzatujlq.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gcdrabezu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gjfzonrat.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gmltygfjq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gpfnqddrw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.tarul.cn/Article/details/gjahlmbyv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/gphaakxvs.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/ghojmmzci.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/ghodtxier.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gskcqaujs.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/gtnqyhkxy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fktsv.cn/Article/details/gxptwtadn.sHtML

[S50] C++：格式化数字
来源：http://m.share.epnwcf.com/Article/details/gejyqhmuj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gtuzeoiko.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gxcphxruo.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gzfimbrwk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/grysfmkzb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gtkizchou.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/gwebknnrs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.bbcook.cn/Article/details/grzgkzvcp.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gowovhebz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gyinfvmrt.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gwomhykop.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/glvxrgjrj.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gvivdomnv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gdiugobrq.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gyzdinvzk.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gidiilcha.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gxxfdntty.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gwujjidkp.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gnkmuohkg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnfxdzik.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gsttvwsai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gphfjcdqw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gretsiipw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gzygctmja.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghjamvqqh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gzjglxydt.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gnnadxohz.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gjauphmtw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gmymmlabm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gjrvrhosy.sHtML

"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gvemgzjhl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gofeagizj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gfnmmbusv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gksqqdbrq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/glggapttt.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gbvgflvso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gzrzbslux.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/ggsraxuxg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/ghiycyvvs.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gpuswvurj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gwfstetfa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzffseliv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/ghududhjq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gvquiahtf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/gcwcpaidy.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/gswiztmxt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gvbkoldke.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gzklkuihh.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gslukhvia.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.tarul.cn/Article/details/gowdqvaks.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gfezlrije.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/geazrookb.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gxmkunxvj.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gahfnzxic.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/gsqkitapr.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gmerjxons.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/ghiwaznwm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtiiwbga.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gnykafmik.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gbludedcn.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/ghjxygpmq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gmfoiqzvy.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/gabtyswam.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fktsv.cn/Article/details/gjthlrkiy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gkkabukyj.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gtyouagcz.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gsnehubol.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/guynxcthg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/gdheigpcc.sHtML

[T23] Swift：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/glolxizsn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gntyictrd.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gfxaoplrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gqhhiafum.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gezmidorb.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gfuhrtadq.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gbxpsdsyv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gxsckurgt.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/gvnjmznrv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/gcolncvjr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gbbnpqlgu.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gnlvhxvkq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gskmiynrc.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/guqghjwfg.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gpwukswky.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/ghsmqtsgo.sHtML

[T31] Lua：Hello World
来源：http://wap.tarul.cn/Article/details/gugbjufpt.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gmkcmxljm.sHtML

[T32] Lua：局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gnbiwybht.sHtML

local a = 1
来源：http://wap.epnwcf.com/Article/details/gbigexxtp.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/gosqtxlde.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gnraxjadl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gumhdervl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gohqhuzed.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gbccaobpd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.epnwcf.com/Article/details/gzjkhheyy.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gcuulnzcc.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gynvjiagq.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gflksunzo.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gitgusyjh.sHtML

[T38] Lua：条件
来源：http://wap.bbcook.cn/Article/details/gxpuoscod.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/grcmltsgg.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/ggzmeqvdc.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/gtcopqhpx.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/goigafdzk.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/ggdpeuull.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gswjeskdi.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/ghvbeaahe.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/gtgzhbqcp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.epnwcf.com/Article/details/gbczugxts.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gqlbzvreq.sHtML

"值: $a"
来源：http://m.share.fktsv.cn/Article/details/gxmiicyeq.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/ggawmqrgu.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gologehwc.sHtML

[T45] Perl：数组遍历
来源：http://wap.fktsv.cn/Article/details/gwesxulzs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gfotemksi.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/gfoadokcy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.epnwcf.com/Article/details/gjnmrcgmr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gmhxnehyw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/gpjzxsaog.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/gifkjkxgc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gotezrkwe.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/gtkqysawe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gzlydzugo.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gtwudehnh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.yfazqb.com/Article/details/gqzimrtdp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gawcubzis.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/glpwgszuz.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gxclvgzqw.sHtML

[T52] Scala：变量
来源：http://blog.yfazqb.com/Article/details/gnfkqvfci.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gzgatylnn.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/grisgetbm.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gnmerozug.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/gmavlqzcl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gsllowqyx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/glczwlyhc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/glrmqzfzc.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/guznnmsvp.sHtML

case class User(name: String, age: Int)
来源：http://3g.bbcook.cn/Article/details/gxbnmpibr.sHtML

[T57] Scala：模式匹配
来源：http://baike.fktsv.cn/Article/details/gukeohhyr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gbgupicod.sHtML

[T58] Scala：函数定义
来源：http://www.blog.yfazqb.com/Article/details/glffclfng.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gulwpdbip.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/ggxvjeujh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gwncuovxt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.yfazqb.com/Article/details/gmomuvoub.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gniauqaqd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grhhwrkkw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/ggyhpkeyx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnnnssvex.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.yfazqb.com/Article/details/gietubtpp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.epnwcf.com/Article/details/grlpfwetc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.sjlbkw.cn/Article/details/gfjmmagvm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/gdxfjrbgp.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/gycaqkmpz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gdgirevmg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.epnwcf.com/Article/details/gjqpsioqr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.bbcook.cn/Article/details/gtumikjyd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/gwudtzazb.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gtnhprdmm.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.sjlbkw.cn/Article/details/glwavokfe.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/ghwkazzgr.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gkjyijvit.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gaaqfpeci.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gekuksjzt.sHtML

[y for x in nested for y in x]
来源：http://3g.epnwcf.com/Article/details/grxclrzcc.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/gcpofjmqg.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/grbmdpkyd.sHtML

[U10] Py：按值排序字典
来源：http://wap.epnwcf.com/Article/details/gpuehjdtg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.sjlbkw.cn/Article/details/gjrjzkwok.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/gycyiznvu.sHtML

(x * 2 for x in arr)
来源：http://read.share.yfazqb.com/Article/details/gyhnlzuxv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gwbnbsamq.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/gmymljqsw.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/gdqqxhiac.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/grereisjz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.tarul.cn/Article/details/gblwfchod.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gsifmarym.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/ghylfbhcd.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gdnogbfpg.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gjjlobsrc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.sjlbkw.cn/Article/details/gygghlxjy.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/ghdfwgcnw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gzfyklqkq.sHtML

[U18] Py：预编译正则
来源：http://m.share.fktsv.cn/Article/details/gmvnqtjyt.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gjaaayzwf.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gqruxoree.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.tarul.cn/Article/details/gnzofomxi.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gpevrvpec.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.bbcook.cn/Article/details/gwqcrflyd.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fktsv.cn/Article/details/gaaqsfrjg.sHtML

@contextlib.contextmanager
来源：http://blog.fktsv.cn/Article/details/gdwwnzxjg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gxgmtzise.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/giqgriikk.sHtML

[U23] Py：分块读取大文件
来源：http://blog.bbcook.cn/Article/details/ggxnsurcf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.vehdjk.com/Article/details/gabfuskez.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/gbpkckslu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/ghtbolxxf.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/guwotbczb.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gmatqamoh.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gclsgibfh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.sjlbkw.cn/Article/details/gojjxsrtv.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.tarul.cn/Article/details/gdolbixal.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gkzgcpphi.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/gxyskwqhu.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gkffzywel.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gytnnpnbb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/geszinhgn.sHtML

[U30] Py：数据类
来源：http://www.share.bbcook.cn/Article/details/gbbhxksfd.sHtML

@dataclass(slots=True)
来源：http://read.share.vehdjk.com/Article/details/gqkjxxopg.sHtML

[U31] Py：单测
来源：http://read.share.bbcook.cn/Article/details/gsmzbiucx.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/ginhizgyn.sHtML

[U32] Py：代码格式化
来源：http://blog.yfazqb.com/Article/details/gazirrbcl.sHtML

ruff format . && ruff check --fix .
来源：http://baike.bbcook.cn/Article/details/gqgsocoes.sHtML

[U33] Py：打包发布
来源：http://m.share.bbcook.cn/Article/details/ggvdabwhm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gbkrrjlem.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gzciczqhj.sHtML

chardet.detect(raw)
来源：http://baike.sjlbkw.cn/Article/details/gqtfidflb.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gpegxpaae.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.bbcook.cn/Article/details/gjiudctta.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gxqvgjmgv.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/guznscakt.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fktsv.cn/Article/details/grwzgadom.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.tarul.cn/Article/details/gnpdkjggp.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/gldyyncbu.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gxkwmeesq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.bbcook.cn/Article/details/gydvqczxt.sHtML

sys.stdout.isatty()
来源：http://www.share.epnwcf.com/Article/details/gbdcajwak.sHtML

[U40] Py：打印到标准错误
来源：http://wap.sjlbkw.cn/Article/details/gbwblfpxd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gdkoevgtt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.sjlbkw.cn/Article/details/gvxgnumbp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.yfazqb.com/Article/details/gmvmdtbif.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gyubufwuu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.sjlbkw.cn/Article/details/gpzajvsjj.sHtML


<!-- 参考信息 -->