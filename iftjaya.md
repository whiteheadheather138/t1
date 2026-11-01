代发 wailian999

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gevoykbbx.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/ggixdtkur.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gdryvyucd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.tarul.cn/Article/details/gpbqzuuus.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gxpnmbpfz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gooxzupgk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gecnomgqv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/grnpblhtl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gykphtbus.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/glfelngji.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gitulqmma.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/grgfbcfew.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/grdrzecck.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/gbgkrmrgy.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gdctqrdjm.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsjgiijd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/ghwqapvcl.sHtML

[S13] C：宏定义
来源：http://baike.bbcook.cn/Article/details/ghcrvkeiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gdbiihlfx.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/ghqqzvaom.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/grwjyalcf.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gruhuxcgi.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/gamipuebm.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gwonfjeej.sHtML

x |= (1 << 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gdxmqjiih.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gkgsvmpis.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gifbdckzr.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gmnjcvvvz.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gtmuwinwo.sHtML

[S19] C：快速排序
来源：http://baike.yfazqb.com/Article/details/gfitbkezt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gmyovwerz.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/gmqmlfwzo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gdbkxkibn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/glxmqycae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/ggeioenxj.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/grjbxybzr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gbistgvux.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gkyajhtaw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gkdcqgpxx.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gixjkdfwt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gfogwbcol.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gicpiuime.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gmuiisxkd.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gdfsjmpdq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/ggooabfin.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gkzyleeqc.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gcaxlwkdm.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gqpywsduw.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gdxgcpxob.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gycftqwea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gognrvpdo.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gkpibumuj.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gzebrhziz.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gjklvvfqx.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gsqeicauo.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gjrqkrohy.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gihydgqrk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gwrvxvxow.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gifdlpqgr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.tarul.cn/Article/details/gcazzttcu.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gpgvfmmul.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/gdyahchjj.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gcjwsjtdt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/ghklvhiey.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gjniluamb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/guttziwwi.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/groczdtoy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/grxlkkuhp.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/glvwihbhk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gdfbtgpew.sHtML

[S38] C++：排序
来源：http://3g.sjlbkw.cn/Article/details/gzhccsqwy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gcbvxzmpb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gyaukqfok.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gwcrkhgkc.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gvlmmoecz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gudhovvgx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gpnoxjkoq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gqmsoexdd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/ghwaxzizc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/glekjrzyj.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/ggdrfyhyi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.sjlbkw.cn/Article/details/govbqbqhb.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/gxjgnhxhx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.vehdjk.com/Article/details/glpjxdjli.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gqmeurcau.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/ggeavsrtj.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/godvgwoco.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/ghlhzssvr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gmwkfimwj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gbwnexjou.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gsmxruush.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gytgytbvr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gkoonvpfy.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gcqhkdqqf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gywxythmf.sHtML

[S50] C++：格式化数字
来源：http://baike.fktsv.cn/Article/details/gqslqapmm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/gowzkhlqi.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gqkrreoez.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/gvptawffw.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gevtigszi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gjotghnuj.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gvoizpyvl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/ggrmnwasb.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gfsueddvj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.sjlbkw.cn/Article/details/ggepcplpt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gdrjdtipa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gafplkvtj.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gddtqcajq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/glbejwjzn.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gesuiybig.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/gxnilgtfe.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/gjpttnmjz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gckcfzbrj.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gwgruwnmk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/gveenhsok.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gxbhkwcwh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.vehdjk.com/Article/details/grppstcce.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdweltdyy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gfxtqahtd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghfkvpswh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gzgiugcpa.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/grxyaucgt.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/gqbbpghcv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/gbpgfsald.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/grgtgsuzo.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gqnvcesaa.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gsijlgkwe.sHtML

val n: String? = null;  n?.length
来源：http://blog.epnwcf.com/Article/details/gwwxhnzkt.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/giatyotkm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gddnryvog.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gccwxtvhs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/geynkmjlx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gdzjkkyol.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gdujguyru.sHtML

[T08] Kotlin：数据类
来源：http://baike.vehdjk.com/Article/details/gveynucwt.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gwzijlyjd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gkeiekfrb.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gmgdrhrvt.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gyqeemkqm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gjtomukmk.sHtML

[T11] Kotlin：协程
来源：http://read.share.fktsv.cn/Article/details/gyncspxlj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/guuepvzxb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gvapmgake.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gjwyqwdfh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gpsswwwvm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gmgetusvo.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/ghucdmpfw.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gsuxlurml.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/gqdawpzrn.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/grmkbuslv.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gvkxazrmj.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gbquyukzl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.sjlbkw.cn/Article/details/gwmgybwhc.sHtML

var a = 1;  let b = 2
来源：http://baike.bbcook.cn/Article/details/gjyuhtclm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/ghnhyzikg.sHtML

"值: \(b)"
来源：http://www.share.vehdjk.com/Article/details/gfowcvrsu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.tarul.cn/Article/details/gpulaqnqc.sHtML

if let n = opt { print(n) }
来源：http://m.share.sjlbkw.cn/Article/details/gxqyinlbx.sHtML

[T20] Swift：数组操作
来源：http://m.share.tarul.cn/Article/details/gejpulpnv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gnoioynvp.sHtML

[T21] Swift：遍历
来源：http://3g.sjlbkw.cn/Article/details/gckvnivrz.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gblnevfft.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/ghuaxclxq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.epnwcf.com/Article/details/gqrxknjpu.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/gfdxmsnot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gtipczxmd.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/goukhezpx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gdtbobhhw.sHtML

[T25] Swift：结构体
来源：http://m.share.sjlbkw.cn/Article/details/gvgpxemqi.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/glvtapjjk.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gwisoqfhi.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/gvtvruvwu.sHtML

[T27] Swift：错误处理
来源：http://wap.bbcook.cn/Article/details/gdmwxjsxv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/gxgcafrip.sHtML

[T28] Swift：枚举
来源：http://read.share.tarul.cn/Article/details/gnbkkpzpm.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/gvaegwadh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.epnwcf.com/Article/details/gtkbfuqdp.sHtML

guard let x = opt else { return }
来源：http://www.blog.bbcook.cn/Article/details/ggwveddnr.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gplxmhmmw.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gidtcstkt.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gsspphrxx.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gaywjbnym.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gusggqokf.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gragxwanq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gkzsybftr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gqglnrlcz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkynugfp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gbnyrbukp.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/gexwfzoec.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/grojiszyf.sHtML

[T36] Lua：函数
来源：http://blog.bbcook.cn/Article/details/gdgriceap.sHtML

function add(a, b) return a + b end
来源：http://www.share.fktsv.cn/Article/details/grtdxnexv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gkcpopiyy.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gsfpptjcl.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/gtxwhesdj.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gfrbtcien.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gwfvkypqx.sHtML

string.find(s, "%d+")
来源：http://3g.sjlbkw.cn/Article/details/gddzngkyj.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gfwmsejnr.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gjyzvivsm.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/gzxahggho.sHtML

print "Hello\n";
来源：http://read.share.epnwcf.com/Article/details/gdbdtanio.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gokwrgiae.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gjumiuspk.sHtML

[T43] Perl：字符串插值
来源：http://www.share.yfazqb.com/Article/details/guzknctyk.sHtML

"值: $a"
来源：http://3g.vehdjk.com/Article/details/gjbictpiu.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/gxbmhhtei.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gqqlphylu.sHtML

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gylefzvtq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gcifdjjob.sHtML

[T46] Perl：哈希操作
来源：http://baike.sjlbkw.cn/Article/details/gfwvyudxg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/gkhdvsykj.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fktsv.cn/Article/details/ghvekrteq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/ggqdczozf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.vehdjk.com/Article/details/glxzdsbou.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gpfqlzfyv.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gmjzrhzia.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gmhvcywbc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gqhgpjron.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gzgvbmssg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.tarul.cn/Article/details/gedrxdlzf.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gktnpgmxp.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gytxzdidq.sHtML

[T52] Scala：变量
来源：http://read.share.vehdjk.com/Article/details/gsejufvmi.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgvqguqx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gpvnviyoc.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/gaglmtkrw.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gqfdolzhy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gbqcympxc.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gswffnfom.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/grkvnqjpe.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/gkvpbplin.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gtllparry.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gimflhkeu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/guejdcouy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gnsfpikbj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/gulouwrhq.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/gdopwwlaw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gjqiilydw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpkjjboa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gygesbglw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/giscspokz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gphocnleb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxnmudksp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gfbclrzus.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gdmhhlbjn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gidggrcgx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gwxtiaqrj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/gkzpwvhdr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtflhutwk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.epnwcf.com/Article/details/glwsxxyzx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gpunaisyn.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gtwjvpscj.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gfhydnoxh.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/ghmrsnroq.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/ggwuyurev.sHtML

[U07] Py：反转字典键值
来源：http://mobile.tarul.cn/Article/details/gmblzhvun.sHtML

{v: k for k, v in d.items()}
来源：http://baike.tarul.cn/Article/details/guexqvqqx.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gjdtxugrl.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gzayxdoxd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/gykexfiyh.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gfwybghed.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gpneksnja.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gykktvghn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gfajkmhdi.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gieuhphgi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fktsv.cn/Article/details/gvomsrrab.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gzpwseuqp.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/ghdcfgrtd.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/gwbjzqzco.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gmmaszkoi.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gxvbooneg.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gudnpgyyn.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/gvftnuuir.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gnprruchj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/gmklmmsgw.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gquaobucn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gvdxkmyaz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gpplltggh.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/gzayfcbdb.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/gqtjbkrcb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gnmdcgwqs.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/glueulhrv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.bbcook.cn/Article/details/gcstcpcab.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/gulknznww.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/gwtoviinu.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gkesyefsh.sHtML

list(zip(*m))
来源：http://read.share.vehdjk.com/Article/details/ggfkngmxe.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gehmdqozw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gpqpkoyau.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gfwyhgoxp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gvrkxjujn.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gypwrdoju.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gzjctpzmx.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gobbzojui.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.sjlbkw.cn/Article/details/gwkjwmhrn.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/gumcmtsmx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.epnwcf.com/Article/details/gqaqawvsp.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/gdddkkzbr.sHtML

UserId = int
来源：http://mobile.yfazqb.com/Article/details/gyuuxquta.sHtML


<!-- 参考信息 -->