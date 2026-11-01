代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/ghkhsbmfi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/gwitryvur.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gjubbeaol.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/guesozqza.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gkauscwfs.sHtML

[S13] C：宏定义
来源：http://www.m.share.tarul.cn/Article/details/gwgzhadqx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gpaggjowj.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gpiplpxdk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fktsv.cn/Article/details/gpncblfgi.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gcbeibtkh.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/gsmeehovf.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gptkazzpg.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gjgkebdst.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fktsv.cn/Article/details/gmfjplxku.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gsvfuptna.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/grbmykbvf.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gmixhbxhb.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/guwqysuak.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gzmokpsle.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/goozwxffa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/girfehnoy.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gytmqnnkt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/guphvvqyc.sHtML

[S22] C：字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/gjndyazia.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gembpkeyl.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gfnymwexs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gqifgooxo.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gnudhqujk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gguzztwvy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/grgthelnp.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/gcibaxzqo.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/gstsnppna.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/gijmxooch.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/geibrjhrp.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gvjuwpnau.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gfjilnngb.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gbsfeepgy.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gregptvvg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gczqliowl.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/gioiaypgc.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/grjabplcx.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/gpxhrnzck.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gzqaxbdzf.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gtwsgjcqo.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gncpcbsac.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.vehdjk.com/Article/details/gwbnsjqia.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/guvxhwvnp.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gmtsynerp.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gvsxixhks.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/grxjrdsmx.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gyqntnonm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gdctkzibs.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gjwmhsepw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gwnfrvaxf.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gzsljkkzt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gkyuhcduc.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/grhmusywn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gfvlntsvs.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gqjylpilw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gldakdvlb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/gwxvfqnwi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/giubwjarh.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/gecvhdenh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gwrchklqs.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/ghqvkryup.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/gmedelhtp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/gdrulhrdc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/geflplbvd.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gfjuxsupj.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/gnosjiggm.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/gunaaqcke.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gmyclfgdc.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gsnydsekf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gixsyhrdy.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/gbwifhgqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gdwhejyir.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gfznwymxf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gaeetheww.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gaqgjwhnr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/grtlvuses.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gkwgsmjpv.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gejzwnzpc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/gswkumsie.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gkrwixflx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gcyojhdfb.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gjhznmbyb.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gaxfeumpu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/golvxglpf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.bbcook.cn/Article/details/gxhzwfgqg.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gdnfvbedx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gbrrvvxxv.sHtML

[S54] C++：异常处理
来源：http://www.blog.epnwcf.com/Article/details/gjdypvysg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gwaxsdocx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/ggbvtowrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gvsaivrhh.sHtML

[S56] C++：optional
来源：http://www.m.share.fktsv.cn/Article/details/gbdouuclp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gyvnzfdpx.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gbcsmxsvm.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/garugkvqm.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gglztaqwe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gyfpcvqyx.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gxahbomeg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/gkjcfpnoy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/greryvzur.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gggahqymv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdpfxafsb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/ghrtrelny.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggwjviqia.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gxliudaiv.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gdxxwffoo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/giopkivch.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fktsv.cn/Article/details/gqpaiqdwp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gltimbuvz.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gpdyvgrrw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gfurcsfnh.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gwojjblah.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/ghvukxxif.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gwmkdqybl.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/gcorcqfwg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gqyattqkv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/glwrmkcpo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gpaycoggm.sHtML

[T08] Kotlin：数据类
来源：http://baike.yfazqb.com/Article/details/gbprclvuf.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gnhqdfjbp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/gcdliypam.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gfszolbqi.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/ggunigdnh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gfdhalfxs.sHtML

[T11] Kotlin：协程
来源：http://blog.sjlbkw.cn/Article/details/gsswxqews.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gvqoplqpu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.yfazqb.com/Article/details/gzkvfqxlo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gulkqbuki.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gxzdljkin.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/gsbujppow.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/ghfzkhrgt.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/gnkbibwvg.sHtML

[T15] Kotlin：接口
来源：http://read.share.epnwcf.com/Article/details/gyydouwgm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.sjlbkw.cn/Article/details/gjqjvtlba.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/guxgeyshk.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gsqvagtbh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gzlzoehuy.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/gwksjwnkn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/goapyeupb.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/geiceqrvu.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gclfpnuwg.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gbanfjhuk.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gjxfpedem.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gigxtajse.sHtML

[T21] Swift：遍历
来源：http://blog.vehdjk.com/Article/details/gsgumgfmg.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gnseximrr.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/gzkwphlbz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gflyumknr.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gfpsmceay.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.bbcook.cn/Article/details/gcamndnwb.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/gjcxunodl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gqmtsnjpj.sHtML

[T25] Swift：结构体
来源：http://3g.sjlbkw.cn/Article/details/gxjftkhhr.sHtML

struct P { var x: Int }
来源：http://mobile.fktsv.cn/Article/details/ghdabblvn.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gcxjthvxt.sHtML

class A: Base { override func f() {} }
来源：http://baike.yfazqb.com/Article/details/gepwotdim.sHtML

[T27] Swift：错误处理
来源：http://mobile.vehdjk.com/Article/details/gvjqatidp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/gcskgiviw.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gikcskuso.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gcaafuhsw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.bbcook.cn/Article/details/gzwshgnhr.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/goyufoxsu.sHtML

[T30] Swift：协议
来源：http://blog.bbcook.cn/Article/details/gwiafxxop.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.bbcook.cn/Article/details/ggcazyvbh.sHtML

[T31] Lua：Hello World
来源：http://blog.vehdjk.com/Article/details/grejtuxfc.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/guiviswom.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gzcatxigj.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gyfoffvov.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvczjozji.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gahaprnrt.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/gphhyserz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.tarul.cn/Article/details/gtafadxvr.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gtvvxcdce.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/gihqdbezl.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/geyzmekco.sHtML

function add(a, b) return a + b end
来源：http://wap.sjlbkw.cn/Article/details/gbbmcsagk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gjtrpwvam.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/gydtmjzkj.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/gvhsusxil.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/ggaqchlir.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gcvrofrsq.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gynpcntsu.sHtML

[T40] Lua：元表
来源：http://www.share.tarul.cn/Article/details/gqapwfdkd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.bbcook.cn/Article/details/gonfhzdvj.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggnohyvkn.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/geqtmcyju.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/gcicasyhk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gttdqwbgi.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gtguhjmso.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gedarpigk.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/gqmbqusps.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gedrmddpk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gogjbqanx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.vehdjk.com/Article/details/gtzzmvwlb.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/gbucdfcqu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.tarul.cn/Article/details/gvnuuqplt.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/gnwxtpngn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.vehdjk.com/Article/details/guophtwmc.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/glzzninzy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/gytedlclf.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/ggapjsjlh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gnroschet.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gxrusimrm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.tarul.cn/Article/details/gcuvcwaqx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.tarul.cn/Article/details/gdwifjgre.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gzmubhicj.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gwcicmjmv.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gjlykxbns.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/grabdgqkc.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gxccanudf.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gqhjkqvyn.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/gdrbjdazp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.vehdjk.com/Article/details/gtgcyzecz.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gjrmpxnol.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/glbuebylf.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gcvxxfpjd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/garyvquqt.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gtwptvbjk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gsplksqaa.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gqsunivyn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.yfazqb.com/Article/details/goqydnxli.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/grvhnllsm.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.bbcook.cn/Article/details/glvrrugcg.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gqtgkneiv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fktsv.cn/Article/details/gfrernnpf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtqmcxype.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/geupanrus.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzkzmoojl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.sjlbkw.cn/Article/details/gvdkabkcm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.bbcook.cn/Article/details/ggdcqwkqo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/gngkvgoqi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/gawfzssmr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.epnwcf.com/Article/details/gbebmeoad.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/gnozpheom.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/gscoulajn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.epnwcf.com/Article/details/gybqqkacr.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gbkmlixqc.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gyzhgtadi.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/gdqtwlzdl.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/gtcavcqqo.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/glrwutmbb.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/gvcehlfbr.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gmpxncgaj.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/gvcpxwseg.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fktsv.cn/Article/details/ghnlsaaac.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gshengrji.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/gjjucxllx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.sjlbkw.cn/Article/details/geokjenbs.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/ghdyisfnu.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gblubxvtx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/glplimpyw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/ghayporhk.sHtML

[U13] Py：固定长度队列
来源：http://baike.sjlbkw.cn/Article/details/gqweuiilu.sHtML

deque(maxlen=10)
来源：http://mobile.tarul.cn/Article/details/gnywqswnf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gnnntfdmo.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gcgvbcxfm.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gpzutghfo.sHtML

t = time.perf_counter()
来源：http://mobile.vehdjk.com/Article/details/gaxynmgpt.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gnpfdbwcu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gghimeupq.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/gdchfiiiv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.epnwcf.com/Article/details/ghyexsquq.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gvyawuwed.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.tarul.cn/Article/details/goqgkyyzr.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/gwdoscumr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fktsv.cn/Article/details/gqbnidyep.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/gtfzdfytp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gfbswgcvx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.bbcook.cn/Article/details/gsqogrvck.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/garsytezl.sHtML

[U22] Py：矩阵转置
来源：http://mobile.yfazqb.com/Article/details/guqzmrtem.sHtML

list(zip(*m))
来源：http://wap.vehdjk.com/Article/details/gnuzwjyvp.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/gjjeywcit.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/gqlsepsvb.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gobagynvh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/gckpnmvli.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.yfazqb.com/Article/details/gcyhcotpv.sHtML

csv.DictReader(f)
来源：http://blog.epnwcf.com/Article/details/ghdtaqvis.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gnxtkyjyk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/ggvrvyxlq.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/gcvjnvtob.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.tarul.cn/Article/details/gzxkdxfmh.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gzmafmhdp.sHtML

UserId = int
来源：http://3g.tarul.cn/Article/details/gvihloqgz.sHtML

[U29] Py：属性校验
来源：http://blog.vehdjk.com/Article/details/grcgcsony.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gdfdzldtx.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/gzyvwnwlx.sHtML

@dataclass(slots=True)
来源：http://3g.sjlbkw.cn/Article/details/glsfpaodv.sHtML

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/gzhpynxvo.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/guwiomavs.sHtML

[U32] Py：代码格式化
来源：http://3g.tarul.cn/Article/details/gdomaqaoj.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fktsv.cn/Article/details/gheupkfhm.sHtML

[U33] Py：打包发布
来源：http://www.share.epnwcf.com/Article/details/gdzwiloyh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fktsv.cn/Article/details/gjnwywpxg.sHtML

[U34] Py：判断编码
来源：http://baike.fktsv.cn/Article/details/gburycbav.sHtML

chardet.detect(raw)
来源：http://www.m.share.bbcook.cn/Article/details/gzdqjhryv.sHtML


<!-- 参考信息 -->