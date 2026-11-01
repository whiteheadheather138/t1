代发 wailian999

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gtqibvfgj.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gnvvvrrfj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gtnhxsnav.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gdptbrcrk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/guyjlchhn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/gjfzefgrl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/gwhpqhtlq.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gytldimjd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.sjlbkw.cn/Article/details/gquwjluwt.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gxrsvynaj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.tarul.cn/Article/details/gnpfigxyl.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gblwwjfqa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gqhbyhwgv.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gblmqjmkl.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/gamaxsihq.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gifxfsbfn.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/geumuduub.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gvejpiybs.sHtML

const double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gdnjdxaap.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gclgmedve.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gvpgmjlok.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/grigckeyq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gnblncfvz.sHtML

[S30] C：头文件保护
来源：http://3g.bbcook.cn/Article/details/gyumpiafs.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gxxrxlkhg.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/gosgxujhv.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gtwvhcnuq.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gokewepmk.sHtML

#include <iostream>
来源：http://read.share.vehdjk.com/Article/details/gxnbzmrau.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/glftyveoq.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/gphaetfnt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/guruggbnw.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gbmvkgjsw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gdbevosva.sHtML

[S34] C++：遍历 vector
来源：http://3g.fktsv.cn/Article/details/gfqnghdcv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/gzqlnlqqr.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/grqtsvoww.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gpunkpdkr.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gpllebeph.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gerqqtbrq.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/gryostknm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/ghquikxyt.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gemvwquvg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gwivpymfa.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gismpvkxd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/ggishdeil.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gymsdnkbv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/godjtaynn.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/ghqdhkdtb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gcxodhcnd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/gjbjvjhtq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gficjuebl.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gjsmndjrm.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gwjdmmnoa.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gxulshdrc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gecmdyqxu.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/grmuxfrml.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gjsqyvhcd.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/ganhymlpc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gaaelgutu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/ghlmdkacm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gpuzyalvn.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gcucducav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gfpvgfcat.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gbeiiyrvw.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gdjrwmnqf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gptxqispv.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gorslkhas.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.bbcook.cn/Article/details/godglleew.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/grrsosbfo.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/ggtpkbagi.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/gfwsmzzky.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gybxvymva.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gtgafzqle.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/ghascxerf.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gijrhhrws.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/ginmbnpfk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gxyjlxxum.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gbvugmcdy.sHtML

[S56] C++：optional
来源：http://3g.bbcook.cn/Article/details/gwtokqkfj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gjnxcgwct.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gacxltpqe.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/gqafnvhkp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gowjqgouo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gnkskhluv.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gijahfibv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/grwxoicht.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gwsadfmzd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.tarul.cn/Article/details/gxqiotjyh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtguvumte.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gcbmvogmb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdiegiehw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gicrccgnf.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gpsuvgkuh.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/grrlrlcwu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fktsv.cn/Article/details/gvvebdabn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/gmpbwkrie.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gzwblvjuk.sHtML

[T04] Kotlin：空安全
来源：http://wap.vehdjk.com/Article/details/guoahkyik.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/grbvgqhvt.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/goluyumwh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gdjzlgsmq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gbmjtshnb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gkgddqoys.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gdetskbfq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gerxwgbgb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/ghfjtdlti.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfojsuwcw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.vehdjk.com/Article/details/glriiwgkc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gxmegkkdp.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.tarul.cn/Article/details/gzsonhlfw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gdfvcztah.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/ghqxpqawq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gjjmyvbys.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/gphojpivk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxagthfap.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/gaobjxnlm.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gdpdiotct.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/gjnnfdthz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/gbnxoasue.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/gfoizbfiu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/gitoeofyc.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/goajbaowq.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gglzjbkvi.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/gcyjodebt.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gntkjrsfx.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gjcwqdxty.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gzpiyduca.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gbckghvko.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/goxzhlifj.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gxohubwjf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gqcxuaayk.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gjsndslpp.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/gzszoimlx.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gxldqdjwq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.tarul.cn/Article/details/gcgopsjzr.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/gwpjkhfqp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gvrnmazjm.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gxpflkzqp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gmeahxzri.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/grxixscrz.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gwoxrhsqn.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gvuewnwlr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/gkvxhsmab.sHtML

[T27] Swift：错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gttiaomcu.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.sjlbkw.cn/Article/details/ggkqkmogo.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gkszwlohv.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/gacqjsbmd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.sjlbkw.cn/Article/details/glihlqizp.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/gssymczoe.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/gggpsfbam.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gudowoqqz.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gtjcdafrs.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gscvymesu.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/gzojkrsag.sHtML

local a = 1
来源：http://blog.yfazqb.com/Article/details/glkxcscrb.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gywkhwwjl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fktsv.cn/Article/details/gpjcdpfqo.sHtML

[T34] Lua：遍历表
来源：http://3g.tarul.cn/Article/details/gcjpjzfwr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gnlchcbao.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gmrtuhfel.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gsidjqiwt.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gosdezckq.sHtML

function add(a, b) return a + b end
来源：http://wap.tarul.cn/Article/details/gxeovoiug.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fktsv.cn/Article/details/gppvglkbz.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/gulnnocxj.sHtML

[T38] Lua：条件
来源：http://www.m.share.yfazqb.com/Article/details/glmkphysb.sHtML

if x > 0 then print("正") end
来源：http://read.share.bbcook.cn/Article/details/gwtbehskp.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gtvlqdhpx.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gwnxoepll.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gwtezzxmv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gcmleheqo.sHtML

[T41] Perl：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gjktzbcnt.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gqxkeieib.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gsuzqfsvi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/gbcrfbdec.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gvqrbhzpt.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/gkpnaqmhw.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gjuwnxtec.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.yfazqb.com/Article/details/gyepdzylq.sHtML

[T45] Perl：数组遍历
来源：http://baike.yfazqb.com/Article/details/gtamvdxks.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.bbcook.cn/Article/details/groymxmfn.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/ghozxhiwl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/geeyigqvm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gsztpphne.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/gxnkvmscj.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gbnurlumw.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gjzelmuqz.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gthvixigi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gjepxnkzr.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gutsiaess.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.epnwcf.com/Article/details/gqurxjdsc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gbufbwuyo.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gjxywqwrk.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gnkudwyxw.sHtML

[T52] Scala：变量
来源：http://www.m.share.bbcook.cn/Article/details/gqzitfsbj.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/gidqvdqzj.sHtML

[T53] Scala：字符串插值
来源：http://blog.vehdjk.com/Article/details/gbnvfycgi.sHtML

s"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gweexjcqk.sHtML

[T54] Scala：集合映射
来源：http://3g.bbcook.cn/Article/details/gvbpfsqzc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/grdrxmzet.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gimqkqfml.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.yfazqb.com/Article/details/gaxwjgkkw.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/gwfjmsruh.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gvhoohbxv.sHtML

[T57] Scala：模式匹配
来源：http://baike.epnwcf.com/Article/details/gebilrwel.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gnvpmprwk.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/gztwyxvnu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gwroerzya.sHtML

[T59] Scala：循环
来源：http://www.blog.fktsv.cn/Article/details/gwdxehazs.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gdnzzzxja.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/glcwuuvnp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/guutgtbwl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdxqdiiet.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gswqtgdts.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtsjwhpns.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gqppvrlpo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gxdylzgdg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/glxxrquuj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/gfeliemzl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fktsv.cn/Article/details/goelwpslg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/gmvzzmure.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gckukbalv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.vehdjk.com/Article/details/gnmoqfkci.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gxwqbkijo.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gemkupegr.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gimevdbty.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gmjycqyxv.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/giglzhnym.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/grdrlaazf.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gggeyuoqv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.vehdjk.com/Article/details/gyhaqyami.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/gzbenayxq.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/ghygwoxsz.sHtML

[U10] Py：按值排序字典
来源：http://www.share.tarul.cn/Article/details/gjwzmmqol.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/gldshxytq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/goyvbqazk.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/gdxcizeeu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/gnsnsbnjj.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gblhtpgle.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/gofzxyjhs.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gyxeqwvwb.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/gfprejibn.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/gxzhbspla.sHtML

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/gnzgtjqza.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gntgcopnf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.vehdjk.com/Article/details/gvmmwzcky.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gbycdlmnt.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/gejpcmsbz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gtfflfhth.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/glgiougwm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gqutrczdr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gbkcbmyts.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/grvybfvzh.sHtML

[U20] Py：缓存函数结果
来源：http://blog.bbcook.cn/Article/details/gdrcaczvv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/gckjnjuna.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gafgflxea.sHtML

@contextlib.contextmanager
来源：http://blog.vehdjk.com/Article/details/gvnawwrtv.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gqemgtkes.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gspaocpqz.sHtML

[U23] Py：分块读取大文件
来源：http://wap.bbcook.cn/Article/details/gnmmorebt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gumbtqjdn.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gtaqqeiyg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gbmymatyb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gjtqoqgzj.sHtML

csv.DictReader(f)
来源：http://www.blog.sjlbkw.cn/Article/details/gsgnegihp.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/gstblzuxd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.vehdjk.com/Article/details/gboxauexf.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.epnwcf.com/Article/details/gsleaexdo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/ghzyobzjb.sHtML

[U28] Py：类型别名
来源：http://blog.fktsv.cn/Article/details/gmmtepyxg.sHtML

UserId = int
来源：http://mobile.sjlbkw.cn/Article/details/gbkeybaxw.sHtML

[U29] Py：属性校验
来源：http://read.share.yfazqb.com/Article/details/gdlmtcsbt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.bbcook.cn/Article/details/gdeqlsvbf.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gjpudhwex.sHtML

@dataclass(slots=True)
来源：http://read.share.epnwcf.com/Article/details/guuebpaav.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/grbyjmemo.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gvqrfqqhu.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/ggilerhir.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/gptvgiuds.sHtML

[U33] Py：打包发布
来源：http://baike.vehdjk.com/Article/details/gthmzxrii.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.tarul.cn/Article/details/gaajtcopf.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/gmwwahsup.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gnmakyonq.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/gozbfndtr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.vehdjk.com/Article/details/gzeiuymrm.sHtML

[U36] Py：定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gwbggqbac.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.epnwcf.com/Article/details/gchnwuafx.sHtML

[U37] Py：读写 Excel
来源：http://www.share.sjlbkw.cn/Article/details/gcsfzpkfr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.sjlbkw.cn/Article/details/gdpruxxxl.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fktsv.cn/Article/details/gjfbkazbi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gmsnbeuov.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.vehdjk.com/Article/details/gziyfmsrq.sHtML

sys.stdout.isatty()
来源：http://mobile.tarul.cn/Article/details/gcfjohchx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.vehdjk.com/Article/details/gqmjvzoxx.sHtML

print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gcvviehzg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/gobkujgwb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gyqhatrzi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.yfazqb.com/Article/details/ghyxjzkgc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gyanzagmw.sHtML


<!-- 参考信息 -->