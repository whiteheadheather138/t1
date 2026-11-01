代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gtnyqnhby.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gkpurpqqd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/grwndtcnw.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gvbvafmho.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gmvdduvzy.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gmiamsxeq.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/guitishdt.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/ghggikhoy.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gwugghfvh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gjxuarvif.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gdfaorejg.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gezxfazie.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/gymjjwppr.sHtML

[S19] C：快速排序
来源：http://3g.tarul.cn/Article/details/gznbtwikm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gdszcngey.sHtML

[S20] C：二分查找
来源：http://wap.sjlbkw.cn/Article/details/gdwxdwpfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gdzcdicfa.sHtML

[S21] C：字符类别判断
来源：http://3g.yfazqb.com/Article/details/gutvuyvwx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gdxdjhoev.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gexndocbf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gwhcnxgpg.sHtML

[S23] C：随机数
来源：http://www.blog.vehdjk.com/Article/details/gsqnnpcxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gmaarotur.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gqtdektfd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gvracvicv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gmocjbpks.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/ghvrclqbi.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gsonfxnxi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gchqhgvod.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gngsbitcf.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gjtxslhkx.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/geevyovfr.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gnoiyvrqb.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gvaugktku.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gutujpdsy.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gprzadnqe.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/guksyuazn.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/glhwdppri.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gntpcyfnj.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gvfihmppy.sHtML

#include <iostream>
来源：http://www.blog.fktsv.cn/Article/details/gftwudijk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gdftzzwno.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gtgfwypqz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gytblpfrk.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/gzvsduocf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbcendaz.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/ggcmdhdho.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gnmifgptg.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gcqjoxazs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/grbmizjgw.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gxvfsfucz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gygsgtylx.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/glagssjbp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.vehdjk.com/Article/details/ghwcnkphs.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gfgffyrjp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/gerwxvivw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.epnwcf.com/Article/details/gbchgzgpd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/glpcatgxb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gveomnjgg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.bbcook.cn/Article/details/gwmcrcxkx.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gmfhbjbjt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gafnmjabi.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.tarul.cn/Article/details/gbxhlulam.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gspqheccc.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gxqppthib.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gxaflwsjc.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gfckmbued.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/ghaljknhi.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gxddlmcdf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gahepeolz.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/ggauzjubo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gccntgomu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/gcugsmzeq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.yfazqb.com/Article/details/gotablgis.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gtpvaryxi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gfmafuwol.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/gewszeswl.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gpzuyydwi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gjgttgytc.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gkclgfyyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/gjnpzonnc.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/ggstlplny.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/gtvuirhpc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gnveogvek.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gcxlalzpl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/grqqikuzu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gpbibxggs.sHtML

[S54] C++：异常处理
来源：http://www.share.vehdjk.com/Article/details/grhyxuxnd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gskoqazpz.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gjeujmnbc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/gwuharnzl.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gydopuswg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fktsv.cn/Article/details/glykkngen.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gtollywdt.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gmoizwryq.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/ghjhmqejf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gdqieudkn.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gpywghlal.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gvcmmlbmh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/gzbuxyhxt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gzumcrxwy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqsshmleq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/goouzezxo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaqmdlzbi.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gfqpyumgs.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/guqujvunb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/ggazqnugs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/ghgtunmxv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/grulhrzxn.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gvrnwppsl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/grmtfawnp.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gkmmwwhhb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gicomtkpa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gaisequmf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gsrkjxjeb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gjysnftco.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gsszszjuh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.bbcook.cn/Article/details/gejctokvy.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gtrhbzoyi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gtfakrftp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/gyqvrudku.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gzlnedbvn.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gcmknyxwz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/ghhdjzets.sHtML

[T11] Kotlin：协程
来源：http://mobile.bbcook.cn/Article/details/gdeexhphm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.vehdjk.com/Article/details/gietnqdez.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gfgtsihew.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gnunewnvc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gtfjhilpo.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/gbpikndjy.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gunvwmxgp.sHtML

for (i in 1..10) println(i)
来源：http://baike.fktsv.cn/Article/details/gibamufjr.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/gtwwhsvcz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gsunwmizu.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gwlubpcdt.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gdwnqkmhg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gldxpqavb.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gnbdikblb.sHtML

[T18] Swift：字符串插值
来源：http://baike.fktsv.cn/Article/details/ggmrkvoul.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gmhvnanqk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gehekidfc.sHtML

if let n = opt { print(n) }
来源：http://www.share.vehdjk.com/Article/details/gygmgjvpj.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/grxjgksmv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gipdvwgei.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gcrmirsce.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/guddyipfb.sHtML

[T22] Swift：字典
来源：http://baike.vehdjk.com/Article/details/gatyoxhky.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gbfjzweyk.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gafbhkklu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gtyacameq.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gawluuszs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gobnkwlfh.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gghgutzls.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gukaksdhd.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gxrzaoiuj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/grdvhmzvc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/giwvsrhjs.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gjjeeqykn.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gempigbhx.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/guebowhzh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/gsxwqwyor.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/gdunqqbiy.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gzqfurxae.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gzmcyiclw.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gsbhrxoln.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/grnvjwpeu.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gqyptxswh.sHtML

local a = 1
来源：http://mobile.sjlbkw.cn/Article/details/gwclrjvcb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/guumzucml.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gfzgmaybb.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gugmrpzir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/glhptbaxj.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/ghevhuhyg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/gshsfsmfp.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/gcimdxsef.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/gphmkvmir.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gpsuyrmdq.sHtML

"a" .. "b"
来源：http://www.blog.vehdjk.com/Article/details/ggladopyi.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/goymamprc.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/gsputbfpq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gbyabulnp.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gromssslz.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/gnvronepu.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gzojrimqy.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/ghsrltdiy.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/giztrvoic.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gyjiqzxxu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/geakipcrc.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/gancaaaaj.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/gebeqiqjt.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gunzwchoj.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.yfazqb.com/Article/details/gfunhmyyv.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/gmqwzngmp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/gftktkqkf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/ggduqfgbf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/gldnoflzg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.tarul.cn/Article/details/govtldgue.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/gjfmyplpd.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/gpzzctvsx.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.bbcook.cn/Article/details/gaczgcfbj.sHtML

[T49] Perl：函数
来源：http://mobile.epnwcf.com/Article/details/gvxyvsjki.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/govlzgsak.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gxgddmtkw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gxsnvkdye.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/giepuevpf.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/govktwooa.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/glxgrtgmp.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/gxlmxnpvq.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/grvdebqfz.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gpnohooih.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gnucvrgfj.sHtML

[T54] Scala：集合映射
来源：http://wap.tarul.cn/Article/details/gexhujgwe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gmegyjehi.sHtML

[T55] Scala：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gwnrltiyf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/givcstrjo.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/ggdqaiqkj.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gycfbyrdg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gmkpxsetv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/ggoqvkibb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/gdancrbok.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/gazzvcgdu.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gvzzarxzm.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gpgkyhnjk.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gzdzrpldx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.sjlbkw.cn/Article/details/goqxbuiro.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpjlozmpw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.vehdjk.com/Article/details/goifduxda.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyixbxyqz.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.sjlbkw.cn/Article/details/gudglznmj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gexlfople.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.tarul.cn/Article/details/guojbhsdl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/gfjrpmysi.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fktsv.cn/Article/details/ggycoijcw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/ginosxgxe.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gfbsijvuk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/grdzyzzcd.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/gwftldpdr.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gcfgvdnzf.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/gonxxbozv.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gvjjlhdca.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gaczxczba.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gxldfofgq.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gmleqkvje.sHtML

[y for x in nested for y in x]
来源：http://www.blog.vehdjk.com/Article/details/gqpmdatqk.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.sjlbkw.cn/Article/details/giypcyaqt.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gjwofotmm.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.sjlbkw.cn/Article/details/gttoutocr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/griqkiqpd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gmpvrzijq.sHtML

(x * 2 for x in arr)
来源：http://wap.fktsv.cn/Article/details/godibpllh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/gcrbtqznu.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gnivrhvqg.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/gjvhnpfrm.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gtyxvrzgg.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gocbpjvdd.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/gcolgthzg.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/gmlswnyyk.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gnztwalsj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gljwhzhtm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/gcxwdessr.sHtML

[U17] Py：初始化日志
来源：http://www.blog.vehdjk.com/Article/details/grnulfdbo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.tarul.cn/Article/details/gdvrfpunc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/gsqnuoztb.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/gehgkwbrz.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/gucxxbrrs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/grxjcbukg.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gguqixxyi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fktsv.cn/Article/details/gxvivgiqv.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gurapesmu.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gsxgayntu.sHtML

[U22] Py：矩阵转置
来源：http://baike.epnwcf.com/Article/details/galvaymle.sHtML

list(zip(*m))
来源：http://wap.fktsv.cn/Article/details/gtrsrzmnl.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/gvnylbqxz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gsqmnuyvz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fktsv.cn/Article/details/gvwbbakmf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gfwblglae.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.sjlbkw.cn/Article/details/grkifsxyl.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/gkjvtvshl.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/ghlcuxlkk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/ghvutipzt.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/ggvorcbjl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.vehdjk.com/Article/details/gmxwcjiiv.sHtML

[U28] Py：类型别名
来源：http://www.share.vehdjk.com/Article/details/gsfjxyftk.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gkpklusiq.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gydrxzdot.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fktsv.cn/Article/details/gknwfrxcu.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gqpujloct.sHtML

@dataclass(slots=True)
来源：http://wap.sjlbkw.cn/Article/details/gnnwchzcl.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gjfxqepil.sHtML

python -m pytest -q
来源：http://m.share.epnwcf.com/Article/details/gjswsgyaq.sHtML

[U32] Py：代码格式化
来源：http://3g.bbcook.cn/Article/details/gfesllzgt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmmkqhle.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/gvujdfpwh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/gkfzkwvxt.sHtML

[U34] Py：判断编码
来源：http://www.blog.sjlbkw.cn/Article/details/gnmynfzse.sHtML

chardet.detect(raw)
来源：http://www.m.share.bbcook.cn/Article/details/gqoaseuvg.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gbbahllsk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/gmacybgua.sHtML

[U36] Py：定时任务
来源：http://www.share.vehdjk.com/Article/details/gjnomvqsh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fktsv.cn/Article/details/glokljulr.sHtML


<!-- 参考信息 -->