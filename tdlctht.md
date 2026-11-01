代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/grfwgbmhb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/ghnntqykd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gmmbgeaoy.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gptptrlhf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gjeummmir.sHtML

[S04] C：字符串复制
来源：http://www.blog.bbcook.cn/Article/details/gzrgtoqjy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/glvucbtgf.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gsematyox.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gyrfsirox.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gyfmvssry.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gbnvidbqj.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gnwpevjkt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.yfazqb.com/Article/details/grdvmcetv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gnksyqcor.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.tarul.cn/Article/details/gjdqjbwgs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.tarul.cn/Article/details/ghunctwzb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gqnfxtyrr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gfemzbgos.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gxezukeux.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gksbbdfjj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/ggiztwpir.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/grmpwmtcu.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/giceehaoe.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/ghrjrzviw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gfutletlh.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gkntvdzgr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/giffmfubq.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gmuyvobma.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gqtsacfjr.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/grolqbqxg.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gbyopgqgn.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gcwldsgia.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/gxealyuyz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/gmyfggtid.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gixvizuif.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gwmvxecrn.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gxyimxmii.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/ggtuskjcq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gzgdvzmth.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gjqasbjvr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gnuixrbsg.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/glrfdtcpc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gjbxadvza.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gmnbvykbr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/giypdpdlu.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/gbwknzdwc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gygktqawa.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gcqzgvfvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gremrjtfn.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/ggdpdmgjj.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gieujonxl.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/ggpfmadof.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/gjtlnblmh.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/ggleitjsp.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gcfybuowi.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gecxrqvqz.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gqokgmajy.sHtML

[S29] C：变参函数
来源：http://www.blog.epnwcf.com/Article/details/gtdhmcuiu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/gjpoethkj.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gyuiaehxc.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gduapdovr.sHtML

#define X_H
来源：http://blog.vehdjk.com/Article/details/gjoyfetbq.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/glopleqgp.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gwhzzcxco.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gqbbkqobi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gaeqtangf.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gftexbjdc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gpfaynhhr.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gssvdzfjm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gnvqizwxb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gbsedvnbv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gkvckmesq.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gosmbnsud.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gyurjnckm.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/goggmbojk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gtdlnjsmp.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/grgpjznim.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/glsexrmsg.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gzwxmlfxo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gfyuczzpc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gwbqphjof.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gadtwwkhd.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gqpurnxzj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.yfazqb.com/Article/details/gwxcuosle.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gaudrjclf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.epnwcf.com/Article/details/gtbyaiwxq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/ggcxgfpqj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gzbechvob.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gmrxbjxwr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gbhvpmdge.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gvndnddjt.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gphxppbfr.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gmtwdjiea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gdrxiekdm.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gcxizylrk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gyzzktmof.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gfhoffjqu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gfebcruts.sHtML

[S48] C++：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gjwqtjkfb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.tarul.cn/Article/details/gjjjwxilj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gzquzuszc.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gdsoisqcb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gldwoqhpo.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gwdvlxmvz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/gseltoinr.sHtML

[S51] C++：显式类型转换
来源：http://wap.sjlbkw.cn/Article/details/giujjdbcn.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/guytgvgis.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gbmrgthmk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gywtbmpmv.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gqoaxuwqy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gsrdakljl.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gvelfxymf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/guiugtclv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gnlzjumes.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gplxmocsc.sHtML

[S56] C++：optional
来源：http://wap.vehdjk.com/Article/details/gxskmqqsb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gfvsnobci.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/gqgoptjft.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/grpkpsqtg.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gsfzaonnp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.epnwcf.com/Article/details/gfuwrdjhx.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gimlzzhhu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.epnwcf.com/Article/details/gbaergsxm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gvjcedugi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.epnwcf.com/Article/details/gujakvgtu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdihsavud.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gszecrjcb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gddjjbdqs.sHtML

[T01] Kotlin：Hello World
来源：http://blog.vehdjk.com/Article/details/gtcoiwwug.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gkydkixfl.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gxnftertf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fktsv.cn/Article/details/gflmjxcxq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/gqmbdgjyc.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gwpmrgkyl.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gzeoylqje.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gwjmzvnjd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gealaayno.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gdedrwega.sHtML

[T06] Kotlin：集合映射
来源：http://baike.bbcook.cn/Article/details/gvourrsap.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gittfsecz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/grfkemnhh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gghprjxus.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/guppgijuc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gwooskpol.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gubgsjvyz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/gpjtdlsdf.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gupugefcv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/gaovrcfhx.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/gjtlmqsex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/giysqfyig.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gkhzvupei.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gojqxzixd.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/gbreroncj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbbgzllk.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/ggppwlsph.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gyafbgcdv.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/gegdddorp.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gmpqbbnga.sHtML

[T16] Swift：Hello World
来源：http://baike.tarul.cn/Article/details/gactsozwz.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/grnyhaypi.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gaiqpjgyq.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/ggrahkhfq.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gluactekb.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gsqnlcidr.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gaxenxout.sHtML

if let n = opt { print(n) }
来源：http://m.share.vehdjk.com/Article/details/gfyyomgsy.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/ghtlvyxed.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gznqficiu.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gygvqxwmg.sHtML

for x in a { print(x) }
来源：http://baike.bbcook.cn/Article/details/glhdhjqix.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gkmhndwqp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.epnwcf.com/Article/details/geotturax.sHtML

[T23] Swift：函数
来源：http://3g.tarul.cn/Article/details/gndktyvib.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.epnwcf.com/Article/details/gvqgeedis.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/guszsjrdg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gocjzpgbh.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gaejnorvw.sHtML

struct P { var x: Int }
来源：http://www.share.yfazqb.com/Article/details/gcxnlzkts.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/geyemrcmk.sHtML

class A: Base { override func f() {} }
来源：http://baike.yfazqb.com/Article/details/gpdweyjbz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/geufycnna.sHtML

do { try f() } catch { print(error) }
来源：http://baike.sjlbkw.cn/Article/details/gnqqsdget.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gtsiqjgcv.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/ggdrrclvb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.tarul.cn/Article/details/gqfoankym.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gejyqbjkb.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/gtzenvptm.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/goiismphm.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/gtvaobzum.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/geudkbpgi.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gbryxqcfc.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/glxzcehvx.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/ghwgodalk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/ggguwuuev.sHtML

[T34] Lua：遍历表
来源：http://baike.bbcook.cn/Article/details/giiambvmj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/glcosdjop.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/gumakpetx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gkxihpxss.sHtML

[T36] Lua：函数
来源：http://www.share.fktsv.cn/Article/details/gtfqkzoxx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gobwvtfyf.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gcfjtimfu.sHtML

"a" .. "b"
来源：http://mobile.sjlbkw.cn/Article/details/gxvpmyfkq.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/ghpiwaxbt.sHtML

if x > 0 then print("正") end
来源：http://read.share.bbcook.cn/Article/details/gpibfuuxf.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/gyfsetkpn.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/gtwhtylaq.sHtML

[T40] Lua：元表
来源：http://read.share.bbcook.cn/Article/details/gbwtlhywh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gmoiiqqar.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gfjvdnxyp.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/glbynetqg.sHtML

[T42] Perl：变量类型
来源：http://blog.tarul.cn/Article/details/gtdipskyx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gobaqdjfd.sHtML

[T43] Perl：字符串插值
来源：http://blog.yfazqb.com/Article/details/gvbdnukgl.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/ghrftltcp.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/gltrfoweo.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.tarul.cn/Article/details/gcxkytrhu.sHtML

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gphvsasgh.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/ghvdrbamh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/gbaxjyqzd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gbgovwank.sHtML

[T47] Perl：正则捕获
来源：http://wap.bbcook.cn/Article/details/gabausuwz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gtcrhffqv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gsdsoicau.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gncamiubp.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gcbjzuqhr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gjfonutsd.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/geerrxoso.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.vehdjk.com/Article/details/gcddiqdyt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gzqhadkrl.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/gczmmpbjy.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/guwjvksht.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gptwqqaqn.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/guaoqbqqj.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gucclrkaj.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gipolqxqd.sHtML

[T54] Scala：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gfhmsxgqg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.sjlbkw.cn/Article/details/gcedzcsga.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gcnpgxdpt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/ghvydjasb.sHtML

[T56] Scala：样例类
来源：http://www.blog.tarul.cn/Article/details/gpzcuahly.sHtML

case class User(name: String, age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gxpcynxgw.sHtML

[T57] Scala：模式匹配
来源：http://blog.epnwcf.com/Article/details/gfjhhxdyj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.vehdjk.com/Article/details/guxdanlat.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gswuoggpi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/ghdisymfe.sHtML

[T59] Scala：循环
来源：http://www.blog.vehdjk.com/Article/details/gxwnwevsq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gyjssxcjp.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/gwtxhdnni.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gmnyemgkp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gijpaaucn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gujwhovgx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gpiedcbyr.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/gxorzqsel.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gtocfosmp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.sjlbkw.cn/Article/details/gsjamoqel.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/gjaxlpaiw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.bbcook.cn/Article/details/gufwbaxht.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.bbcook.cn/Article/details/gkbyvsgfw.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gprwplcme.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gfnkzpnch.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/gesopamuh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gyqlwsuzt.sHtML

[U06] Py：合并两个字典
来源：http://3g.epnwcf.com/Article/details/gsckulidp.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/gqlitxjzn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/gufmmfunk.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/gmadpzyin.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/ghhmqusmg.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gidfmjfmk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.yfazqb.com/Article/details/gtothvbzt.sHtML

max(d, key=d.get)
来源：http://mobile.vehdjk.com/Article/details/guyntrnsc.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gtxrpclah.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gswdsfxtl.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/ggqnkjwjn.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.vehdjk.com/Article/details/gkkpjkwxm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.bbcook.cn/Article/details/goqydndog.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gklaajuvx.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gwvhdthtw.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/gdyqfsjzm.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.epnwcf.com/Article/details/gjmtoeixw.sHtML

defaultdict(list)
来源：http://www.blog.bbcook.cn/Article/details/gzbyrqtuw.sHtML

[U15] Py：高精度计时
来源：http://3g.vehdjk.com/Article/details/ghadkpbiu.sHtML

t = time.perf_counter()
来源：http://mobile.epnwcf.com/Article/details/gtkojbase.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.vehdjk.com/Article/details/gyznehevi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/ghctzldva.sHtML

[U17] Py：初始化日志
来源：http://baike.fktsv.cn/Article/details/grakozfzw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.epnwcf.com/Article/details/glxyuystt.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/gnydhyauw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gjngemyhy.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gslzzzdoj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/gggmopgpe.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gcxptmnfr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.bbcook.cn/Article/details/gkxrputew.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.tarul.cn/Article/details/gpupgenth.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/groupzeff.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/gruoqnbdw.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/gjdumsopy.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/gtebkqggy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgnzedkm.sHtML

[U24] Py：路径操作
来源：http://read.share.tarul.cn/Article/details/gqorksvet.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gncxrbtcu.sHtML


<!-- 参考信息 -->