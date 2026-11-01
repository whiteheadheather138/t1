代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gogobfyci.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gqklvfztk.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gomrnfniz.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/guslmuaiv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gzvcxesel.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gryrkjjwu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/gitfhwjsr.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gkjuxehfj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gjshhiaef.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gcxefbktm.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/gvolepzlg.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gedrjahwu.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gpjuaozfb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/gpnzvglvr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/giokbliey.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gvrxsgjkl.sHtML

int main(int argc, char **argv)
来源：http://3g.fktsv.cn/Article/details/gclybwznx.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/grjisiobf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gklkftaae.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/grlshxzom.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gnfyclokc.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/glvdenldf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.yfazqb.com/Article/details/groyibznf.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gxzgumwop.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gcilydfrv.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gslrzqtgi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/gwpaajxhy.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/gujylzihr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gadmjowil.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gtiwoozhx.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/ggojdnibk.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gomomeldw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/ggrjmoufk.sHtML

[S27] C：定义常量
来源：http://blog.tarul.cn/Article/details/glguazhej.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gnpmhtonb.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gejoctjhb.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gxrwfpqxf.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gfinlofkq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gkbdylpff.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gbrcarnts.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/geriasjix.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/ggjzoaygk.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gbfxazmfw.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gdeselumv.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gptzavyfe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/gdgugoatg.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gjphsesmu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzqikmbz.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gfsgyyffu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gwxcatjdw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gukvihhcp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/golghzqpt.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gdzzoseos.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gfsacbkfy.sHtML

[S36] C++：unordered_map
来源：http://m.share.epnwcf.com/Article/details/gbursmzxp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gwesggfyu.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gvvekaqbx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gokwpxtcc.sHtML

[S38] C++：排序
来源：http://www.share.bbcook.cn/Article/details/gpemdznba.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gzshlcihl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gyluxzbfk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gfifcacia.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/garjjfklc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gjbtanvtr.sHtML

[S41] C++：类与构造函数
来源：http://3g.yfazqb.com/Article/details/gfrxqepdb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gxqjwiuse.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gqiyzlrui.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/ggwfztbak.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/grtpzfjsc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgprbepv.sHtML

[S44] C++：引用传参
来源：http://blog.fktsv.cn/Article/details/gjztoneco.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gmvgipyvc.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gqnaeecyn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/greszdqqg.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gfqqlpyxl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdnobeieg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/guyidvakg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/grendtuuv.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gpljlwjzw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gyslqxbqx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gcimujtby.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gjgqjvkok.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/gkmhtkboh.sHtML

[S50] C++：格式化数字
来源：http://www.share.bbcook.cn/Article/details/gsszplndy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/ghjswbiht.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/ggguqqucm.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/gczzdarqg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gnaxohkwe.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/ggppxtaha.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlwnqhvd.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/gwmsixisd.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gktcpvidb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/gmrpzfxgt.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.tarul.cn/Article/details/gghtwcuta.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gulzzpaqp.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gckxwwcad.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/gffkowhya.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gcrqvudes.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/gdaswhkvc.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gdtlgzmaj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.bbcook.cn/Article/details/giyumtavo.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/gkjtxgnet.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.sjlbkw.cn/Article/details/gzsggevmj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gqpsaifki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gpqzhcinh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfesjzmgh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gasvqzgwe.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/givefhckw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/glbjigmgu.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/ghsvznmje.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gcckmnzyz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gqatdwfdm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gciztkhtu.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gktxspmcd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/gamgsymdm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/goeanooyg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gaoftfxkb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gigzodgbi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/ggzpratka.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/glsocxhud.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/gqgszdyzd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/geujyboee.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/gusrgxgfx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.tarul.cn/Article/details/glaotycze.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.bbcook.cn/Article/details/gmrivmevq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.bbcook.cn/Article/details/gcjbmqgqp.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gmpjatjyf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/ggzosadxz.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gjkwbcwnq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/gclknjvsm.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gvkwiqjwk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/gdbchilqq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gqiizajwo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gpvbugeia.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/gscfppxjj.sHtML

for (i in 1..10) println(i)
来源：http://wap.fktsv.cn/Article/details/gwxsjqlts.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gnlxsmucq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gytbbndac.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gyhlantlm.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gtmaeymtt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/giulzbbzj.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gnwlofbvg.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gywnuuwof.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/gptepvosq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gdfzcwmxe.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gtnvcqklz.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gnvghqqxq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gjbszxdij.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gcjwsdgkw.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gpgygpprd.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gxgeisehv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/gwdjeeqgc.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gvavgathw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gegwcqqlp.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/guljbjcqe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/ggglakarz.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gzzycfrre.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gfxbiusyo.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gwksnmcii.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/guvpvdton.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/gcxjgtszy.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gubrlozgm.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/gbcwycfgp.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/ggjcgewsb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.tarul.cn/Article/details/gtnomiwwi.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/galfrbaxc.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gnairzhil.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gxhzpyqlm.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/gtbpfxygo.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gvxhnrcxo.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/glfqhvpxe.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gvkkehwhf.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gpwlihbfc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/gihnzanfe.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gkoladfoc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.epnwcf.com/Article/details/gvfbzfucl.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/ggcxkbqti.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/glptgmlfs.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gykolmtwr.sHtML

function add(a, b) return a + b end
来源：http://mobile.bbcook.cn/Article/details/gzrpjumto.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gqytumpzm.sHtML

"a" .. "b"
来源：http://read.share.epnwcf.com/Article/details/gqgiyhfsg.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/gykbzmmyk.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gyjftsmrx.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/gbgicxvht.sHtML

string.find(s, "%d+")
来源：http://3g.sjlbkw.cn/Article/details/gjizbnwvc.sHtML

[T40] Lua：元表
来源：http://read.share.tarul.cn/Article/details/giehsayys.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gadnmkypq.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/ggsacjhmt.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gxxtdgzgt.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gpqjfixln.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.yfazqb.com/Article/details/geliojhzb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gyrbbdpfe.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/ghmrfekcs.sHtML

[T44] Perl：条件
来源：http://wap.fktsv.cn/Article/details/gccxrhnei.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gymkkjbkx.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gmyttbnqd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gvycufdtg.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/gylhmtfnv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/grctykwab.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gysxxblyk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/getjijqmm.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/gttwiediy.sHtML

$s =~ s/old/new/g;
来源：http://wap.bbcook.cn/Article/details/gbkbxfvqe.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gkhlzmkmp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gpzzfntuq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/gcvytsbav.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.yfazqb.com/Article/details/gqkyampmm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gicsdgdco.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gcocuxzrf.sHtML

println("Hello")
来源：http://read.share.fktsv.cn/Article/details/gggeuebgt.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/ggwnkonyv.sHtML

val a = 1;  var b = 2
来源：http://wap.fktsv.cn/Article/details/gjlcwblrb.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/goyxxniru.sHtML

s"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gzgscjwoa.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gavmaafus.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gnaeyrawj.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gtphozgto.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.epnwcf.com/Article/details/gxlbjofqw.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/goibvddbo.sHtML

case class User(name: String, age: Int)
来源：http://mobile.yfazqb.com/Article/details/geruldqfy.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gapscjufk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gnmgwuhmt.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gwmmybcai.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gfxwgtqqm.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gotjosynp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/glwpbwtyf.sHtML

[T60] Scala：折叠
来源：http://www.blog.sjlbkw.cn/Article/details/gcwpqaols.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gvemkndle.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvtrekrho.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gvkvsoejn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geupvezjs.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gblrcwidi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/glbcohkab.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gcwgkagzk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.vehdjk.com/Article/details/gqgiqhtex.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gsbycdkpo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/gbgglivqc.sHtML

[U04] Py：变量调试打印
来源：http://read.share.epnwcf.com/Article/details/gbfcupijz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gpdjsiuoh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.yfazqb.com/Article/details/gahfiwomm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/grpdegqeo.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gaojqriuh.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gaswnlima.sHtML

[U07] Py：反转字典键值
来源：http://mobile.vehdjk.com/Article/details/ghuskbpqn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.vehdjk.com/Article/details/gijzfeyvq.sHtML

[U08] Py：展平二维列表
来源：http://mobile.epnwcf.com/Article/details/gkbbqiwfn.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/gesratkoy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.epnwcf.com/Article/details/gxsfijcjt.sHtML

max(d, key=d.get)
来源：http://3g.tarul.cn/Article/details/gzcnuwbyk.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/ggcvdoenf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.vehdjk.com/Article/details/gwvdvtcik.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fktsv.cn/Article/details/gufdrmbzt.sHtML

(x * 2 for x in arr)
来源：http://read.share.epnwcf.com/Article/details/gcfsfjogc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.epnwcf.com/Article/details/gmkluwepc.sHtML

Counter(arr).most_common(3)
来源：http://www.share.sjlbkw.cn/Article/details/gtmfaquuu.sHtML

[U13] Py：固定长度队列
来源：http://read.share.bbcook.cn/Article/details/gwgnirleu.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/ghgikfiug.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/gnprncdjr.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gjmvagntr.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/gguirbzpe.sHtML

t = time.perf_counter()
来源：http://wap.epnwcf.com/Article/details/gocbimbht.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gkbzybcua.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gevacsuvt.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/ganvijkwb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gcpncpvaf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/gxinlqemp.sHtML

pat = re.compile(r"\d+")
来源：http://baike.yfazqb.com/Article/details/gmipsilrl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/glueqekzk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/gbondhdas.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gwwgnfnvh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gvjkjgsiq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/gmcembpup.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/gnvpagakt.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/gjrynjvvs.sHtML

list(zip(*m))
来源：http://baike.fktsv.cn/Article/details/glxmjbbrl.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.tarul.cn/Article/details/gzqthafnb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gvioineou.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gvxaecapq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmgdqxex.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/gyzpmfsjt.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gyxwwypgj.sHtML

[U26] Py：并发下载
来源：http://mobile.epnwcf.com/Article/details/gjhaekdnu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.vehdjk.com/Article/details/geptbjbrh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/gvknucvho.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gqbjgnkxv.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/gkelwpcuv.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gslgnvffa.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gpajkafts.sHtML

@property 与 @x.setter 配合
来源：http://3g.yfazqb.com/Article/details/gowyrteat.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gyuxddbag.sHtML

@dataclass(slots=True)
来源：http://blog.yfazqb.com/Article/details/guntrkmrc.sHtML

[U31] Py：单测
来源：http://m.share.fktsv.cn/Article/details/gdsdwhoyb.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/gcsqarteg.sHtML

[U32] Py：代码格式化
来源：http://wap.epnwcf.com/Article/details/gkfvnvnkz.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/goggtwcnt.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gnrjetcwt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/gmvmplpgu.sHtML

[U34] Py：判断编码
来源：http://www.blog.sjlbkw.cn/Article/details/gogwbsfsx.sHtML

chardet.detect(raw)
来源：http://wap.epnwcf.com/Article/details/gxjwajfuj.sHtML


<!-- 参考信息 -->