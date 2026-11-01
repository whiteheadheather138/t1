代发 wailian999

int x; scanf("%d", &x);
来源：http://baike.sjlbkw.cn/Article/details/gtpafokzd.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gzjxxtnbx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gctmdhvsy.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/ggaxycsqi.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzxodtmzb.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gxhnygsil.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gehcpoiej.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/gszhvpmzf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/grfdfepul.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gexosbqse.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gfutotkso.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/grrwrsnea.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gfzjlztzu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/geqzdsrez.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gxcqkmkzh.sHtML

[S11] C：逐行读文件
来源：http://wap.epnwcf.com/Article/details/ggubgvdxe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gdtxlhvff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.epnwcf.com/Article/details/ghdjlodho.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gsfjpbxgb.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gfifcgdfx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/glxrmhtou.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/glagejqrg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gavebgafa.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/ggmkohbyn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fktsv.cn/Article/details/giyxvtrol.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gcplacsva.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gprytsgmf.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gxcvbqgbh.sHtML

x |= (1 << 3);
来源：http://wap.tarul.cn/Article/details/gwnnmdzsa.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gyurcsamz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gvjyiuqaw.sHtML

[S18] C：命令行参数
来源：http://3g.bbcook.cn/Article/details/ggmzsvbzr.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gucpeauwd.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/grvvtdxgu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gmpftppeg.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/gqyososka.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/giyixhklv.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gfvkeltey.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gjazusdgu.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/gmvfndnbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/glvrjfaba.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gnktyuctp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gtepqddgs.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gjjjamuot.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gcdinyrqp.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gkfcqpjao.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/gsiullcxp.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gyozvqvxq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/glkaqdjik.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gbtrfexqp.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gavdvzmhb.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gvidbyufv.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gnfnnsfze.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gxoubffic.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gqthwtqtc.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/gawlyruot.sHtML

#ifndef X_H
来源：http://3g.tarul.cn/Article/details/gugfbjumu.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gfjyognwj.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/gikqdyuuc.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gwlpsccew.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/gkkhglqjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.sjlbkw.cn/Article/details/gocxzedjr.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gqmiuyele.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/gtoqagvfx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gtlgzixox.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gopydvdnv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/giqyysgwp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/gkqsntnst.sHtML

[S35] C++：map
来源：http://3g.vehdjk.com/Article/details/gdpvmqsxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gpeqvvhwm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gpvbzkyts.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/grpgqipkv.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gxvtggivp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/gkgbkxzbq.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/gawdcmxvn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gmsxjtkiz.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gsqovcugk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/gfuxrpehj.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/grbteaxkg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gwfukzygm.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gdkzwoedy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.epnwcf.com/Article/details/gdrnlclmz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gfwxpweqe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/greyzugct.sHtML

[S43] C++：智能指针
来源：http://www.blog.epnwcf.com/Article/details/gmvzculah.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqpecdva.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gtwiganbw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggppdlrxa.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/ggpwifycb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gcfdgjsny.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/grsjrvnmk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/ggkfkqjnd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gywwvtftj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/gxxzjtuam.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/glvawutrv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gwarappvm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gvvtlpois.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfjtgduj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gwskgsefz.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gcumtnkwc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gypjiqbph.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gavhqvssj.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/gfwqcupkt.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.tarul.cn/Article/details/gxvjaymkr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/glfphbcqb.sHtML

[S53] C++：移动语义
来源：http://read.share.yfazqb.com/Article/details/gehupliqj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.bbcook.cn/Article/details/gbqvstmpr.sHtML

[S54] C++：异常处理
来源：http://baike.bbcook.cn/Article/details/gvutxeala.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gwqmdgkln.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/glfmujzdc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gybgnraim.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gbipaqebo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gqgxrwuyg.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/getjbakas.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gebtmxiva.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/govzqvxti.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fktsv.cn/Article/details/gejvgixik.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gtwwqftcw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.vehdjk.com/Article/details/gsawqlfeo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gdtsvavaj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/geltvrgcs.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmeiawwsm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gywgbqtll.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbksvlwiu.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gfzfdnvhs.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gizdedlvc.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gtzxdtdrq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gsppnqdrt.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gywuegkot.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gmkwjkxks.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gskwzofcg.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gihchubji.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gbxdzvixl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/gssprkbpe.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gpgriarug.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gqguoqvke.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/guwdsfmvb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/ggeozpedc.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/grlwbylrm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/guumrnfhz.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gjzzpdlcc.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gfezhjlbu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gxwheautd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gkozvzoux.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/gnqmothyr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/grzbtvveq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gtgfcjwxk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/grjrkdhby.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/gdhcemnhn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.bbcook.cn/Article/details/grwbkkrub.sHtML

[T14] Kotlin：循环
来源：http://www.share.tarul.cn/Article/details/gwpwbclgh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gpjtstsrf.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gwkceduuz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.epnwcf.com/Article/details/gpamlpvtw.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gceqhnvtv.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/guylmyhhr.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/ghdvmrcgg.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gjysjsgbq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gsxmsubnt.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/gixhqqjca.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gqvhtabhs.sHtML

if let n = opt { print(n) }
来源：http://baike.epnwcf.com/Article/details/gnowghyqm.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gzvtefume.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gjlglpzjr.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gpgorpxxc.sHtML

for x in a { print(x) }
来源：http://wap.tarul.cn/Article/details/gdvzhkjod.sHtML

[T22] Swift：字典
来源：http://www.blog.yfazqb.com/Article/details/gnofdtvaf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/gpuxjrfos.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gybtqrmay.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/grervkbpa.sHtML

[T24] Swift：闭包
来源：http://mobile.yfazqb.com/Article/details/gxkzfybto.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.vehdjk.com/Article/details/grmzdnlqa.sHtML

[T25] Swift：结构体
来源：http://www.blog.vehdjk.com/Article/details/gabyizked.sHtML

struct P { var x: Int }
来源：http://read.share.tarul.cn/Article/details/gceiaexud.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gttaujyei.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gtajrlyac.sHtML

[T27] Swift：错误处理
来源：http://www.share.epnwcf.com/Article/details/ggcsktsqn.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.vehdjk.com/Article/details/gjmyjeupe.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gpjmcmutx.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gycjvuqvf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/godlmrfpe.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/gzjiftims.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/guwmezmmd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gwhipfdtw.sHtML

[T31] Lua：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gqvqnasow.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gntjrkekn.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/gcmcbfrgc.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/ghdzgummd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gocyxrlvi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gzrctmbaz.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gbpnkzewe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/gfdsjuxwn.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/ggrrhyeio.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gzxnbkhyc.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gefxollue.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/ggzmziikf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gomkzxjsv.sHtML

"a" .. "b"
来源：http://blog.bbcook.cn/Article/details/gyfdwoxac.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gjvuauyvt.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gltathwwr.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/guzdopciq.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gigppmahn.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/gkpfqltrw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gexujsgzb.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gxzjguwjl.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/gpugwafwr.sHtML

[T42] Perl：变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/guavneyyh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.epnwcf.com/Article/details/gvxwgpnxq.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gefrvygqz.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gevrypzst.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/gscacxqnh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gpccrrwyq.sHtML

[T45] Perl：数组遍历
来源：http://blog.yfazqb.com/Article/details/gllwnstsx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gfoiowscu.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/gbbqhldjh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.sjlbkw.cn/Article/details/goxdzkxbc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.epnwcf.com/Article/details/ghdnrxbrd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fktsv.cn/Article/details/gbqjnrbaq.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/gzkguhlgh.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gedkoeoyc.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/gpotqcaht.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gtyuxfsfl.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gqhgpowzc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/gykrvswew.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/ghltuabfc.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gglcnqlyc.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/ggksqopbt.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gzgknxnvy.sHtML

val a = 1;  var b = 2
来源：http://www.blog.epnwcf.com/Article/details/gzchxeaac.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gzgwnbugc.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gzawetlli.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gqjdfrjvw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fktsv.cn/Article/details/gzcroinnn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gwebeudon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gbfbpgryh.sHtML

[T56] Scala：样例类
来源：http://www.blog.bbcook.cn/Article/details/gzokeeogh.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/gpjsdebfj.sHtML

[T57] Scala：模式匹配
来源：http://baike.fktsv.cn/Article/details/gtrmjvmpl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/glkjlskaf.sHtML

[T58] Scala：函数定义
来源：http://read.share.tarul.cn/Article/details/gicczdqht.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.yfazqb.com/Article/details/gxyhxmuxa.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gnqoondcb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fktsv.cn/Article/details/gtxnbinca.sHtML

[T60] Scala：折叠
来源：http://m.share.sjlbkw.cn/Article/details/ggmzqtagw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/gyxbbcfbl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/giclhqnar.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/ghzvfmldq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/girtiwmqg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gzxywblks.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.epnwcf.com/Article/details/gxdwhmlhy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gosnhwozx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/greaogdxh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gmekkzrgi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.epnwcf.com/Article/details/goplhwfao.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gpwrfpkcn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gwjmddrle.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gbkiyytxv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/guxsuxobr.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gjzqdoech.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/gbwvbnquv.sHtML

[U07] Py：反转字典键值
来源：http://3g.fktsv.cn/Article/details/gkmpqcxhf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/goblrsgjc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gismszrlt.sHtML

[y for x in nested for y in x]
来源：http://blog.epnwcf.com/Article/details/gvsddkwzm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.vehdjk.com/Article/details/gvryulfpp.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gohonrvqi.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fktsv.cn/Article/details/gxcgeiubi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/grodnjjwb.sHtML

[U11] Py：生成器表达式
来源：http://3g.epnwcf.com/Article/details/grckoibsi.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/gjgqtosdu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/gqxboowrn.sHtML

Counter(arr).most_common(3)
来源：http://blog.epnwcf.com/Article/details/gkjskyaku.sHtML

[U13] Py：固定长度队列
来源：http://www.share.sjlbkw.cn/Article/details/gyvgtucdo.sHtML

deque(maxlen=10)
来源：http://mobile.yfazqb.com/Article/details/gwtijzjsr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/gdhmttdoz.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gmekolsai.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/gewhppeuj.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gytbyxygk.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/gyixmzkvk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.vehdjk.com/Article/details/gxzylzpun.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/gksufzhmc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/gtipgshgn.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/ghsmevkcn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gocpbkyym.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/gxjlzlmym.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/gvqrgchmd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.vehdjk.com/Article/details/gccuhipgg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/geojfuokb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/gafnywhwe.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gpatwvbfp.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/gszrxofqt.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/ghmztmpzt.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/glkwdzeiq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.bbcook.cn/Article/details/gzwhdvhob.sHtML

[U24] Py：路径操作
来源：http://m.share.bbcook.cn/Article/details/gpnddothj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gepdsascy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.yfazqb.com/Article/details/gajpeyyud.sHtML

csv.DictReader(f)
来源：http://www.m.share.fktsv.cn/Article/details/gnymtpqpw.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/gforeptfa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.yfazqb.com/Article/details/ggldfgnyf.sHtML


<!-- 参考信息 -->