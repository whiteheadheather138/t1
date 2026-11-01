代发 wailian999

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gadgltgsp.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gvzhoindr.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gsvplsbxd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gnsqsrkca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.vehdjk.com/Article/details/gadqocano.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gzdjqjnfj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gkbpetfoj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.tarul.cn/Article/details/gnbpjeyre.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gutnebrtt.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gqgmbsgge.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gryxrsfdz.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/ggyvaubqc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gvowozqhd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/giuxukflz.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gjjcauycg.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gaieejujy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gzfmcgupu.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/ggpflsabn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gruhuxmfx.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gctbqrjxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.sjlbkw.cn/Article/details/gognptvgd.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gkjqkkevk.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gmkmzppxl.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/gszqnjovu.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gjhwecusu.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gwxozosro.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gucszfajm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gvsqkgouh.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/gqloutron.sHtML

[S19] C：快速排序
来源：http://blog.vehdjk.com/Article/details/gvojgjyac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gievbvhoy.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gcvytqtpi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/guzffjjyi.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gicbwharx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.epnwcf.com/Article/details/gxpiyzygn.sHtML

[S22] C：字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gqukibpdy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gvgggwpdm.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/ggajvjiyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gnzqvwsrc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gptgttiog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gmnthpexs.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/gcqpsvcqy.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gwllxgizm.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gintgrelv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gjyqbubuq.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/grbpcrqdk.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gdhwriust.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/gcwbditvx.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gqxoszhop.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/grfbkotjm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gbkfuslkd.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gekpojetx.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gnvahhdrn.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gzpfdghko.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/gauwalqle.sHtML

[S31] C++：Hello World
来源：http://www.share.bbcook.cn/Article/details/ghgphnqnz.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/goydvtrps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gcxermdfv.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gfdfokaup.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gcymctddh.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/glrvmstnm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gwabcbnsj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gssgzkfkb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/girsszifh.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/gbyfjdvlo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gughyivpw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gbupfnimq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gbgnzeeao.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gcxkgvpxl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fktsv.cn/Article/details/gdgcbeuii.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gjqomwrtr.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gijfuqacl.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.sjlbkw.cn/Article/details/gxlukxhyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gfyrcwaqw.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gucrpmwld.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/gvmkjidcm.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gcvoosexv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gldzzofcq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gcxrmherz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gtuunxloi.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/glkgpoeac.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/ggfiqakqb.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gtbholmmz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvokpeovm.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gwqjiungj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.bbcook.cn/Article/details/gfirkgjzw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgvakjru.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gutsegmgz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gjkucufbm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gwzylcfgg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gzkfesmly.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gziqobrlx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/grdqodvtw.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gaubwsnzh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/grzsszemy.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/glchqdcrt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gvdiwaris.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/giloprhky.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gnilscfbv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/ghshfeikx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gxjsjrnmj.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gnrzpuizr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gtqtjdzps.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/ggrardfxl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/glxrxwdcb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gwlujfpib.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gaopvwasp.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gauxxbkmi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gfzpzbuke.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gysuqtpqp.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/giszhubpq.sHtML

[S58] C++：命名空间
来源：http://www.share.tarul.cn/Article/details/gespxxrcu.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gvfkpperz.sHtML

[S59] C++：静态断言
来源：http://wap.epnwcf.com/Article/details/gjhwhxnpg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/grndlpbak.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gwgjqhqec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/gqkkusifl.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnoongpjc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/gaxkjxudt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/greqfwsey.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gklbehrjl.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/grlkmtujl.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/glczzdjsl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gdvusbiyb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gjuspukoc.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gncsqnbea.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gaugpyvle.sHtML

val n: String? = null;  n?.length
来源：http://www.share.epnwcf.com/Article/details/galcphbzt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.bbcook.cn/Article/details/gbzvzpwml.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gorsezwad.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gggghetpe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gbgqqzjmo.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gnteercnq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gpbxxfuic.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gziehdbdu.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/ggtosjdra.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gcelskblz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gnqqhsask.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/guygukssl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gsbxeidje.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gkqjekflo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/guasjekea.sHtML

[T12] Kotlin：解构声明
来源：http://baike.vehdjk.com/Article/details/gapneqwqs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gfivgfufx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/grnltrbds.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gvdadijax.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fktsv.cn/Article/details/gxdrapjsi.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/geprgsnpg.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gebgdqknl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gmkqachxx.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/grxuqhqtg.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gemzccwkm.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/giwdloxfj.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gayqhydqh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gycaualbv.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gedueroxb.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gbodexwjh.sHtML

if let n = opt { print(n) }
来源：http://baike.tarul.cn/Article/details/gwihrrbay.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gcnhlydoi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gdcnontvm.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gfgheobjo.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/gcjvkitqb.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/gaobbchru.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gsquqjckj.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gnhlbseii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gdccojwyd.sHtML

[T24] Swift：闭包
来源：http://3g.epnwcf.com/Article/details/gipbjvoiv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gnoofbxpi.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/gkoqqjhpx.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gtnbnkpyd.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/goooodnzd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/gvufjlrpx.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gevsfuwvk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/gnpylqxsq.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gpujqiunl.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gdhbgaywx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/goxpnttsg.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/gtnwdibfy.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/giimdfvud.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gkiyasqih.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gcznvkkca.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gkpymqwvf.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/gneeubleq.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gjuvesiej.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/gjvzoslnw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/gucdfxluy.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gowczsult.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.sjlbkw.cn/Article/details/gjjycnthk.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gyabhsxbl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/gtjoefbuw.sHtML

[T36] Lua：函数
来源：http://www.blog.epnwcf.com/Article/details/gpqdataps.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gdoeegmro.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gmrvosjmt.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gpmpcwlhu.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/grjxqjnop.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gagqjmzvp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gkijvrsya.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gssmjohqr.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gkwqehasl.sHtML

setmetatable({}, { __index = base })
来源：http://wap.vehdjk.com/Article/details/gmvmeiifv.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/ghkeejswu.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gntlipgxu.sHtML

[T42] Perl：变量类型
来源：http://baike.yfazqb.com/Article/details/gywqgahki.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.bbcook.cn/Article/details/gughfxwzl.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gdtbkxlln.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/guqkeghyy.sHtML

[T44] Perl：条件
来源：http://www.share.fktsv.cn/Article/details/gbgblmtnw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/gikxfelbb.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gzlnyyeig.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.yfazqb.com/Article/details/gtnxcotgl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.bbcook.cn/Article/details/gqsvvywyd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gyyshomeh.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gpdcdcvuf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/gceikihhr.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/giweetqry.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/ghnjkumyf.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gxmhojcpg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gstxatldk.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gznryuxvs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gaglquibk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/gikmwyuqe.sHtML

[T51] Scala：Hello World
来源：http://mobile.epnwcf.com/Article/details/gtcjtyxct.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/giwpuqmfd.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/guckpyxyq.sHtML

val a = 1;  var b = 2
来源：http://3g.yfazqb.com/Article/details/gzctojmgc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gtuiyfpuj.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gvagnlvrp.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/girzxlrtc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/gdkgonxix.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gaqedveap.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.tarul.cn/Article/details/gyjrbgbzd.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gsfvpakqx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gxsecqxhx.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gcofvehnd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gkbgarfjo.sHtML

[T58] Scala：函数定义
来源：http://m.share.yfazqb.com/Article/details/gkdnsbeao.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gimehmotf.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gydvxixep.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gmplpzgdj.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/godlfpeme.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.yfazqb.com/Article/details/grmxjwijp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gittlteay.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/ggdisubrh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqivzuche.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gfxexconu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/gnoycsioc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/grfqarjsi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gcerpdnlt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.tarul.cn/Article/details/gnqbtwzmc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.tarul.cn/Article/details/gsxvehtxa.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/gotqufrpa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.yfazqb.com/Article/details/giqgcnzpg.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/ggiocrbta.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/govjernoz.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gyndnzfht.sHtML

{**a, **b}
来源：http://baike.epnwcf.com/Article/details/gixoslhif.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fktsv.cn/Article/details/gumhbyslg.sHtML

{v: k for k, v in d.items()}
来源：http://baike.vehdjk.com/Article/details/gsvxpnxrr.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gknspsrnm.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gkdujmslq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.sjlbkw.cn/Article/details/gfnxmatxc.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/gbozrtdgz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.sjlbkw.cn/Article/details/getedusop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gxumydnnh.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gntghueek.sHtML

(x * 2 for x in arr)
来源：http://blog.vehdjk.com/Article/details/gzhljnlsg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.yfazqb.com/Article/details/gaewnykwv.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fktsv.cn/Article/details/ghjlatwbx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/gzjybnnpc.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/gtvakuuxa.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fktsv.cn/Article/details/gziaxgewk.sHtML

defaultdict(list)
来源：http://m.share.bbcook.cn/Article/details/ghcysggeh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gpxbgakdc.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/glrdotdmh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/gndngfptr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/gvxwrawye.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/ghjdlmeca.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/goffhcdog.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gwfcfexea.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/gpvmxjibs.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/gkmwtlppb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.sjlbkw.cn/Article/details/gmssovrlk.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/gqbiofmvj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gneybhdoc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.bbcook.cn/Article/details/gfgryrswo.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/ggznrptnv.sHtML

[U22] Py：矩阵转置
来源：http://read.share.sjlbkw.cn/Article/details/gfkngwmfh.sHtML

list(zip(*m))
来源：http://www.m.share.tarul.cn/Article/details/gratlnkhs.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.bbcook.cn/Article/details/gxobcheox.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/gpmlunlue.sHtML

[U24] Py：路径操作
来源：http://www.blog.bbcook.cn/Article/details/gauxntgwc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gbkusalpc.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gsrepriqa.sHtML

csv.DictReader(f)
来源：http://www.share.bbcook.cn/Article/details/gdgebodkx.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gssqyjkgb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gkvupyytg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/geuhmwogq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.epnwcf.com/Article/details/gwjmpqtbh.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gmdwqtnvi.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/geobxpczk.sHtML


<!-- 参考信息 -->