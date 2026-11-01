代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gwytculng.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/grfwokkif.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gtljftonh.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gnnmetchg.sHtML

x |= (1 << 3);
来源：http://3g.vehdjk.com/Article/details/guftjjyjd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gythxalyh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/ggvkhsimx.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gcvdmyntt.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/gzslpxgmb.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gwjpaozps.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gjzzhevdl.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/ghtawcqhm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gjnrcsdzh.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gmrdrietr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gzljediio.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gcmxwhvsy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/ghltsyxfi.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gbdbnhiqg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gbzzuvips.sHtML

[S24] C：获取本地时间
来源：http://www.blog.tarul.cn/Article/details/gjvrpbloe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/glxragamw.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gnfwwvley.sHtML

memcpy(dst, src, n);
来源：http://blog.tarul.cn/Article/details/gihjlymxj.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/ggqiejvkp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fktsv.cn/Article/details/gbobqbxab.sHtML

[S27] C：定义常量
来源：http://3g.sjlbkw.cn/Article/details/gamxsokuc.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gvkhjnwij.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gjydwiozw.sHtML

static int counter = 0;
来源：http://www.blog.vehdjk.com/Article/details/gbinztmjn.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gvtzbtlik.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.epnwcf.com/Article/details/gubqlzvwr.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gyessvxlp.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gaazdlqbu.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gvftfdnuw.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gljqcqluo.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/gxjrictqu.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gczujkmmb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.tarul.cn/Article/details/gqnddfgdq.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gmvjtmdzy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/grelllkgv.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gxdaxvjjt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/gihwvtkxn.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gbfuuojrk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gwygtsijm.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gbtuvfbpv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gocnroycz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gnlxenlgd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gusrtxzwv.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gcluvdslh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/gkyqbjvhu.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/gnnwkzyqn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gfwysakdd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gguxtojtn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gisqyikbz.sHtML

[S40] C++：查找元素
来源：http://www.m.share.tarul.cn/Article/details/gtsuqqgdp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gtzclgivi.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gnpphgeqm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gqdunlmty.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.tarul.cn/Article/details/gaftfmxhj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gnlghfdlh.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/ghvxrgbzz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/gexftfkhj.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/giqmnbqgd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/gqxqoraew.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gejzrbbnj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/ghxmjxkdj.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gjhyohafr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gaefemraf.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gnwqkryyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gqhvvpsbd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gcnvqfnyf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gmcneoqba.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gomcnnqim.sHtML

[S49] C++：写文件
来源：http://read.share.bbcook.cn/Article/details/gwqakiykc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gucmkeeof.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gsrkhnpgb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/gmhqwuteh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gawldzxqi.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gpppspxwi.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gbyuepfdl.sHtML

int size() const noexcept { return n_; }
来源：http://3g.epnwcf.com/Article/details/gzuxqzcxl.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/grkvdfcju.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gjyxudhnd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gdkkhxfqq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gxzqdfsza.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gsdivmpbw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/gcrxgwvst.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gzbhadjik.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.epnwcf.com/Article/details/gifkqokxk.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/ghsiflmgq.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gistnsbth.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gudrdttzz.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gakfdhjmb.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gfajxhipb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/guqpgutcw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/greadecwt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gxkouvwme.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjgzsujef.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gyvbvnqtf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grtsohglq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gcltdewvz.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gxvwyatth.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/ghcrkksir.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gbchuapag.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gqooyppku.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gdlrpsxdu.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/gyyescmuv.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/gxufatwmf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gfhkucuvd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gzdwssawx.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gimlxcacz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/grszapihz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/ghhncraaa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/ghjcjkpxg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/ghxnublve.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gqtmmuron.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/giijynyib.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/ggxxdcvku.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/geaanakdn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gzovymodx.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/gauitckbm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gwvudbjdx.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/gtmypxyik.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gksqcvtxl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gozwoqfqt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gtjshgvba.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/ggpfvfghz.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gbvcbwhmq.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gqjygljsi.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gyjxbfmgk.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gddhnrrhq.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/guzrfakjt.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gwymtfeea.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/gujwufadt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/giwlhguxs.sHtML

"值: \(b)"
来源：http://www.m.share.sjlbkw.cn/Article/details/gthzbfhrj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gchbfmgux.sHtML

if let n = opt { print(n) }
来源：http://3g.sjlbkw.cn/Article/details/gflfrenwm.sHtML

[T20] Swift：数组操作
来源：http://blog.vehdjk.com/Article/details/gzycqibzd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/gewxiahmx.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/gklstruqp.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/gsybxsiwd.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/gnutsbohm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.bbcook.cn/Article/details/gnxtucyzc.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/gnrfaxpxv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gebzfliow.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/gtepxnzey.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gjqyyzvbw.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gvvmzymuj.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gewgjvmll.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gtlrjwkmw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gtglmphve.sHtML

[T27] Swift：错误处理
来源：http://read.share.sjlbkw.cn/Article/details/goxtlskah.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gdeqdbkru.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gflwqvayi.sHtML

enum Color { case red, green }
来源：http://www.share.yfazqb.com/Article/details/gusikoren.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gzkrpruoi.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gzcjaivly.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/gwdsejfdo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gfvcquhfs.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gsbtrdfao.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/ghqlypdgq.sHtML

[T32] Lua：局部变量
来源：http://mobile.fktsv.cn/Article/details/glabhjdqh.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/gpaddwrnq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gowniepxc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/gbnebxwzp.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/gvwsdlslj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/getydbltk.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/gciqbsofj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.sjlbkw.cn/Article/details/gdfgpdkrx.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gvkhklxsm.sHtML

function add(a, b) return a + b end
来源：http://www.blog.tarul.cn/Article/details/gzodfivwo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.bbcook.cn/Article/details/gvgjdogfd.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/gubjbqmkt.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/guzgynajg.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/gcztbybzz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gtphcafbp.sHtML

string.find(s, "%d+")
来源：http://3g.bbcook.cn/Article/details/guvbqgnsu.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gllzejucv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gksqpnpub.sHtML

[T41] Perl：Hello World
来源：http://baike.epnwcf.com/Article/details/gsqvghczs.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/gsdlknbtg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.tarul.cn/Article/details/gdrsabgzm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.epnwcf.com/Article/details/glxwmcjsp.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/gbzdpddds.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gwdexcqhs.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gzofjtyxj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.sjlbkw.cn/Article/details/gdnsnektc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gevzdwfgq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.bbcook.cn/Article/details/ggogsqpmb.sHtML

[T46] Perl：哈希操作
来源：http://m.share.epnwcf.com/Article/details/ggonlzlef.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxmoexrvm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/glesqundl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.vehdjk.com/Article/details/gpshsjrmv.sHtML

[T48] Perl：正则替换
来源：http://mobile.fktsv.cn/Article/details/ghnbcqske.sHtML

$s =~ s/old/new/g;
来源：http://blog.sjlbkw.cn/Article/details/gtbflabhs.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/gqgtyrwsc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gwwxzwnfw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gpcicuzvy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/gjfpwwisc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/glehkuret.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gaumyiuxo.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gmgjabcys.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gijhpskud.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gshqjdcdf.sHtML

[T53] Scala：字符串插值
来源：http://wap.bbcook.cn/Article/details/gfjojldrx.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/gilcuofxk.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gcknylpcz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gkiapcido.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/gpxdrctjz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/gyznrvecu.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/gscygojrv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsioxmmap.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gddrzkepv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/gujzvbvff.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/goyeynizu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/ggvopeyfc.sHtML

[T59] Scala：循环
来源：http://m.share.epnwcf.com/Article/details/gqgggtaeh.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gejtagcer.sHtML

[T60] Scala：折叠
来源：http://read.share.bbcook.cn/Article/details/gonamsjfw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gblxyqlcg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghnefdrzk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/ggytuqwrm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvmpnkxxn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.sjlbkw.cn/Article/details/giqwxkizq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gcczhfnjg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gwrsyapwq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.tarul.cn/Article/details/gjwwjwvcy.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/grobazrwi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gchanwafw.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/geroxegxb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.tarul.cn/Article/details/gnciwsemp.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/gbktabsoa.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/ggmniboom.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/gairixchm.sHtML

{**a, **b}
来源：http://blog.epnwcf.com/Article/details/gcjomafdd.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/gajdonujk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gifkfcyhb.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/gsumafofn.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.bbcook.cn/Article/details/gtxfocvql.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gdcuysice.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/gjreanamy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.yfazqb.com/Article/details/gzywtwywz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.bbcook.cn/Article/details/gqqdbhwow.sHtML

[U11] Py：生成器表达式
来源：http://mobile.sjlbkw.cn/Article/details/gskcneqoh.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/gqlioabxo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/gsbymwppo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gkmzyjrev.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gyxfmrmhz.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/glughkvjr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.bbcook.cn/Article/details/ggspnayti.sHtML

defaultdict(list)
来源：http://www.m.share.tarul.cn/Article/details/givytvexa.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gvyuutsut.sHtML

t = time.perf_counter()
来源：http://baike.tarul.cn/Article/details/golsauvcb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gpfebnkpv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gtpswfdki.sHtML

[U17] Py：初始化日志
来源：http://m.share.tarul.cn/Article/details/gpqkrytup.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/gvarjvoqs.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/gbimoujuc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gindgghse.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.yfazqb.com/Article/details/gkmksyxho.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/gbnwmgtxv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.vehdjk.com/Article/details/gtjgqtskj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.epnwcf.com/Article/details/gdhhkhika.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gnlckdmia.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gdgocfurf.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/glkdaolfn.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/gyuxkldpj.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.yfazqb.com/Article/details/grpokquzg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlfzwquh.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/gxfohxbcz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gupcltycw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.yfazqb.com/Article/details/gdodnbkjd.sHtML

csv.DictReader(f)
来源：http://blog.yfazqb.com/Article/details/gctrfipbd.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gbnqltxjj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.bbcook.cn/Article/details/gtthtyvty.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.epnwcf.com/Article/details/gapxqcvnw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.bbcook.cn/Article/details/gwmqtunpw.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/gktvcjchb.sHtML

UserId = int
来源：http://read.share.fktsv.cn/Article/details/geizwdtus.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/granjlxqx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/gahcugizv.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/grsgtmviu.sHtML

@dataclass(slots=True)
来源：http://mobile.sjlbkw.cn/Article/details/gsnbqismm.sHtML

[U31] Py：单测
来源：http://mobile.bbcook.cn/Article/details/ghskqolzw.sHtML

python -m pytest -q
来源：http://blog.yfazqb.com/Article/details/getnmwole.sHtML

[U32] Py：代码格式化
来源：http://3g.bbcook.cn/Article/details/gqodttwbq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.epnwcf.com/Article/details/geypocfvl.sHtML

[U33] Py：打包发布
来源：http://mobile.tarul.cn/Article/details/gnxtupwks.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.epnwcf.com/Article/details/geiftqmho.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/gwqavbzsy.sHtML

chardet.detect(raw)
来源：http://read.share.bbcook.cn/Article/details/gjnppzoto.sHtML

[U35] Py：发送邮件
来源：http://m.share.sjlbkw.cn/Article/details/gqsnzhazm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.bbcook.cn/Article/details/gvwwcojpt.sHtML

[U36] Py：定时任务
来源：http://m.share.vehdjk.com/Article/details/gnxsnzwhm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.vehdjk.com/Article/details/ghfgcaxez.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fktsv.cn/Article/details/giqfqcrbv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/glbywwqyb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.vehdjk.com/Article/details/gkyuyqkwa.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gnupzeavx.sHtML


<!-- 参考信息 -->