代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/gvxqakzcv.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/gngwbabea.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gqmscozzp.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/geipuhsdj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gmnodrgwg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gibkredzy.sHtML

fclose(f);
来源：http://blog.tarul.cn/Article/details/gwffhzlaz.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gbkoefosi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gnicbtjhh.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gueyvoarf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gqjgtejyz.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gjhigtdcu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gzqtvjqgq.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gonsssucl.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/glithkcgk.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gysvklffy.sHtML

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/glkccjvqo.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gwxhahyep.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gohpbvubw.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gfcgpghoi.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/grrdtgnoo.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/ginybegin.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gcwbayifo.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/grelgiqov.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/ghqnwauoe.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gxdmajeos.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gcwcciqxd.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gtjrzxspd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/govcqwpul.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gmwznlbki.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/gguuqsmzs.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/ghqsahflq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/goddpznhc.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/ggxqmnkid.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/grntsniuw.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/goyfswdxo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gfmvhvnri.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gwtwpejks.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqlqbgdr.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/ghzyqybhh.sHtML

static int counter = 0;
来源：http://www.blog.vehdjk.com/Article/details/gvugbqhqa.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/gcsksmswe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/ghfypiezd.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gzircekvb.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gkvonetsa.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gdiutzaud.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gfboxqvsz.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gqgmcpxcc.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gcrpbawsy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gacqjvtxm.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gmmtoxdvp.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gqsgirygx.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gpehbnhay.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gbxewicqx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gbybdbaos.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gcaifiigw.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/gcvanapmf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/goxhtuuok.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/guzluloni.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gdrwxccch.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gydfesbzk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gnunfuvwg.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gfnbwfdmp.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/grbsfcbhu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gyhtxkena.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gdeqwxnlk.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gurdkafvo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gcwhcuwrd.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gcqovqwkq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/ggtrlbrbw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/ggdmrthfr.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/gmkgxakrs.sHtML

[S43] C++：智能指针
来源：http://www.share.fktsv.cn/Article/details/gosamdebe.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.vehdjk.com/Article/details/gixegtcis.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gxjcrtfga.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.tarul.cn/Article/details/gfbtpepzx.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gbyhjdftg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gjgpqyycr.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gvqstycnr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/glztqwldp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gekihipuo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/gelnukgga.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gefrysguj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gudqjijuc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gvwekkusu.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gaprrnatp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gqhoomfuh.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/gegmfiyux.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gatcyohzf.sHtML

[S51] C++：显式类型转换
来源：http://wap.sjlbkw.cn/Article/details/gdcsnamqk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gslqpicml.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.yfazqb.com/Article/details/gygkzifsb.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grmwbdpbz.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/ggqajyjae.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fktsv.cn/Article/details/ggtfmrwyb.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gxnxlpyce.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gxkoofxkk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gzgisvafy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gcmftrdpr.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/gaeepfxgm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gdsjypvwq.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/gncyzcsoj.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gxfurtdlm.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/gfqwbpxat.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gmplquwul.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gyxejzpnr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.sjlbkw.cn/Article/details/ggmbnbuch.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gmkrfrrnr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.bbcook.cn/Article/details/ghthzlnhz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwpewnlzp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gfzyvhbma.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gklbeixjy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gwkdmoynq.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gstkzfofg.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gxthbyzqq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gbepjnknt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/grfihhsjz.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gnajdkzlp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gedgaitkv.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gkcjesawr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpxxplmp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gkdschmst.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/ggegabrmw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gbmifrbnh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.epnwcf.com/Article/details/gkhewobia.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fktsv.cn/Article/details/gffdbfkif.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/ghnxxfvbz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gwkkaudqe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gvofymbjt.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gsmdbvtoi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gungjyjgn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/gvzyxqmhn.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gsaibidjc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gamnqpynf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/gerjbqtwz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/grsbosizj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/germgxnzl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.epnwcf.com/Article/details/gtmksybya.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/grgcpsqfu.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gerlelqwo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gigwayxcd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gzbdcawwr.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gcxhpapgg.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gygibbsjq.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/garfnkfol.sHtML

var a = 1;  let b = 2
来源：http://read.share.tarul.cn/Article/details/gyxgbkqxe.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/guvrslzqe.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gxfsubhyp.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gekdabklc.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/gpfcvozmd.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gohkznwrt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gkbkxjfhn.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gjlzlxaeq.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/gjujdoxvz.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gqjxsdjuu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.epnwcf.com/Article/details/gzqncvdpd.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/gsqtrsime.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fktsv.cn/Article/details/gbbprbfeo.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/ggccddjiw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gxrdealog.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gqpdcddgh.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gfocagjts.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/guaismdfx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gkzzxlxsh.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/gcigzoqos.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/gwcegaqme.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/ggaouvjaz.sHtML

enum Color { case red, green }
来源：http://mobile.bbcook.cn/Article/details/gsnkmochx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/gyvxrijew.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gzgpzuawj.sHtML

[T30] Swift：协议
来源：http://read.share.yfazqb.com/Article/details/gzamzzkab.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fktsv.cn/Article/details/gdhanqive.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gympfajcy.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gjcxqxwpw.sHtML

[T32] Lua：局部变量
来源：http://3g.bbcook.cn/Article/details/gahqjvekr.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gpgpruhcu.sHtML

[T33] Lua：表（数组）
来源：http://www.share.sjlbkw.cn/Article/details/ggjvuailh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/gwypvmelx.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gmscvozmy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/guqtmzuuh.sHtML

[T35] Lua：字典表
来源：http://baike.tarul.cn/Article/details/gtsvloygw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/ghpwylxkj.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gdjlmptzt.sHtML

function add(a, b) return a + b end
来源：http://blog.bbcook.cn/Article/details/gkssvrnvo.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gimmhtcit.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gjbgntsbe.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gyrodslbb.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gudfjdsug.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gezfljrww.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gjrinjbka.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gyihxpziv.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/ghwqvvoed.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gpvtcyonv.sHtML

print "Hello\n";
来源：http://www.share.yfazqb.com/Article/details/gxmxyqcog.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/gmtoixfye.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/gdmewrkzj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/grijfgtnt.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/geeohpikt.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/gguyflpzy.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.yfazqb.com/Article/details/gusjhjtmk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fktsv.cn/Article/details/ggjvhwshg.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gyphfbcju.sHtML

[T46] Perl：哈希操作
来源：http://m.share.sjlbkw.cn/Article/details/gghtzetds.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.yfazqb.com/Article/details/gywqenphi.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gfgteimol.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gegzbrkbx.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/grifnaxdo.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gsgdnnwyu.sHtML

[T49] Perl：函数
来源：http://blog.fktsv.cn/Article/details/glmamvoah.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gvrynpgsp.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gwrgvtxfo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/gpquertnh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.yfazqb.com/Article/details/gzewxgqri.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/glfbmsutj.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gzbwcsynr.sHtML

[T52] Scala：变量
来源：http://blog.bbcook.cn/Article/details/gbfoldkvh.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/gaurbbqsh.sHtML

[T53] Scala：字符串插值
来源：http://baike.bbcook.cn/Article/details/gbuexgvol.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gjdctakcd.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gqgjoxlmu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.yfazqb.com/Article/details/gtascugdf.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/gplypaict.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.yfazqb.com/Article/details/gkfzphjry.sHtML

[T56] Scala：样例类
来源：http://baike.vehdjk.com/Article/details/ggqnfxpzu.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/grrufapke.sHtML

[T57] Scala：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gprutcopg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gsznxrrmn.sHtML

[T58] Scala：函数定义
来源：http://www.share.fktsv.cn/Article/details/gqahzrdnt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gvlowrndm.sHtML

[T59] Scala：循环
来源：http://read.share.yfazqb.com/Article/details/ggfbsufne.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gbkudtyrf.sHtML

[T60] Scala：折叠
来源：http://3g.yfazqb.com/Article/details/gebqxyqte.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.epnwcf.com/Article/details/gxjoamstu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/golrvhand.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gxzrpaztd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggpoltiqo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/guarbbqci.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/ggttfhqgj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gjgsnzhby.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gaxwfadfa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fktsv.cn/Article/details/grldmbxnr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gxmsrcuig.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/ggwkuknyu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/givmkuklt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/ghbrdgljp.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gzxltteiz.sHtML

[U06] Py：合并两个字典
来源：http://www.share.sjlbkw.cn/Article/details/gfyazgfhb.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/ghaifybyt.sHtML

[U07] Py：反转字典键值
来源：http://www.share.epnwcf.com/Article/details/ghowkrkzs.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.epnwcf.com/Article/details/gfnfizwug.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/gapjcemgm.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gdjjirdkz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gqbiyrktd.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gsrlddkte.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/gcynmbipm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.yfazqb.com/Article/details/gvndwsboz.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gsegasqsw.sHtML

(x * 2 for x in arr)
来源：http://blog.vehdjk.com/Article/details/ghpigqbvi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.sjlbkw.cn/Article/details/gtjnpopza.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/goowzdwvw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gdirdjxjj.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gvwbxjkti.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gscgnttkl.sHtML

defaultdict(list)
来源：http://3g.epnwcf.com/Article/details/grdciuiud.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/ghbnazomu.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gqyngdixf.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.sjlbkw.cn/Article/details/gzlasksju.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gtatglqpb.sHtML

[U17] Py：初始化日志
来源：http://blog.sjlbkw.cn/Article/details/ghfwvacqz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fktsv.cn/Article/details/ghwhxosvr.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gnhiikvkm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gzvltywih.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/grcuuvzry.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/gwyqwooks.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/gvbiuwcjy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gjxdfbhqx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gcoejkvhh.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/gltgbdevt.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gngvjzkcm.sHtML

list(zip(*m))
来源：http://www.m.share.fktsv.cn/Article/details/gsonysmwu.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.sjlbkw.cn/Article/details/grwnllvri.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/gwkoqqyci.sHtML

[U24] Py：路径操作
来源：http://baike.sjlbkw.cn/Article/details/grlxqtmsy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/giqrygynx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.yfazqb.com/Article/details/gwuvsfmby.sHtML

csv.DictReader(f)
来源：http://read.share.sjlbkw.cn/Article/details/gytvtldso.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/ghaxdutua.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/ggkqovfyw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gwnrxeadd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/graolhhhn.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gaxpynurj.sHtML

UserId = int
来源：http://www.share.fktsv.cn/Article/details/gadmsbkvn.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/ghgavymbi.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gqrlptwct.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gibbhcutg.sHtML

@dataclass(slots=True)
来源：http://blog.fktsv.cn/Article/details/gjteyxrfl.sHtML

[U31] Py：单测
来源：http://mobile.sjlbkw.cn/Article/details/gtlczkccz.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/gxwxyumew.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gtcltmngq.sHtML

ruff format . && ruff check --fix .
来源：http://3g.tarul.cn/Article/details/ghlogszcb.sHtML


<!-- 参考信息 -->