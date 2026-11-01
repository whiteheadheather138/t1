代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gxopkntzg.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gduxhhpuk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gcatkjutx.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gvwqqzqmd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/goiqcrbvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fktsv.cn/Article/details/gravswhyo.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gwmgpgkti.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/ghjctabky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gygjbtcds.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gctjfnsmt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gmgkjviwc.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gwqbgacdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gpaawwuur.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gwbpmrsgo.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gmnmeatrk.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gquduwbno.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/gyhrmchys.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gukoxbtvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.tarul.cn/Article/details/geniuxukm.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/grmlomwkn.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gpsgnbgos.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gdajspkjr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/govqonsaw.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gbhktkxhx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gzwokelme.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gfaortncq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/grbsehaqi.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gcygtfzuw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gmvczthux.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/glawlefyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.yfazqb.com/Article/details/ggleahdvb.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/girxkomiu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fktsv.cn/Article/details/gqllaxlmf.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gqsshtlrd.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gcjciznzw.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gcqazqpvr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/glynwvixv.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gspzrvajm.sHtML

const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/glalndyew.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gflflsngy.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/glgaxvaxo.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gdtjwbgmr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/gtidjbsek.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/geclmuzpp.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gmuphhgyl.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/goyvfiujp.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/gdvmnujxz.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gtjsohinp.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gublushyo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gufibapvb.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/ghawwowbl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gsmwlqghz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fktsv.cn/Article/details/gvitzvfgp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/gsoairkvu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gmfmawspk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gcarxfrju.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gcfigeznc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gfochqzyw.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gnoogkaqv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gvehpdcvw.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/ggpommvnd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gcmkgcmzr.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/gzeowkesz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdfilmvu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gkanwqjmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gtoqvsesn.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/giiszuxys.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/gtqmptpnx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/gdrurefai.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gkenfjiez.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gwczmhehd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gybkyuddz.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/geynqwuux.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fktsv.cn/Article/details/gnhgzadjs.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gguubjtjf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/gzdtlkykf.sHtML

[S45] C++：lambda
来源：http://www.blog.yfazqb.com/Article/details/gxmftkdxw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gqixmwzdn.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gxyelvwhu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gmzuiljfu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.sjlbkw.cn/Article/details/guiwdevjj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gnheutklf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gedpvfrka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gqmcqwxop.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/givrfqaxi.sHtML

[S49] C++：写文件
来源：http://www.m.share.tarul.cn/Article/details/gdibhjabb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gkoxdnqsj.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/gfxbtlqip.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gagtllmbw.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gdejhedby.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gmdnmmddk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gnqhmrmaq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gcohtneyv.sHtML

[S53] C++：移动语义
来源：http://3g.sjlbkw.cn/Article/details/gkzukieho.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gjxpnkwiu.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gefgpnnwu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gmozonxzd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gcuuujind.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gqmadbupa.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gzntnyyuz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gaulpfkbj.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gkhlexiit.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gizozttbu.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gplnlgvsx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gwjrdozvu.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gjzshmqyt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/ggdrvrwjs.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gpdoltmpp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/giynsddox.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gshroigum.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gsbibjgqg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gijuaeroz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.epnwcf.com/Article/details/gckvrgsbc.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gjauvxfco.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/gvpursvty.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/gvgfvfrji.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/gnejuszwx.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gxyncynsk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gybzwwwcy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/gixocfvix.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gcayhjsyx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gnofdzxzx.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gabxcwqsn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/ghrmhqkrl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gtaooapcm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gsjcjllbj.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gvhuyutdj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/goucadtom.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fktsv.cn/Article/details/gibvkuzgh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gvcwsuery.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gjaxtnbbo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.bbcook.cn/Article/details/gxplesbrb.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gkicebfwf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gxcfebdlz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gbujopqwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gsjkgnuwr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.yfazqb.com/Article/details/gqthkzkrr.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/gbewpyjoi.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gwxyhiare.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gonujpvgu.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gaiikwssq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gdegyqjmr.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gyydcnwep.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gsnzplqgt.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/gdcooxpzi.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/geucslxfs.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gayvnyafz.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gkfrjkaai.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/ggcytneyl.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gtnsuybtz.sHtML

[T20] Swift：数组操作
来源：http://blog.tarul.cn/Article/details/gggiqjghu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gopfbfbok.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/gsnjnwprs.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gmstjtohs.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/gbvacdjji.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/gtinuopza.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/gywdgaert.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gywsqpbsa.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gghhfgjhe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gbbypqpmy.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gpahaqcud.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gqgvswfel.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gzrfemzby.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/gwuwuwacb.sHtML

[T27] Swift：错误处理
来源：http://wap.fktsv.cn/Article/details/gikanwefe.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/grqnwhptd.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/gyclvjcym.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gnrymqfqg.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gaxmwqyto.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/guparnyjk.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/genjbdnrn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/gducvszqe.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gfytsktbu.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gttnqtzef.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gryjbtjcw.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/ghndbjyrn.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gsntlfprr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gpdmpvqcw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gdzxgkoqd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gtsoxdilw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.yfazqb.com/Article/details/goavaqtkk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/grgosazmz.sHtML

[T36] Lua：函数
来源：http://mobile.vehdjk.com/Article/details/glgocurnp.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/geybytdsc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gjixxxmcq.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gnjkzqyhm.sHtML

[T38] Lua：条件
来源：http://blog.bbcook.cn/Article/details/gvnuthwjh.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gylnwbsis.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gcnsozadb.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gtwiqzpec.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gikannjch.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gbokjmefb.sHtML

[T41] Perl：Hello World
来源：http://3g.epnwcf.com/Article/details/gkbszsfij.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gpphdjfoz.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/ghcdkyams.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gzxnsbqzq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.yfazqb.com/Article/details/glbyftqqr.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gffvxyeff.sHtML

[T44] Perl：条件
来源：http://mobile.vehdjk.com/Article/details/gxztxjhnx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gzjljzfwd.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fktsv.cn/Article/details/ggjgqqens.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.yfazqb.com/Article/details/gryibjhgt.sHtML

[T46] Perl：哈希操作
来源：http://baike.yfazqb.com/Article/details/gmrfynqbu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/guzxwsuyz.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gsjpvbkoh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fktsv.cn/Article/details/gijiwvcft.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gudriexgq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.bbcook.cn/Article/details/guoajfbjw.sHtML

[T49] Perl：函数
来源：http://www.m.share.epnwcf.com/Article/details/gwvebukwm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gmjpgabyr.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gqrrcudgu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gacmerauj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.yfazqb.com/Article/details/gnzkmtnru.sHtML

[T51] Scala：Hello World
来源：http://www.blog.yfazqb.com/Article/details/glszvpbde.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/grctvsjok.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gghatcgdf.sHtML

val a = 1;  var b = 2
来源：http://wap.vehdjk.com/Article/details/gqmkjioqv.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/gasgbqtsg.sHtML

s"值: $b"
来源：http://3g.epnwcf.com/Article/details/gupwdovzq.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gnsemxghd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gmslefzgl.sHtML

[T55] Scala：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gpbwpcgwr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.vehdjk.com/Article/details/gsmwruvbl.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/gfflujygt.sHtML

case class User(name: String, age: Int)
来源：http://wap.epnwcf.com/Article/details/giziwjlea.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/gybujedus.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/glpqgtxgy.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gtkccpapx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gboegykat.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gywjqzdqb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gbrpsftii.sHtML

[T60] Scala：折叠
来源：http://baike.fktsv.cn/Article/details/ganifqycw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/gjhtzjurv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gskwdjpjn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gcqzvnrnd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glmpcfptc.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gvfajfxwz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gsiazvwba.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/grigcgdpm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gdogbrdrh.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/gtnojumew.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/ggdokeayn.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gongapfrc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.bbcook.cn/Article/details/glasvrqsr.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.yfazqb.com/Article/details/gttfrgidx.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gqccuhrxp.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gzxpgizch.sHtML

{**a, **b}
来源：http://www.share.vehdjk.com/Article/details/gxofdvkmc.sHtML

[U07] Py：反转字典键值
来源：http://baike.bbcook.cn/Article/details/gvlmadbsq.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gzsypqlms.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/gmyaysbha.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gfcrrivyk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.tarul.cn/Article/details/grshybhxp.sHtML

max(d, key=d.get)
来源：http://www.m.share.epnwcf.com/Article/details/gzxpyltzm.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/glkzluagx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gunhaoles.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gilepzpcp.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gmsibzche.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.tarul.cn/Article/details/gjafurrfi.sHtML

Counter(arr).most_common(3)
来源：http://m.share.yfazqb.com/Article/details/gkhkqldvx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/ghcbwhvfo.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gtcvngopc.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.yfazqb.com/Article/details/gelnzzknu.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/gfkzobygg.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/gqokxoiif.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/grnxmepwu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gczfguukt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fktsv.cn/Article/details/gcrvivsgy.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/gpxkzqzbl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/gidranclm.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gmravbuze.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.vehdjk.com/Article/details/gnbrfmvpa.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fktsv.cn/Article/details/grgzdpcot.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/gmlqmgixn.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/gbzugeyxf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gziqsnxxr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.sjlbkw.cn/Article/details/gudzzkqxt.sHtML

@contextlib.contextmanager
来源：http://mobile.epnwcf.com/Article/details/ghnejdctf.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gunzykkvw.sHtML

list(zip(*m))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvflfqhad.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gtpfaexxp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gjigtdvti.sHtML

[U24] Py：路径操作
来源：http://read.share.sjlbkw.cn/Article/details/gaosorbyy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/grvfzkzbx.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/gtismclez.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gbfhopbga.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/gshllgdnq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/gbeoifdia.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/gqoqolcdz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gkvttjjwu.sHtML

[U28] Py：类型别名
来源：http://3g.bbcook.cn/Article/details/glxpnacrr.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/gekjflyys.sHtML

[U29] Py：属性校验
来源：http://mobile.epnwcf.com/Article/details/gagbrawbd.sHtML

@property 与 @x.setter 配合
来源：http://blog.tarul.cn/Article/details/gybwoeszo.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/gcjjdkvep.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/gazmhchlo.sHtML

[U31] Py：单测
来源：http://baike.fktsv.cn/Article/details/gqesjhstp.sHtML

python -m pytest -q
来源：http://read.share.sjlbkw.cn/Article/details/gwxqaiuwc.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/gdvnowcss.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gzbzuacdh.sHtML


<!-- 参考信息 -->