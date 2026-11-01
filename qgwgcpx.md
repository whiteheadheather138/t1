代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gfavevmlj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.epnwcf.com/Article/details/gezofxbpv.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gndhuvony.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/ggfyspacu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gbirmjdpk.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gdcltleul.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gcostkswg.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gltxzjvef.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gralgjjil.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gbqfsjnmz.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/gxwguhhvw.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/gpdsmyuhx.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/ghglvhjra.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gskbpesjn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/ggoujzrqe.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/garlnkczi.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gbccdtnch.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gifvdeupl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gtvmjcona.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gvyeadqdn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gqnkbtdni.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.epnwcf.com/Article/details/guwnqnuej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gernygtrz.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gachormkx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbtapehm.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/ghnegpcuq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gvqvgwuov.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gjpqufiey.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/goatgrtbh.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/geokxhzaf.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gswnxznwt.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gyktjmyxc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gbkzhvzse.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/ghwluonmy.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gnvthqlre.sHtML

[S28] C：静态变量
来源：http://www.share.bbcook.cn/Article/details/gpkqyjtuz.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/ghojpwhyb.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gbhuivgqq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gojvztjyq.sHtML

[S30] C：头文件保护
来源：http://baike.bbcook.cn/Article/details/gzlcfjugr.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gmjryeizg.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gjettogkb.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gszxzdqaw.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gpcjynwel.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gynmlfqhr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/ghfxbsuty.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/ggnfjkdsx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gfemhsjjo.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/gnyzjlnhk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/goxwnfvgn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gdqhcggvs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gxvhdnfae.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/gullltyla.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gfaipqogr.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gbbvxklqu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gmpotxybu.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gytejhxaf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fktsv.cn/Article/details/gdjluxlha.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/gtfwznuhy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gtytrfymg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gdlnyhezk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gllugaezq.sHtML

[S40] C++：查找元素
来源：http://read.share.bbcook.cn/Article/details/ghypndddl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gtmcmdoub.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gatisyghd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gtdzklsxp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gyxlfcvat.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/grbbslckc.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gskdvpbph.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gkprkqshj.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gyynrcmbf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/glochzgyh.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gwkrrodiz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gqlokfarx.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gsegodmrm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/ghuplqqix.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gohxhcfjj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/gaazmuumo.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gmzmwwyki.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gecbdgwbf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gqpooncbl.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/giuclbdro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/guveqjffq.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gviecllfo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gqhegmkhc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/gwgffqxrl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gqbtuxrdp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.epnwcf.com/Article/details/gfvqjqxfb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gastkdwhe.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gckulwhju.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/glfxzcnez.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gnnpqcroq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gpvmpmkqs.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/glsrppqpg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gridwckyu.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gkeesmbju.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gqumralln.sHtML

[S57] C++：编译期常量
来源：http://baike.vehdjk.com/Article/details/gpoqzktmk.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gxnwcyrya.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gseqffzqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gxdqjnkcs.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/guxrvkesp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gxpjldony.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gakudjvqr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gvnqejfvl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdlqshius.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gftuqmmks.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/goozgxyms.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gznydcxxo.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gryjogjgt.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gzibcdzri.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/ggvtinpxr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/ghqxlbslv.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gcoaeaefz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gmpyipsom.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/gbnofkdih.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/glpzqotwb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/ggnlbahzc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/glxqnhyfq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gkvsgdlpr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/gnvquooma.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/gqrhfqrlp.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gpzegmiet.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.yfazqb.com/Article/details/gbtoudknz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gfckufeza.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.sjlbkw.cn/Article/details/gbgzvjyin.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fktsv.cn/Article/details/gvlgxkakr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gaonacejk.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/grufnytxp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/glxckwfaj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/gtbjxruxz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gmpbqaohd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/guqoaokae.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/gwezhkadx.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gdqklwlox.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gobhaqepd.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gsfmqnukk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/ghjrqovsx.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gifgnlpiq.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gtupuarqh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gmnioeddf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gutqsxkiv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/glldcjoer.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/ggvvklhwb.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fktsv.cn/Article/details/guuxscqch.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/ghwklnnfb.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/gmifqhndg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/gtgbdfpzk.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/gaucoqlhj.sHtML

for x in a { print(x) }
来源：http://www.blog.bbcook.cn/Article/details/gjbuwgvnk.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/grdghfxnx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/giopxlwqz.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/ggyzyflcq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.sjlbkw.cn/Article/details/gpkgoampf.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gqllxxyfi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.tarul.cn/Article/details/gnqvsfgvz.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gupnsoqdn.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gmwafopqx.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/gvylecsdc.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/gxvqzjnfq.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/gtpirxfgk.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gydbnfvfm.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/guwwshowk.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gewdcffze.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gjpldqnwk.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/geoykeauj.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/gperkxtbx.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gtpcqqqub.sHtML

[T31] Lua：Hello World
来源：http://wap.tarul.cn/Article/details/gwhhtuung.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gzeqzwsto.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/ghonymwmn.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gijypkafc.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gnoszaimn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gnjqxgqcu.sHtML

[T34] Lua：遍历表
来源：http://3g.tarul.cn/Article/details/gpqakxjck.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/gtsgjtkna.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gpmccgzck.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.sjlbkw.cn/Article/details/gcayoodvi.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/gpmgnxlaa.sHtML

function add(a, b) return a + b end
来源：http://read.share.tarul.cn/Article/details/greojhimc.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/glbaqxaxq.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gzxxhcjls.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gwehchgei.sHtML

if x > 0 then print("正") end
来源：http://blog.yfazqb.com/Article/details/godybdnhq.sHtML

[T39] Lua：模式匹配
来源：http://3g.fktsv.cn/Article/details/glxmtmnso.sHtML

string.find(s, "%d+")
来源：http://mobile.vehdjk.com/Article/details/gpaycpqus.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/gqcloyiif.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gvjeelaep.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/gjhhmveyo.sHtML

print "Hello\n";
来源：http://wap.fktsv.cn/Article/details/gpwogroqn.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gmbenqnas.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gfaoowuwk.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/gfxeydbzc.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/getemsgow.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gatatebdp.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/gwhnrxhnq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gaqjojopf.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.sjlbkw.cn/Article/details/ggrioarwv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gbiiqigvu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.epnwcf.com/Article/details/gvppihyoa.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/gidbmpdmo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.vehdjk.com/Article/details/gkegkgqhp.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gaeevlejm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/gynlrdikr.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gcosrfbib.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gksurmjqo.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/guwabqrld.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.epnwcf.com/Article/details/gwldhkhri.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/gzoumxcbk.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/govbyxwhc.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gwavuvnxl.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/gvykpgtcx.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/girohmxhz.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gdagsehsu.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gviqnwyma.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gfeeegdpd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.tarul.cn/Article/details/gedemrwmd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fktsv.cn/Article/details/grcvrjyoy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/gzqgfldes.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/grmewphlb.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/gqxzchkql.sHtML

[T57] Scala：模式匹配
来源：http://blog.vehdjk.com/Article/details/gfkzfejez.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/gftkgfuwy.sHtML

[T58] Scala：函数定义
来源：http://mobile.sjlbkw.cn/Article/details/gdbtfofsh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/ghharzwod.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/gpqqhljko.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gczqsdwoc.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gassobdbf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gskmoppps.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmqclfdub.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gflasbwkj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gadasaigw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gwynfgahv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gdtjrbjpv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.tarul.cn/Article/details/gftygyhmg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/gqlzdgovl.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.vehdjk.com/Article/details/gzdfqfthf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gbkieprae.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gzrvatuwh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gilwhvaxe.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.bbcook.cn/Article/details/gzhvafbgf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gcerwlvvr.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/gjmaoyeay.sHtML

{**a, **b}
来源：http://read.share.yfazqb.com/Article/details/gigwjplez.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/gytddxtuu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.sjlbkw.cn/Article/details/gidpmrxty.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/gfcflfkfe.sHtML

[y for x in nested for y in x]
来源：http://blog.fktsv.cn/Article/details/gopdbokpw.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gialyqgfx.sHtML

max(d, key=d.get)
来源：http://wap.tarul.cn/Article/details/gvaudrvbx.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gfuyzpgdl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.epnwcf.com/Article/details/gxjjqrrat.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbkyrxft.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkuzkkshh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/glqeifnzi.sHtML

Counter(arr).most_common(3)
来源：http://3g.tarul.cn/Article/details/gfgwkkrol.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fktsv.cn/Article/details/gbescidhz.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gbbdasfil.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gtumxolrp.sHtML

defaultdict(list)
来源：http://baike.sjlbkw.cn/Article/details/ghcyzgoan.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gnxyrueit.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/gzulucxyf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gesqspycu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.sjlbkw.cn/Article/details/gmoolkvnx.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gabktynyz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gobfahzfc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gbynjgjuw.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fktsv.cn/Article/details/gjlqjjphg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gucrezrud.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gopuhjxom.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/ggvmbcglz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.sjlbkw.cn/Article/details/glwibimnk.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gieymyqun.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gaiwelnnw.sHtML

[U22] Py：矩阵转置
来源：http://wap.fktsv.cn/Article/details/gozmcjhfx.sHtML

list(zip(*m))
来源：http://www.m.share.epnwcf.com/Article/details/gsqvszymt.sHtML

[U23] Py：分块读取大文件
来源：http://3g.bbcook.cn/Article/details/glmnfbqxm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/ghsszypkr.sHtML

[U24] Py：路径操作
来源：http://wap.fktsv.cn/Article/details/grwyvzgkm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/goekuumev.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gdpmpqjtj.sHtML

csv.DictReader(f)
来源：http://www.m.share.fktsv.cn/Article/details/ggosnvxaa.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/gabxwbftt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.vehdjk.com/Article/details/gxqwdnqqw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gcfaddhzi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gkyladqwb.sHtML

[U28] Py：类型别名
来源：http://3g.vehdjk.com/Article/details/gfzsnzeuh.sHtML

UserId = int
来源：http://wap.bbcook.cn/Article/details/gafcuvxme.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gfarxtzys.sHtML

@property 与 @x.setter 配合
来源：http://mobile.bbcook.cn/Article/details/grptzymcx.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gthztwfvs.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/gehpvxlfp.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gusnfxbyy.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/geswscgco.sHtML

[U32] Py：代码格式化
来源：http://www.blog.yfazqb.com/Article/details/ggjwuysev.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/gxzcaonrn.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/gaqqunriw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gkeqchylg.sHtML

[U34] Py：判断编码
来源：http://read.share.yfazqb.com/Article/details/gkgmxnkmr.sHtML

chardet.detect(raw)
来源：http://3g.epnwcf.com/Article/details/gddmxkxgk.sHtML


<!-- 参考信息 -->