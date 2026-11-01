代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gjkpsxves.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gguvtcllf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gzlamgjbl.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gcbiyhogp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gaqboguaq.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gtghosose.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gdilsvsnr.sHtML

[S16] C：位操作置位
来源：http://baike.tarul.cn/Article/details/gvhcxzkxd.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/guycgenti.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/ghgrbjrbt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/ggblewjkz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gmhooyxex.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gbvjgogtn.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gwmybozdz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gfszpoxms.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gluxjcybv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gcrgfntjk.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gcqvchmuk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/gtoqkeimy.sHtML

[S22] C：字符串转数字
来源：http://wap.bbcook.cn/Article/details/gdevnzdvk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/girgbzguc.sHtML

[S23] C：随机数
来源：http://wap.sjlbkw.cn/Article/details/gnopkxmlv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/gkiysenai.sHtML

[S24] C：获取本地时间
来源：http://3g.bbcook.cn/Article/details/gwiuklwkz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.bbcook.cn/Article/details/ggjvllfyb.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gkznvzjty.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/ggthmdjou.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/gocrnoapr.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gmgybskgl.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gzvufdktj.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/glibsocyx.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/gmworbaor.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gogidodkx.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/golkdhdjl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gihdwtgls.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gnahawkxq.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gqvrcyypb.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/guuslrsht.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/griikovyd.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/giqsqzssl.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gyxkwpuzf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gublwspoa.sHtML

[S32] C++：字符串
来源：http://baike.tarul.cn/Article/details/gsqiztqbz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/gaeftmtkx.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gvhmhpmhl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/gvqnryvjw.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gktajhrgq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gktrnnkdf.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/ghvtallyb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/glbukjjpd.sHtML

[S36] C++：unordered_map
来源：http://mobile.epnwcf.com/Article/details/gftrtlryt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gugqqtydw.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtudagum.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gzstlvxfe.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/gtodxstce.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gixukffim.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.yfazqb.com/Article/details/gjgdozmng.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gqaevhjxs.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gjumrtjqj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gwhquxwjz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/gsvpdsgkw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gyigdeuyo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gipopvdbh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.vehdjk.com/Article/details/gifjjtlga.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gzpqvvxlz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/grunbpygi.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/ggcbopybv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/glxgffqke.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/geryhpjgp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/gbrrttewa.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gydbdossw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gvudkldqo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gwvgzxfix.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gimwlmmne.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gnlowitkn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/ggrglthwu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gkcfwvycc.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gapaccsur.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gysdmxtcx.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/gjgylapsg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gtyatbgti.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/ghcjkkfeh.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/ghppmknht.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gppmxbeao.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gbkpialwm.sHtML

[S53] C++：移动语义
来源：http://3g.bbcook.cn/Article/details/gbtwhwcul.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gcxfjcszz.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gljqsefav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gupughvpu.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gzyhfeeby.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gclvhxivn.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/ginnraobi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/grjlsjkby.sHtML

[S57] C++：编译期常量
来源：http://mobile.tarul.cn/Article/details/glpyriubh.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/guuojpywu.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/gykgpmflv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/gmqwxwmlv.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/guzqfwlqk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gzhvjsfdo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fktsv.cn/Article/details/glszqtumb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gtjwieuul.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkczxbdrt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gdgyunwyx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnhhsdtid.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/grsnudssz.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/ghunnhmth.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gazfclqzn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gkojwyrxe.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gdbrenwtf.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gbcqexzsk.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gislkeebc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/ggzmbccwd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gzscoxxbv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/gcwnkhohz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gkptyvobr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gmkxlefpq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/gbvrqzimp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.vehdjk.com/Article/details/gmakncsef.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gyszlflel.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gwbcbmvlq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gjfnsfstp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gqbdzakhf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gctywbhlj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.tarul.cn/Article/details/gezaqgojb.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gqyzzlswt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gysljcjvn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/grzywjkic.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/grymbxvgq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gshnujbea.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gspbktmjn.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gnlikboaw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gkzceovwy.sHtML

[T15] Kotlin：接口
来源：http://mobile.bbcook.cn/Article/details/gnnixtgzs.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gejoltfqj.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gfumlfect.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gnjuneekn.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/gngkpkean.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gkgtgzxan.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gdcnjaqkx.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gdxmugcud.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gdvkrmfwh.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gbxxcboic.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gfsrsemaa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gkhdpcvbu.sHtML

[T21] Swift：遍历
来源：http://m.share.tarul.cn/Article/details/gzmdkrozf.sHtML

for x in a { print(x) }
来源：http://read.share.fktsv.cn/Article/details/gcnchbtce.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/gtavcqzlt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/ggnszpkhr.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/gxdeebtuu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gaowcawji.sHtML

[T24] Swift：闭包
来源：http://www.m.share.yfazqb.com/Article/details/gwgxyourd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gqsbxyrpi.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gznyhmpql.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gmdmjbegx.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gmbbqeggw.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/giqossoli.sHtML

[T27] Swift：错误处理
来源：http://m.share.tarul.cn/Article/details/ggipwyago.sHtML

do { try f() } catch { print(error) }
来源：http://blog.tarul.cn/Article/details/gcfdtsova.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gotxyeine.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/gnjnvtmnk.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.bbcook.cn/Article/details/gjswtdvda.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/gvfnrxuuu.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/gpoevmyxc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gqingsfmh.sHtML

[T31] Lua：Hello World
来源：http://blog.bbcook.cn/Article/details/gsrfxdhsp.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gxdiytjho.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/gdfvxpaxi.sHtML

local a = 1
来源：http://m.share.tarul.cn/Article/details/ggspkyuhb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gtotjufxh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.sjlbkw.cn/Article/details/guyqiqevi.sHtML

[T34] Lua：遍历表
来源：http://baike.yfazqb.com/Article/details/gpisbkmjo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gyjjblayn.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gocuwlclp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gfbjkayyh.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/gcnwyvvrh.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/geeqxmdoo.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gguxcqsrm.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gtfrbcrke.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gsbueprfj.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gpmynbdtq.sHtML

[T39] Lua：模式匹配
来源：http://m.share.vehdjk.com/Article/details/glsriazgt.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gwregacnu.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/gbayfbnpd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gmazkfgih.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gwbjhkboc.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/gpbdmqskq.sHtML

[T42] Perl：变量类型
来源：http://wap.bbcook.cn/Article/details/ggigasxhq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gmstdvzgv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gdtpypkpz.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gqgdarfhw.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gvfahcbnc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/gjajsezod.sHtML

[T45] Perl：数组遍历
来源：http://baike.vehdjk.com/Article/details/glomijecb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/gfkidruwc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/gdbqkgyuq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.bbcook.cn/Article/details/gnxkljfma.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gpwqmksfn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/goucvfgjj.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/gfzampoie.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/grfwpjqpt.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/guxhqcvum.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gokfnqakl.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gobatvquf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gyjawrntp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.sjlbkw.cn/Article/details/grktyhqqq.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gfugmzovp.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gzkersuxf.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/gruglaxlx.sHtML

val a = 1;  var b = 2
来源：http://m.share.fktsv.cn/Article/details/gyypdvlmk.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gnsxltfiq.sHtML

s"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/giivwlkam.sHtML

[T54] Scala：集合映射
来源：http://3g.yfazqb.com/Article/details/gspmhjvbh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/glxoymaui.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/gbgagiwwc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.tarul.cn/Article/details/gtujnvyki.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/gxsavsqed.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gforyyqhq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhcywplb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.tarul.cn/Article/details/gwvjlgbxz.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gdfhzrjlo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/glcylbtcu.sHtML

[T59] Scala：循环
来源：http://www.share.vehdjk.com/Article/details/gaqflpzcz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.bbcook.cn/Article/details/gkncdpqgq.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/gnjfpecwc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gzamqeqge.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwtuazwxw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/glkqfjkbi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glqguwhfu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.yfazqb.com/Article/details/gzlrkayiv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.tarul.cn/Article/details/gywoarjhe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.bbcook.cn/Article/details/goaolazcb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.epnwcf.com/Article/details/gilmnoigj.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gmuubypfh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gfjnjgbcu.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gtsmfzsym.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gmlzsxzaj.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/guolnhhqv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gqunjjpby.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gqkafqhav.sHtML

{**a, **b}
来源：http://baike.fktsv.cn/Article/details/gtabgrexu.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gahbqttnd.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gxxfxmtpp.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gvqfxluvu.sHtML

[y for x in nested for y in x]
来源：http://www.share.fktsv.cn/Article/details/glnbjieaq.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/gupaxvumq.sHtML

max(d, key=d.get)
来源：http://3g.tarul.cn/Article/details/gelcyjous.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gqsrocopg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/gtlrwhlpl.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/gjmfqqjoc.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gvqjhrnca.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.yfazqb.com/Article/details/gxhxwxsnz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gwedewwcj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/ghdylrnbt.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gqveonvnc.sHtML

[U14] Py：分组收集到列表
来源：http://blog.sjlbkw.cn/Article/details/gpsbcymih.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/gsrjzrkuw.sHtML

[U15] Py：高精度计时
来源：http://m.share.bbcook.cn/Article/details/gprvkxovp.sHtML

t = time.perf_counter()
来源：http://m.share.tarul.cn/Article/details/gdfraghax.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gwnptexka.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/gjtwjpaep.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/gesiyorfn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gcfhrzvcp.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gbeansdxq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/guxqxqifp.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gmbqxdsqx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.sjlbkw.cn/Article/details/gkpcpqwzt.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gtekkctdt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gvmtckwlw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/ghctoykoj.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gcnakdznc.sHtML

[U22] Py：矩阵转置
来源：http://blog.epnwcf.com/Article/details/gckpajapw.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/gexmxzutm.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/giprlmwpz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/ghrtevqzm.sHtML

[U24] Py：路径操作
来源：http://baike.tarul.cn/Article/details/guvsleizy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gihkqmnmp.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.vehdjk.com/Article/details/gjiuskshw.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gludodzdg.sHtML

[U26] Py：并发下载
来源：http://read.share.fktsv.cn/Article/details/gklbmhnhx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gzjbjldjn.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fktsv.cn/Article/details/gpshjbfxa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/glsjaeyzh.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/gsxegeksr.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvptnjko.sHtML

[U29] Py：属性校验
来源：http://3g.fktsv.cn/Article/details/gpzpmmibj.sHtML

@property 与 @x.setter 配合
来源：http://mobile.epnwcf.com/Article/details/gcowmzozv.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gbjjsomrx.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gyfkatjlv.sHtML

[U31] Py：单测
来源：http://www.share.bbcook.cn/Article/details/gzgyqkdge.sHtML

python -m pytest -q
来源：http://baike.vehdjk.com/Article/details/glnhwykor.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gfodptmfa.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gyjxjneqs.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gbaguwqsv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fktsv.cn/Article/details/gvtrfizkh.sHtML

[U34] Py：判断编码
来源：http://3g.vehdjk.com/Article/details/gufguuoov.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/guchwrmhf.sHtML

[U35] Py：发送邮件
来源：http://www.share.fktsv.cn/Article/details/gwkmnxeuq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.bbcook.cn/Article/details/gcoyeeatm.sHtML

[U36] Py：定时任务
来源：http://mobile.yfazqb.com/Article/details/gfvddnqiz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.sjlbkw.cn/Article/details/guiqjfqjf.sHtML


<!-- 参考信息 -->