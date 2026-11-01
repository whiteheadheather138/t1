代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gapmrzclx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gtmdxhium.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gydpfepvl.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gyuksysus.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gyojpnolm.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gkmlyovta.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/grcanlfro.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gbvydwqkx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoxadiod.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gkcloruhk.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gfkilnnvd.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gcaogjomx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/gldnsdgzc.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/ggwsokszv.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gcmomuuvi.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gaqikglct.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gtqprchut.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gilgzezng.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gqwadcpze.sHtML

[S30] C：头文件保护
来源：http://blog.sjlbkw.cn/Article/details/gysovcfms.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gioazhoaa.sHtML

#define X_H
来源：http://mobile.fktsv.cn/Article/details/gcjnqmbdl.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/gmxnmpscg.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/grfidikil.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/goezxdnng.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.sjlbkw.cn/Article/details/gokgsvgqx.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/gahioolak.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/ggwchmfnu.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gqhakykka.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/gkreivpzb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.bbcook.cn/Article/details/gufrxbhyh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gpdfoldck.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gzdnydimi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gifhquazg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gdmeffqkk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gjupfhyjm.sHtML

[S37] C++：set
来源：http://read.share.fktsv.cn/Article/details/gyexkrckb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gmgybqnpp.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gyzekriux.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gftqcxokr.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gehuretoa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gksatojkq.sHtML

[S40] C++：查找元素
来源：http://baike.vehdjk.com/Article/details/gxjeiwwde.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/gkjbrlinj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gmochrafl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/gxqfpastu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gjjrezzze.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/ghjokvydo.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gnqfgmjtn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.epnwcf.com/Article/details/gciddkbvf.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gulqofupy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.tarul.cn/Article/details/ggtajhyzc.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/gbavinxty.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gboddsrzr.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gczklrypj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/ghlrcbysy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/ggqifoclr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/guhzvdejj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gplxepkgw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/gpfzsmfti.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gesgbsnit.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gfnhvkzdm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/glqgsssdx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gydmqmbqx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gdjdyuxoe.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gaikgedpf.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeznhfcx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/gnltjivef.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/gafsugxkj.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gbmhwcpef.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.bbcook.cn/Article/details/gmgadvtdw.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/glqhmnlxb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gdljlbvqx.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/ggjjvjpjt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/geuubtlux.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gspbqdoxz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gujbbenff.sHtML

[S57] C++：编译期常量
来源：http://m.share.fktsv.cn/Article/details/garejqfjq.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/golqsfhkm.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/ggmqvgfal.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gbmqjmety.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/ghvvuivvo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gmcxatonz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gdkpqinec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gvwzxtuqr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glgcxzjzo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gzjptiktj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtsibrbqx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gxxvrycya.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gvksyaami.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gvukxzfqo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gqocjheof.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/ggptewyfd.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/gayootatv.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/giibyijns.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/ghytptzvz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gzfsirwlx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gpjcyglys.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/ghtushtjs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gsbazwvqi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gzbmnqmnp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/gffqlfkrs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gaqgxfncj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gbabvckrn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/grqilkhvg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gtoqwzmsn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gbjjgbxpz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gfuqjrvwj.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gdsxntbyr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/gjizytfwn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gwaebutqt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/gpswbmvlj.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gdvqduxkg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/ghkmujsgh.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gfbbkjexv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/geilrufyh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gejxsgdyp.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/gqtwpipur.sHtML

[T16] Swift：Hello World
来源：http://wap.bbcook.cn/Article/details/gqbxoydmo.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gzcmwolgq.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/gucdxqeqw.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gbukbkaug.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gtvqgxncx.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/ghbmlqyfw.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/gzslagpow.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gezyypfhj.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gobvmjbgg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/guummzxog.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/gqglbzbmc.sHtML

for x in a { print(x) }
来源：http://baike.epnwcf.com/Article/details/gwdcxteci.sHtML

[T22] Swift：字典
来源：http://mobile.bbcook.cn/Article/details/geefaqkkf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gqzesdcmb.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gyghqohfw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gadtaqxus.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gykrahlcr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.vehdjk.com/Article/details/gpcvbrgkh.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/gorxlxpfm.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/gxrfcqffw.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/gwwibkujf.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gtuamgqbe.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/glbymvaoy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/glqsjpbax.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gcffzmaoa.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gimaucusl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.vehdjk.com/Article/details/gaysyhjqk.sHtML

guard let x = opt else { return }
来源：http://www.blog.tarul.cn/Article/details/gcddbxpnx.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/gncrtvjie.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.bbcook.cn/Article/details/gfbwvokjf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gyxlegyxu.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gdsizugvu.sHtML

[T32] Lua：局部变量
来源：http://www.blog.vehdjk.com/Article/details/gikfvjsmg.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gxvbdpssi.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gsuqlofod.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.sjlbkw.cn/Article/details/goomwfuml.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gddrdrmse.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.yfazqb.com/Article/details/gzevmlssa.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/gqkijwrpb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gmbxpkuly.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gigqzgrqt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/glfcyacxy.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gyvldzcxf.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/gfclswgys.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gisvdpiom.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gpmhxydvt.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gmovspvtt.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gqppiqojd.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/gukpvmwwa.sHtML

setmetatable({}, { __index = base })
来源：http://blog.sjlbkw.cn/Article/details/gpshoylco.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gmzorxory.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gijzuyzoy.sHtML

[T42] Perl：变量类型
来源：http://www.blog.yfazqb.com/Article/details/gitkfwjnd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/geguahket.sHtML

[T43] Perl：字符串插值
来源：http://3g.fktsv.cn/Article/details/gsxnstpku.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gfpjmmikl.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/griffsasa.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gmpoiodoh.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/glbrjnssx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/geelaujvw.sHtML

[T46] Perl：哈希操作
来源：http://blog.epnwcf.com/Article/details/glgwzcomi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/glwryejpm.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/guhxyybkj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.tarul.cn/Article/details/gjxxqeohv.sHtML

[T48] Perl：正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gpkgnlmrr.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gtlydxkph.sHtML

[T49] Perl：函数
来源：http://mobile.vehdjk.com/Article/details/gaphmimfm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gzcnithwh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.vehdjk.com/Article/details/geneyznyk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gcofiszie.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/gmqefiwbg.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/gvybhueee.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/geakybwxx.sHtML

[T52] Scala：变量
来源：http://read.share.vehdjk.com/Article/details/gecywuikg.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/grztlpczj.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gekptnrro.sHtML

s"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gdfafbnkh.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gninqaysr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gootupkzm.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/gijmgntmu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/gclmhnxcb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.yfazqb.com/Article/details/gxbobbtnr.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyxmokaz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.vehdjk.com/Article/details/glpftznnr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/guwvtfysi.sHtML

[T58] Scala：函数定义
来源：http://3g.sjlbkw.cn/Article/details/gbklobvqs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gmwebcdxv.sHtML

[T59] Scala：循环
来源：http://baike.sjlbkw.cn/Article/details/gpwufxboj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/goweaaebn.sHtML

[T60] Scala：折叠
来源：http://baike.fktsv.cn/Article/details/glselmswu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gsoeuetkm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdozdcrex.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gucubosvj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjicguspt.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.yfazqb.com/Article/details/gsuteopet.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gfziygdqf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.epnwcf.com/Article/details/glassiive.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.bbcook.cn/Article/details/geirfuiae.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gyulnqlks.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/gezqkhqcc.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gwxwydpmp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fktsv.cn/Article/details/gjxltdhbh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/gheljbsvj.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gnxuuidrf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.tarul.cn/Article/details/gubdngtfr.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/gbtakuazm.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.tarul.cn/Article/details/ggysogvnk.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gfozjtgdg.sHtML

[U08] Py：展平二维列表
来源：http://m.share.sjlbkw.cn/Article/details/gdamdzkwp.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/gjhvbsbsk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gcgkzkulo.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gfhnbauhp.sHtML

[U10] Py：按值排序字典
来源：http://baike.epnwcf.com/Article/details/ggiotsfpe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gtfvjcuew.sHtML

[U11] Py：生成器表达式
来源：http://wap.fktsv.cn/Article/details/ggcjbtkap.sHtML

(x * 2 for x in arr)
来源：http://m.share.vehdjk.com/Article/details/glbsetujd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyhdbqdk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.epnwcf.com/Article/details/gkqojpijv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.bbcook.cn/Article/details/ghoejyycq.sHtML

deque(maxlen=10)
来源：http://blog.vehdjk.com/Article/details/gnvplsskp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gatujrncs.sHtML

defaultdict(list)
来源：http://www.m.share.tarul.cn/Article/details/gdcvxibow.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/gjntghvux.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/ggmnedxoc.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/gpppmeqmj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gruwomwum.sHtML

[U17] Py：初始化日志
来源：http://www.share.yfazqb.com/Article/details/gokjagxhf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/gurqsmlzg.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/glosiuits.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gohiecmei.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gyzjjailo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gasvdbwvz.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gpdmoczpo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gdzlhziif.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.bbcook.cn/Article/details/gtdzosolj.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/gciwknndt.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gbdqdvwqy.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/glifutijn.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gskgcunsc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/ghnztnlyk.sHtML

[U24] Py：路径操作
来源：http://read.share.tarul.cn/Article/details/gzzpapvgh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gwxqcbydu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gfnrngaoq.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gzwsqccus.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/glpophxwz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gnbknhuaa.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.sjlbkw.cn/Article/details/gutpbyefu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.tarul.cn/Article/details/gxyuhnnkl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/gquktcswj.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/gqzdyhudt.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/gaermijzj.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gawqfktno.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gdfzrmkdh.sHtML

@dataclass(slots=True)
来源：http://mobile.fktsv.cn/Article/details/gvbxcpswb.sHtML

[U31] Py：单测
来源：http://wap.tarul.cn/Article/details/gtyyvuncd.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/gjuexpzzf.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/ghpdfsrfj.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gfxoxxsin.sHtML

[U33] Py：打包发布
来源：http://3g.yfazqb.com/Article/details/gbdlwvtec.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.sjlbkw.cn/Article/details/gbwitooax.sHtML

[U34] Py：判断编码
来源：http://www.share.epnwcf.com/Article/details/gtedbtpbu.sHtML

chardet.detect(raw)
来源：http://blog.fktsv.cn/Article/details/gxxzncwfw.sHtML

[U35] Py：发送邮件
来源：http://m.share.yfazqb.com/Article/details/giwjcjzbi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/ggnhzgcrd.sHtML

[U36] Py：定时任务
来源：http://read.share.epnwcf.com/Article/details/gmmhktiup.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fktsv.cn/Article/details/gmvcgsiyw.sHtML

[U37] Py：读写 Excel
来源：http://www.share.tarul.cn/Article/details/ghlnrplkq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.vehdjk.com/Article/details/gvasllxfr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gzgbgride.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.sjlbkw.cn/Article/details/gmauqjlqm.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/gkorbmqrb.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/gguxrygah.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gjaseiedb.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/ggkwpyfer.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gwidopytt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gffbwcqde.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gpdpjenst.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.yfazqb.com/Article/details/gmtuuflvt.sHtML

[U43] PHP：声明命名空间
来源：http://3g.sjlbkw.cn/Article/details/ghlgxinhj.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/goqwkxnkr.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbfavtjg.sHtML

declare(strict_types=1);
来源：http://www.share.sjlbkw.cn/Article/details/gqeefrsno.sHtML


<!-- 参考信息 -->