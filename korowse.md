代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/gqiwxhfvf.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gjmyjumjn.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpqjrzfk.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gndffpcby.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gqtdmdyau.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gjvmffnlk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/gujosbxxv.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gizeysyaq.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gvcrqefrp.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/glhssjxzo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gasvqpdep.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gjwfzscne.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gczuiipiv.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/ghwyspegr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gangulbur.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gbpdbfriw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gjkiepldk.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gtbleghpd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gpnozmqhw.sHtML

[S24] C：获取本地时间
来源：http://baike.vehdjk.com/Article/details/gnfoogqeb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/ghuozcdzx.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gwtpeqgzh.sHtML

memcpy(dst, src, n);
来源：http://blog.sjlbkw.cn/Article/details/ggelfqymb.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/gzsdcrxho.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gzpqqiyvz.sHtML

[S27] C：定义常量
来源：http://3g.yfazqb.com/Article/details/gounqtvif.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/govcgglta.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/golxoomal.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gsjbgqqou.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gezzcgczo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gekeglmtd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gpwnwybfw.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/glmvsmkyt.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gycyqmmob.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gbltqkvbb.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gohpopceh.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/gptnzwlps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gcfylursb.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gcfygmhjl.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/giojojuqi.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gklyctprg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gkdztxien.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gmgtjnisa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gfahdowai.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/glupjpciv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gncwuwcjp.sHtML

[S36] C++：unordered_map
来源：http://blog.epnwcf.com/Article/details/gcstaikkg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gjjdbaqug.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gemrfmzev.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.yfazqb.com/Article/details/gfdvwbvkj.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gvwprbdmb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/giqtylslx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/ghmdaydzl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/gopaofnnn.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gdywhjmhb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.bbcook.cn/Article/details/gwifzvglz.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/ghcmiasdd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gsyyyzobb.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gyqhwfmoi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/gfhlxkqel.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/gcdwggdkn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/grtdblbrq.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gscqichcm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gbijimjyy.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gdhcznkts.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/gyacdiucx.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gfabojwqm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/ginebckuw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/goruajrhk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/ggpbkxjwx.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gtzmzgdnq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gaccxiugw.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/gchvhobqw.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gqylbkvjs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gjefnknlp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gxuzxnpux.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.bbcook.cn/Article/details/ghnsxgdqh.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gcquzzunt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gprqqihwa.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/gjgmfvsid.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/gsgitfxfu.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gzlimafcq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.vehdjk.com/Article/details/gphsnwyfo.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gsysmphdg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gxujagakx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.yfazqb.com/Article/details/gvfteywep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.yfazqb.com/Article/details/gutlmgift.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gpmcurjti.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gnhxwzttj.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gmatggmxa.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/gljjezlnh.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gtwkwzldo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/ghaymtsxe.sHtML

[S59] C++：静态断言
来源：http://mobile.epnwcf.com/Article/details/gwlbhlmqk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/ggwdwliaw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/gvjormzel.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gqftkpoiv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gewnkfxkb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gbrnmpyjt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbgzknwjf.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gjzcgvhgt.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gakgxyysj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.epnwcf.com/Article/details/goimgccze.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gvixdpcnp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/gyjwmhivm.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gtlujtvos.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/gntcvkloa.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gdnkheakx.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gkklbqhwv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/galexirel.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/gavklrbik.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gmfbklwdt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gfztxnbbf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gctntiofr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gityfguqy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/guhdkkrdt.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/gnkfxzpdn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/gduqivhsh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/glfvcnqwj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/gquiascsd.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gmxolqrff.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gvreqdjhu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gaqwmybaz.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gknksnvjx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gntxrevps.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/grhvgrfxu.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gpndygqnz.sHtML

for (i in 1..10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gkwwakbbv.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gezttqtzf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/gylkjbuje.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gpikovhox.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gfbvgprcd.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gjvtwwurt.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gnysnjcwm.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gfzxlnuyx.sHtML

"值: \(b)"
来源：http://mobile.vehdjk.com/Article/details/gsnoxasot.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/guotzgejn.sHtML

if let n = opt { print(n) }
来源：http://read.share.epnwcf.com/Article/details/greeaaiwc.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gydrnlunq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gtpqpxsvf.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gkeluaygj.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/gxcvjjtou.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/gsnnwthsp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/gptnysvpi.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gjctvnanm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/gztjobucl.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gotuwcbdf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gqqxaxmbs.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gofxzyelx.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gcjykyxfg.sHtML

[T26] Swift：类与重写
来源：http://www.share.fktsv.cn/Article/details/gzowwkbdg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/galucwicc.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gnyqkapgm.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gkhghazny.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gralrwkqj.sHtML

enum Color { case red, green }
来源：http://m.share.tarul.cn/Article/details/gzeoojxhx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/glhedzicn.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gwmsycyzm.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/gfuxzxhsz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gdgivdhei.sHtML

[T31] Lua：Hello World
来源：http://wap.epnwcf.com/Article/details/ggyrvykrq.sHtML

print("Hello")
来源：http://mobile.epnwcf.com/Article/details/gzbkqfslh.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/gdoolzxme.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/gpgkyrwxy.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gjldivfse.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.sjlbkw.cn/Article/details/gwibfslhb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gximlpzpe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fktsv.cn/Article/details/grltcdxtw.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gkdzmqyzy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/gdsweccmx.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/ggogqzxyh.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gztdyhjux.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/ggfbegfse.sHtML

"a" .. "b"
来源：http://baike.epnwcf.com/Article/details/gawgudxmd.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gbhapkqta.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gprrrarqu.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/guvbqvpiy.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gglrykzew.sHtML

[T40] Lua：元表
来源：http://www.share.fktsv.cn/Article/details/ggbmbzkbw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/gomsskxnv.sHtML

[T41] Perl：Hello World
来源：http://mobile.tarul.cn/Article/details/gapvmvjnt.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gwmviwamt.sHtML

[T42] Perl：变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gbwsdpnxs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/gmstxxjel.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gqgrwypdi.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/ghwwlyjdi.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gemhduduy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/goytqbtka.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gaagajils.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/gtzksnwqc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/ghaxhkmer.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gxxvmqhil.sHtML

[T47] Perl：正则捕获
来源：http://3g.fktsv.cn/Article/details/gxdtkeyfd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gshvljsjy.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/ghtynaqtw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gxqomjqqi.sHtML

[T49] Perl：函数
来源：http://blog.tarul.cn/Article/details/gxtobohtu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gvuvizrui.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gbgdvzcru.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/glzoaejbr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.epnwcf.com/Article/details/gfviqvlyp.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gbkndtxgj.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gibkekhvy.sHtML

[T52] Scala：变量
来源：http://blog.epnwcf.com/Article/details/gsoldewin.sHtML

val a = 1;  var b = 2
来源：http://wap.vehdjk.com/Article/details/gcddwcujh.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gihdfduhb.sHtML

s"值: $b"
来源：http://blog.epnwcf.com/Article/details/gbrqfspld.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/ginjfnibg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/glgjwzgmj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gpdijdscv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gkbupikvs.sHtML

[T56] Scala：样例类
来源：http://www.share.tarul.cn/Article/details/gshmxknje.sHtML

case class User(name: String, age: Int)
来源：http://wap.epnwcf.com/Article/details/gwugctjfc.sHtML

[T57] Scala：模式匹配
来源：http://read.share.vehdjk.com/Article/details/grrbebsqy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.yfazqb.com/Article/details/gnemtdxhv.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/grunaxxon.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/ghaskmgbp.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/gcufvticc.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gqeknpuoh.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/glkfdmbrx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/gzoncgaqr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggtgjusps.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/gdqwmkwft.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcywjlwom.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.vehdjk.com/Article/details/ghifkkqys.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gauidohkw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/gjptosyvv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.yfazqb.com/Article/details/gmbxcrxdq.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gobsqbuon.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.sjlbkw.cn/Article/details/gxrycdqhm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/gzxrmdlfs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/gehzmxqea.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gqiijgslo.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gvmswwdvs.sHtML

[U06] Py：合并两个字典
来源：http://wap.fktsv.cn/Article/details/ggfluxehs.sHtML

{**a, **b}
来源：http://www.m.share.bbcook.cn/Article/details/gjxditrko.sHtML

[U07] Py：反转字典键值
来源：http://baike.epnwcf.com/Article/details/ghhzuetsl.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gxnynhpco.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/geeerrygm.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gaaxaldzq.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/guicgaelr.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gcjasrzsg.sHtML

[U10] Py：按值排序字典
来源：http://baike.fktsv.cn/Article/details/gkboualit.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.tarul.cn/Article/details/gmvbyqlyn.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gzodmopwp.sHtML

(x * 2 for x in arr)
来源：http://m.share.fktsv.cn/Article/details/glzhqsmtf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gralddhxf.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gtmuvxbcw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gfamnixpy.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/gwnhomqlw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/guapaiums.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/guezuzqos.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gtsufojmy.sHtML

t = time.perf_counter()
来源：http://read.share.fktsv.cn/Article/details/gxxxojvvw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.epnwcf.com/Article/details/gsgmnawdo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/gvokqvssz.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gckgjapau.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.tarul.cn/Article/details/gxbizfsai.sHtML

[U18] Py：预编译正则
来源：http://www.share.vehdjk.com/Article/details/gpkkwvrju.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gxuatsiek.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/gnqeqswbj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.tarul.cn/Article/details/ghdmltrmk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gdflcqetu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.vehdjk.com/Article/details/gcuukihbt.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.epnwcf.com/Article/details/gzccbzjde.sHtML

@contextlib.contextmanager
来源：http://m.share.tarul.cn/Article/details/gxljkxsfn.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/gxpaissrp.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gmauvgwzr.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/grkxgkjsz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gdzhwuafa.sHtML

[U24] Py：路径操作
来源：http://read.share.vehdjk.com/Article/details/gbwxdqzvh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gcctftkal.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.yfazqb.com/Article/details/gwfcgcgnv.sHtML

csv.DictReader(f)
来源：http://3g.vehdjk.com/Article/details/gudnijbez.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/ghlqfkreo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.epnwcf.com/Article/details/ghztvjebx.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gzqvfvkvl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/grfajldfr.sHtML

[U28] Py：类型别名
来源：http://3g.fktsv.cn/Article/details/gfiwifgkp.sHtML

UserId = int
来源：http://www.blog.yfazqb.com/Article/details/gxijwgagf.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gpjjccelb.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gvnyxuzba.sHtML

[U30] Py：数据类
来源：http://baike.yfazqb.com/Article/details/ggxuuclsj.sHtML

@dataclass(slots=True)
来源：http://3g.vehdjk.com/Article/details/gobmyptqh.sHtML

[U31] Py：单测
来源：http://www.share.sjlbkw.cn/Article/details/gbekhsyxv.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/grcxrgyvc.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gvwmhcdbi.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.sjlbkw.cn/Article/details/gxjcxonwp.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gfaiddbex.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/gzcajiwqh.sHtML

[U34] Py：判断编码
来源：http://www.m.share.yfazqb.com/Article/details/gmgnauuvh.sHtML

chardet.detect(raw)
来源：http://read.share.bbcook.cn/Article/details/gjlhgsydu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/gmfhhrpzx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.bbcook.cn/Article/details/goewoljtc.sHtML

[U36] Py：定时任务
来源：http://www.share.vehdjk.com/Article/details/gzbitjwdi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.tarul.cn/Article/details/gohzdiyzt.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/guqskhapj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gstunjmzr.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/gxabbtaff.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gxukthbfw.sHtML


<!-- 参考信息 -->