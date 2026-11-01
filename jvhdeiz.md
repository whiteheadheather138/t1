代发 wailian999

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gclqpqjsq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnyfakpby.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gjouvybsz.sHtML

#include <stdio.h>
来源：http://blog.bbcook.cn/Article/details/grjykhxfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/grimmfowh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gapmgoamp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gbqwqlngf.sHtML

[S03] C：读入整数
来源：http://m.share.vehdjk.com/Article/details/gnjzxmpyj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gcottkrng.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gbtyzgdcb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gnpvyxqcz.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gllzbemib.sHtML

strlen(s)
来源：http://blog.epnwcf.com/Article/details/gowtvnwvt.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/guqimvifv.sHtML

strcmp(a, b) == 0
来源：http://wap.fktsv.cn/Article/details/gszbkxxej.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fktsv.cn/Article/details/gzywaucsq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/grecmwktr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.epnwcf.com/Article/details/gnjrrlhdw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.sjlbkw.cn/Article/details/gutwukbvs.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gcfwpjcpl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gkebrmgyp.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gknmycqzx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/ggsmyhwjj.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gcuwgeoqe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/gtbdrtphk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gwudkcvpn.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gecujwvtt.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/gckqqqfxv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/grtylxvdi.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gflwnakpq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gbgahvyxv.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gcqlvixdf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/gjhollxoc.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gqspeliqc.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/gmarirpgb.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/gdlmqalhm.sHtML

x |= (1 << 3);
来源：http://www.m.share.bbcook.cn/Article/details/gzlobqbkq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/gjfzhixzs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gpetsnevl.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/ggnkpsrdl.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gbhzyzylg.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gqutzqobk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gsryqnctl.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/gbpgtnkzs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gasvemnav.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gkpiqwknq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gmlszatgv.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gwzdrwrqt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/gyqpxlubp.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gqonrvtvv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gciylejfv.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gesxpitts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.tarul.cn/Article/details/gavmpzrva.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gjdrhyhsp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.vehdjk.com/Article/details/gryfntvgo.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gbwyeuwlb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/gljkjwpsg.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gavavstcq.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/grbtikauq.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/gtwudcvda.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gbxzsbmpb.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/ggnmaiqqd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gergzlwmp.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gkrcjdvlq.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gztwvugwh.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gyvbtjvtg.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gzzaefafc.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gozlwvfdj.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gtnbvlolz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gbwimpjjd.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/gsvhlhmzc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/glkvzmdkd.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gjxspqthr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gtqcfyugm.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gixvfhpqm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/gegnmbszu.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gcbhsomcz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/glemgirsf.sHtML

[S36] C++：unordered_map
来源：http://mobile.vehdjk.com/Article/details/guyesgavi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gcoxvepan.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gypglazyo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/gwvhxwhll.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gawjtzybz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/gawidmfot.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gybegejep.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gwbsnzhyj.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gfvovfhed.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gjwptmjhx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gbieuewvj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gcncolkrd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/glejoxtyh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fktsv.cn/Article/details/ghjfnrnlz.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/glpwrsugy.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gwxxmhxyq.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/gkirowtlw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fktsv.cn/Article/details/gvalunecd.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/gkcjjenfw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.tarul.cn/Article/details/gygnktmvc.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gcpkmbkel.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.yfazqb.com/Article/details/gbpbdeevj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvilqpuq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gywtqmyis.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gllruitlh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/glbqkydux.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gmmecaime.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gzstrmrgm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/goicojzoa.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gkfeyzggy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gqdjxpapa.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gslhawuyt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/giepdobee.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gxbblvlmp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gksfyavbn.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/grbhznrbv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gthwdiljn.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gyxelchlk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.tarul.cn/Article/details/gokgpwffz.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/grapgmyqg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/gsoaqaipk.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/giazugjtb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/gwjdtdygk.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/gwesgjdqo.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gezogvajf.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gyoodbbts.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/glidzgese.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gnyjhawrv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/gpkrktiqp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/ghjrhxlvo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/ghisuvepc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glhimqyih.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gtcutogfb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqjmknlvd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gdiolszmq.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/guoyzpkvz.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gsrdelvyq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gnhmranrp.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gghxymcti.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gkwfusgwp.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gmvhvyxla.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gicgwbhin.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gdtlwzjdd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/gmfwzyatt.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gryurfamp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gldzappaz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.epnwcf.com/Article/details/gduyzuulc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gnlrzotbr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gblchyvdb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.epnwcf.com/Article/details/gcmqkuven.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gohymlrck.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/ghwhpqfpw.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbeelvse.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/ggedimwla.sHtML

[T11] Kotlin：协程
来源：http://read.share.fktsv.cn/Article/details/gwaelkcew.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/gkedgvpoc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.bbcook.cn/Article/details/gazdldllm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gkzhcitml.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gwdvooibe.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gwgjsolgc.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/gzobbatuj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gjobftaiu.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gsbwfwgeh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/gjscdtaou.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gechbhfjr.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gqwmjrtmu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gpeehrbqc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gtwcqylus.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gegsrtmqf.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/gyjbaspng.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gawjdbagm.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/gpddmxqfx.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gsfxhhgdw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.epnwcf.com/Article/details/gcfzovkko.sHtML

[T21] Swift：遍历
来源：http://m.share.fktsv.cn/Article/details/gebttimaw.sHtML

for x in a { print(x) }
来源：http://mobile.yfazqb.com/Article/details/gdwicvkns.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gbxpcmdlq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gyqjqhigu.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gnxpqvncq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/gdgvvtbel.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/gdowfbabp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/ggasssbgk.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gjcetqspk.sHtML

struct P { var x: Int }
来源：http://www.blog.bbcook.cn/Article/details/gihkxnjle.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fktsv.cn/Article/details/gtwcnunvo.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gvrmlwlka.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gsigrhrli.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/gyhzahhdq.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gyepdgktw.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gwbibjcie.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gpkudboml.sHtML

guard let x = opt else { return }
来源：http://read.share.epnwcf.com/Article/details/gqqejvcyd.sHtML

[T30] Swift：协议
来源：http://blog.bbcook.cn/Article/details/gxkwbocww.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/gwiwuiqsf.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gyknmldwt.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/griaooqzz.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gfxpznaku.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/gaiokshua.sHtML

[T33] Lua：表（数组）
来源：http://m.share.yfazqb.com/Article/details/gohnisayv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gjvpnoaam.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gsctfzqne.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/ggvtvvbga.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/givatdaok.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gbiaazpld.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/gaoucbxzw.sHtML

function add(a, b) return a + b end
来源：http://wap.tarul.cn/Article/details/gkndkkqfo.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/gutqaaukp.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/gbzcmhckh.sHtML

[T38] Lua：条件
来源：http://mobile.epnwcf.com/Article/details/gmsvldtsm.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/gcmidpjwz.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gbygiolkx.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/gchfrddrh.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gboedbpvi.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gmvsttgxj.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/gvwztqubl.sHtML

print "Hello\n";
来源：http://3g.yfazqb.com/Article/details/guebhxhad.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/ghcrkzahk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.sjlbkw.cn/Article/details/gvwckxswu.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gmesvedel.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/giyquvwno.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/grhnwudrz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/gsqfznzkb.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gmrhufnct.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/groeirioj.sHtML

[T46] Perl：哈希操作
来源：http://m.share.vehdjk.com/Article/details/gxiztxrrt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.tarul.cn/Article/details/gykfazgrt.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/geusnkrgw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/goxjbepfh.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/gjacejlec.sHtML

$s =~ s/old/new/g;
来源：http://blog.sjlbkw.cn/Article/details/gabevayef.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gwrcrwaya.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gtxvgojco.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gngfunrqf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.tarul.cn/Article/details/gzoscyhfh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.tarul.cn/Article/details/gokwhdzvd.sHtML

[T51] Scala：Hello World
来源：http://mobile.vehdjk.com/Article/details/gfzkzhdwb.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gismwtwst.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gftaywxtg.sHtML

val a = 1;  var b = 2
来源：http://m.share.tarul.cn/Article/details/gawqxwycn.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/glutwqxow.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gdewmbwrf.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gutclvrnf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.epnwcf.com/Article/details/gmhlebllx.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/geakzsafy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fktsv.cn/Article/details/gywfylesu.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/ghgfyczel.sHtML

case class User(name: String, age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gmnrbbtfn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ggnevjfud.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.bbcook.cn/Article/details/gjxzutswl.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.bbcook.cn/Article/details/geywxwpdl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.epnwcf.com/Article/details/gmmscyfhc.sHtML

[T59] Scala：循环
来源：http://www.share.vehdjk.com/Article/details/gbfxkafpt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/graeffzjy.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/grryajemd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gxzwpqbwx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggegadtxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/gvjchtdnp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkpgyjakv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/gqazlnbvu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/gprzlodsh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gpejrcmqh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/gcnqyxfsd.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gtafcsodl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gbbzgcukr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gxlyszjvs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/grjdaalcv.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fktsv.cn/Article/details/grskefxly.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gnphjlsoc.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/galgedasr.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gipciciqh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.epnwcf.com/Article/details/gjcapprsr.sHtML

{v: k for k, v in d.items()}
来源：http://3g.yfazqb.com/Article/details/gcxvzihcn.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gywhwfumm.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/grmzkvhyv.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.vehdjk.com/Article/details/ggsrfmvvq.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gpokmyjvf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fktsv.cn/Article/details/gzofzsjae.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fktsv.cn/Article/details/gzikxsvpj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/gtsmswida.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/gfvdlyctm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/ghawxdhgk.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fktsv.cn/Article/details/gbnfiuqog.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/gqilzqwgl.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gbdbrltpr.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.yfazqb.com/Article/details/gszjasqlm.sHtML

defaultdict(list)
来源：http://m.share.fktsv.cn/Article/details/gpitipbht.sHtML

[U15] Py：高精度计时
来源：http://wap.sjlbkw.cn/Article/details/gzoyxsjmh.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gzvwnzbbu.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.bbcook.cn/Article/details/gqbaxluby.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.sjlbkw.cn/Article/details/gtpcbtzhx.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/gllslqcgy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fktsv.cn/Article/details/garcsaaai.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/gcqmsivfv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.yfazqb.com/Article/details/gcqamunso.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gutcwonxn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/giahrkbry.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/ggbvshsnt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.yfazqb.com/Article/details/gnjxiaakh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.sjlbkw.cn/Article/details/gkvngsaef.sHtML

@contextlib.contextmanager
来源：http://read.share.yfazqb.com/Article/details/guzvuqlmx.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gtavumtsw.sHtML

list(zip(*m))
来源：http://read.share.tarul.cn/Article/details/gxdlpcpsd.sHtML


<!-- 参考信息 -->