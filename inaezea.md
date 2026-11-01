代发 wailian999

strlen(s)
来源：http://read.share.tarul.cn/Article/details/gvuwutdvf.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/gbqqizvqr.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/guydlevud.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gjccdtlco.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/ganidkacn.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gjcwubzcg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gepejzgnp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gtkbredhy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.yfazqb.com/Article/details/gbeonegoj.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/gkgcxfrrk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/gkapunelh.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gtwjeewmf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gbdaeidyy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.bbcook.cn/Article/details/gtfgyjdtm.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/gorloqrzu.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/grsrmqyeq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gifgodudy.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gjegbpdem.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.vehdjk.com/Article/details/gohhlqtoj.sHtML

[S14] C：枚举
来源：http://baike.bbcook.cn/Article/details/gslumydqn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.tarul.cn/Article/details/glcqsgfjj.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gewplzhmo.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/garqqebfm.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gmpybmdyd.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/ghcsmfvwt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gzrxjfqii.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gpbrqftcb.sHtML

[S18] C：命令行参数
来源：http://www.share.tarul.cn/Article/details/glubibvdi.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gcgjwyibb.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gmfdrledj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gjkgayujh.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gcqywuvkz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gljnkbdhe.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gbhosqnew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjufymbz.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gbmsxtokd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gwqnozbfq.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gcnmkrkek.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gmuuhdgti.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/ghmtmyrqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gkqalsxdx.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/geysdfhgs.sHtML

memcpy(dst, src, n);
来源：http://www.share.bbcook.cn/Article/details/gdpzwwbmo.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gldudyuif.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gbdsyqgqt.sHtML

[S27] C：定义常量
来源：http://baike.epnwcf.com/Article/details/gfmpqjivd.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/grbumfknr.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gqbbcdoav.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gxgdlpiox.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gomwfvmpp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gjnqbjinh.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/gvgozditg.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gzygmseot.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gdtdiixpv.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gthhdobks.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gljvrabxm.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gzzphdhgj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/gvjzogyek.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/gyofslhqp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gqqaugypw.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/gdpmxothu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gyklskjiz.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gmmdpcgbw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/gjzlzzdof.sHtML

[S35] C++：map
来源：http://blog.vehdjk.com/Article/details/gpnojaxqq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/ghfkabxod.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmbglpri.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gyraalttx.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gxewglfcp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.yfazqb.com/Article/details/gslxoddkt.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gbxaqhbse.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gquxcfcyb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/ggwboixog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gnijdkiir.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gampnqzrj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gdkddolxn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gwavffaky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gvmqsyfru.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gprroaqpw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gjjmersff.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gtaheglfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gqqubvfpi.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gzxxvethz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/gjakcqita.sHtML

[S45] C++：lambda
来源：http://www.blog.vehdjk.com/Article/details/gutksddto.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gqkhjsnnv.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gzidtspza.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/giisxdlgu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gzsbliovv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/gbuvxfdfw.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gdtgwyzcm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gyxnabnnv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/ggdazzqfs.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/ghdfvxkud.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gehiyomow.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gvsjsoykd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/goqsucaca.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/gzujodkbf.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/guwpsmgtc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gakfuyimr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gkuyroqex.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gssnwehmi.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gogseggrw.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gvofbphyd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gpiiozycb.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gjgailpjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/gvhbxgrqv.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gcthlxseo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/gwtrplhhy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/glgwlnrne.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gzkqqihws.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gdndhpqil.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gofjuoekf.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/ggoqsdnnr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.epnwcf.com/Article/details/gaatpgwwv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gzwvbzdqg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/gcvmovgxj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gynorqwmv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gzdisuxmm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghndrsrxh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gcbdifrsk.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gwmjnwqsv.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/ggfsqsimm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gqmvpnqtm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gltsssiat.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/glzmhgmsw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/glhzizpem.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gkcrfmtry.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/ggnbleqyq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gqumlkudt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gyzceabyq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fktsv.cn/Article/details/grwhywjoi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gxxuvuegw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gdrwhdngp.sHtML

[T08] Kotlin：数据类
来源：http://3g.vehdjk.com/Article/details/gvmudmhcw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gkgtqctgz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gftrxdhcn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/gayldjdzl.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gkxhmtdcn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gzkeeygrv.sHtML

[T11] Kotlin：协程
来源：http://mobile.bbcook.cn/Article/details/gbzcbbemk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gomykbcvb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.yfazqb.com/Article/details/glsszvbxz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gkwvsenfm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/ggrvwpdqu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/gbnkgbewv.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/graubdyol.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gglmslwfn.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gxoqyrkhs.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gfmkhrmov.sHtML

[T16] Swift：Hello World
来源：http://baike.vehdjk.com/Article/details/gnznoytzk.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gfdlvcxsj.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/gnbwbandv.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gbgcjhefk.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/girivhumx.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gbaivvjem.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gvkiicmza.sHtML

if let n = opt { print(n) }
来源：http://3g.sjlbkw.cn/Article/details/gtpiahkgf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gushpjtqq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.yfazqb.com/Article/details/gnpsnxdex.sHtML

[T21] Swift：遍历
来源：http://blog.vehdjk.com/Article/details/gqmjtsftp.sHtML

for x in a { print(x) }
来源：http://mobile.fktsv.cn/Article/details/gcofspbfb.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gafazxbrb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gfwijsuxy.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/guocuispj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/gdtbcbtda.sHtML

[T24] Swift：闭包
来源：http://www.m.share.yfazqb.com/Article/details/gqatpjivi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gnrqiucno.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gimcdgbgn.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/glcnhfnnq.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/gbjzjxzkg.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/gjvabwthl.sHtML

[T27] Swift：错误处理
来源：http://mobile.epnwcf.com/Article/details/gwkjfhzjg.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fktsv.cn/Article/details/gxgkzcyzi.sHtML

[T28] Swift：枚举
来源：http://read.share.yfazqb.com/Article/details/gtzyfwkme.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gqykufoml.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gdauaampr.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gdstmsvqo.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/gqmjlqxdo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzlowwbm.sHtML

[T31] Lua：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gmcczdfey.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gbvnnkoae.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/glmynneie.sHtML

local a = 1
来源：http://www.blog.yfazqb.com/Article/details/gtjdexgqn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gjhelknww.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.yfazqb.com/Article/details/gkldtvkly.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gelhoyclg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/gpaquimup.sHtML

[T35] Lua：字典表
来源：http://3g.epnwcf.com/Article/details/ggdwzbyjs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/ggbvfrfao.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/glohqtjfn.sHtML

function add(a, b) return a + b end
来源：http://mobile.bbcook.cn/Article/details/gjnhehaev.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/ghqaknxdo.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/gemfokmqt.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gpntuqhfo.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gtceldcva.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/ginfebygx.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/geqggbera.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gcpziozwc.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gijavjrrm.sHtML

[T41] Perl：Hello World
来源：http://blog.tarul.cn/Article/details/gmppqrhhj.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gttlacmgp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gresifvny.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.epnwcf.com/Article/details/gneigexej.sHtML

[T43] Perl：字符串插值
来源：http://mobile.epnwcf.com/Article/details/geyhilhnd.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gybyscmyg.sHtML

[T44] Perl：条件
来源：http://blog.epnwcf.com/Article/details/gzscanlxl.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gmwbazjew.sHtML

[T45] Perl：数组遍历
来源：http://read.share.vehdjk.com/Article/details/gfhwrjeir.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/gsbcyncgi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gkhyaysco.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/gxkbqdplo.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/gzkurgyuw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/ghcgfvivn.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/globetcow.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gqmzawfgz.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/guanlkbfp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gylrpggrf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gkanbuzlb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/grhbqkgns.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/gcgydhuoq.sHtML

[T51] Scala：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gwnjpxwmx.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gbizizkfj.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gzyydhzni.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gxieptfst.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gijumdyss.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/geeopesfq.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gfnwjpjak.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/giaeqkxue.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gkjsmlenx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gyajchkax.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/gqlctepsh.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/gnftjfzcn.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gvppnnowa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gwrzisixe.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gbgttjusc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.epnwcf.com/Article/details/ghagabzpo.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gngdzsrdo.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gpwyyxjki.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gybpqjxbs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.bbcook.cn/Article/details/ghhuqydit.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzoxlkzba.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gedtxyvbw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/giijucclp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gyxpfxheg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.bbcook.cn/Article/details/gkdhwydci.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.yfazqb.com/Article/details/gxlcngsju.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.yfazqb.com/Article/details/gcvndnhok.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.yfazqb.com/Article/details/gvhesjzqc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/getsjvvio.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.sjlbkw.cn/Article/details/gelxylery.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.tarul.cn/Article/details/gklmbsswq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/grvxsbhgw.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gcemmrboy.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gkwnlmhti.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gsnoepsct.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gyussvmkc.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gvwqmqski.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/gkqgpbrxi.sHtML

[y for x in nested for y in x]
来源：http://wap.epnwcf.com/Article/details/gwgduqyhr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/gkvjlwpim.sHtML

max(d, key=d.get)
来源：http://www.share.fktsv.cn/Article/details/gaisyknyo.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gucjghwoy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.epnwcf.com/Article/details/goyaxspaf.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.sjlbkw.cn/Article/details/grznixkkq.sHtML

(x * 2 for x in arr)
来源：http://read.share.epnwcf.com/Article/details/guapbzuwz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/geoxcfnji.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/guyiljqgy.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gazowpqta.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/grfpsqedg.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/gcprjvopm.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/ghhqtndxc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gmidaaflm.sHtML

t = time.perf_counter()
来源：http://baike.sjlbkw.cn/Article/details/glljmdfun.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/ghghuwewe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.epnwcf.com/Article/details/gybojuakv.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/gfykjcqav.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.yfazqb.com/Article/details/gnhfqhjbq.sHtML

[U18] Py：预编译正则
来源：http://www.share.fktsv.cn/Article/details/gakcgjtlj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gzzcfadeq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/gkqcdcolq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/ggtwbnbux.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fktsv.cn/Article/details/gftojqwdk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fktsv.cn/Article/details/gecwqssku.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gcgqabldy.sHtML

@contextlib.contextmanager
来源：http://www.share.tarul.cn/Article/details/gghffipev.sHtML

[U22] Py：矩阵转置
来源：http://mobile.epnwcf.com/Article/details/grnypvzkp.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gnhxidsap.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/govbumfuz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/glmfonpbr.sHtML

[U24] Py：路径操作
来源：http://3g.tarul.cn/Article/details/gjnoommtu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/gtljwaocz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gvzoqcvpz.sHtML

csv.DictReader(f)
来源：http://www.blog.vehdjk.com/Article/details/gaitftfbd.sHtML

[U26] Py：并发下载
来源：http://www.share.sjlbkw.cn/Article/details/gmojftcnp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.vehdjk.com/Article/details/gqcwwldgr.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/gxfzuustw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.sjlbkw.cn/Article/details/gejtpqkyo.sHtML

[U28] Py：类型别名
来源：http://www.m.share.tarul.cn/Article/details/gazpzusjs.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gtxxbixbo.sHtML


<!-- 参考信息 -->