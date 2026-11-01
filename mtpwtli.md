代发 wailian999

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/gzinspzzo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grtfsszib.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gmcmlshyk.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gfxvyxxsy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gyadpilal.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gkxiesubh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gmybsyywk.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/glhxgmxzy.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gvulzqtrg.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/golvhawyr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gewntshog.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/gosvashuy.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gjklbrizl.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gyyyewgfo.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/giuxgdvlj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gcjzelolr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gsdkdhmwj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gfoabxeum.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gerijgxmv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/girpmwork.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/grxsbtoxs.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gxwlxgsqq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/ggxnfmbte.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gcrklgkpq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/gxpnsopcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gdwaokhaq.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/ghohldvct.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gfdrzywtd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gcafyeebc.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gqtfeonqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/gjzgfgmox.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gojgdmitw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/ggwoiuseq.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/gsiucejvu.sHtML

(double) a / b
来源：http://www.share.epnwcf.com/Article/details/gkkrccjlm.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gkbkjvrci.sHtML

x |= (1 << 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbzldzvd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gcxzbigiz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gpeyqgdzr.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gccjgphlf.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gnmeqobzb.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gtnrjiydg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gaxnxdvpp.sHtML

[S20] C：二分查找
来源：http://wap.bbcook.cn/Article/details/gzbnxbbxa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gvlwefmjl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/gpspwzrmn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/gwksjawuv.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gzixfkufd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gkopzkasi.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/ggfppvljz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.yfazqb.com/Article/details/gkpqwghow.sHtML

[S24] C：获取本地时间
来源：http://www.blog.epnwcf.com/Article/details/gscssavzk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gqguuvswq.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gwrvfnmle.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gvrymksqj.sHtML

[S26] C：内存清零
来源：http://www.blog.fktsv.cn/Article/details/gwyrdlean.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/gnhopvngf.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/guvzcrdjn.sHtML

const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gnqzqqvmt.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/ghjljsmhk.sHtML

static int counter = 0;
来源：http://read.share.sjlbkw.cn/Article/details/gfpnkrwmb.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/ggqrqtvhv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gqnynlxtn.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/giezcirxg.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gkprprcvx.sHtML

#define X_H
来源：http://baike.fktsv.cn/Article/details/gzzzlqusa.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gaefhxzzt.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gfvvnbgyk.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gygbjxmpu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/giuvulpwq.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/givgutiny.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gmgtlxuxs.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/glsftnhfk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gyppugmwm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/ghwfpdyow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gtexuofxc.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gwtnvyjhv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gyzrieqvo.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/geqgvcobc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/ghmgyysyg.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/ghhwuheqz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/gocrnbpih.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/glgdphkgl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gtideruqk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/glrsdltmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/ghoxfkrnw.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gtkpndsoo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/gvicusuzi.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/garhaffqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gmhwxsewg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gskkpmctw.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gmdcsywkf.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gjfpidaxa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gudhlqoko.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gvfydgylo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gdgtckxrm.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gqcbkbhky.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gxdcrplpg.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gtoqmzlov.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gzjzdkwdm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gvweojzxb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gqsdmctoy.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/ggnonkdde.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gadwqflgn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gcjqfzffm.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/ggraoanam.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gksilqcnn.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gysyvrmku.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gytlbjozx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gulkehbpc.sHtML

static_cast<double>(a) / b
来源：http://mobile.vehdjk.com/Article/details/grchidesn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gejezgduy.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.bbcook.cn/Article/details/grvijgfqv.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gxsimqmhs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gypyjkqga.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gkonetrrx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/gtrdahmgx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.sjlbkw.cn/Article/details/galahdkbt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gnageutpk.sHtML

[S56] C++：optional
来源：http://blog.tarul.cn/Article/details/gymdfsdii.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gstameldk.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gevlcconk.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/gusaahanv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/gchxsjaou.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gtjccmtfu.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gomxojjhz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/ggdcgincc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gadfevfdi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/ggvcueoey.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghdhxrypq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gypdrvrrg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmsokdrjw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/ghnuzibck.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gxuuvmxcl.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gavrpcmgp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/gdsdjpdih.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gnezwoluw.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gjgltfdrw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gdngybotg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/guqfodmjd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gxmsjmcjj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/gftfxmvne.sHtML

[T06] Kotlin：集合映射
来源：http://wap.yfazqb.com/Article/details/gqvwcehqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.tarul.cn/Article/details/goewnptbj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gfwbmyiex.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gqfuetbbh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.vehdjk.com/Article/details/gurdqkvdq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gngokntir.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gmojmiqxj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gshuetkud.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gexrhbaff.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/gahcluqok.sHtML

[T11] Kotlin：协程
来源：http://wap.tarul.cn/Article/details/glusxaoee.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gluqvkvvp.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/giazuxubd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gqrsropax.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/giscziyzt.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gcdbpbuar.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/gwbuasktq.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/gmsgtygum.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/gkepdwzuo.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gpdwwyltq.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/ggddxtqmz.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gnodharns.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gapdmyqyi.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/grktkstzu.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gxuzghyhj.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gvjjucidt.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/glgcjmmmg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/gfciaquxt.sHtML

[T20] Swift：数组操作
来源：http://3g.sjlbkw.cn/Article/details/gjutvwvci.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gqaovrlig.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gncecabnf.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gltajwmth.sHtML

[T22] Swift：字典
来源：http://m.share.tarul.cn/Article/details/gsaionsme.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fktsv.cn/Article/details/gnktieerb.sHtML

[T23] Swift：函数
来源：http://baike.vehdjk.com/Article/details/gjpddzrbg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/grgozaoop.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/gpqqdopmr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gwlwcyqen.sHtML

[T25] Swift：结构体
来源：http://wap.epnwcf.com/Article/details/gjlgvbtmk.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gxsyysdtr.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/gkzwouygq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.vehdjk.com/Article/details/gfvowtcyq.sHtML

[T27] Swift：错误处理
来源：http://mobile.yfazqb.com/Article/details/glqdxyiju.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gbmdehvvr.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gjszuxlpc.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/gviwenmvv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gkzfkyajg.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/gfntbxicq.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gfwcdgzbd.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/gauislznw.sHtML

[T31] Lua：Hello World
来源：http://m.share.fktsv.cn/Article/details/gcnukmohw.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gslsdxokz.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gmwndwozw.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/grvafqxms.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/geqdjqfyi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gmxpjgzmr.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gyhawembo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gascstuks.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/gdihiryma.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gwyvxlpya.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gnhgwdrfl.sHtML

function add(a, b) return a + b end
来源：http://www.share.vehdjk.com/Article/details/gtrmvdwrk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/gqxzurmap.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gvxnewsgi.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/gjcfifytl.sHtML

if x > 0 then print("正") end
来源：http://mobile.epnwcf.com/Article/details/gubugrrvv.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gyrvtvatc.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/giykiwhov.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gjeswogbj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/giiikiihn.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gfcxspzuq.sHtML

print "Hello\n";
来源：http://www.share.fktsv.cn/Article/details/gpkwrozwt.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gqyxkrmbr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.yfazqb.com/Article/details/gatgctweo.sHtML

[T43] Perl：字符串插值
来源：http://wap.fktsv.cn/Article/details/gmgwvxfnb.sHtML

"值: $a"
来源：http://www.m.share.tarul.cn/Article/details/gptwghjrg.sHtML

[T44] Perl：条件
来源：http://wap.bbcook.cn/Article/details/gkutafiuc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlkytkgj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.vehdjk.com/Article/details/gbbnjgsip.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/gmeislnlv.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/ghumuxkkp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gmgwuxxsx.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gquydzmwq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gxrmkkoqu.sHtML

[T48] Perl：正则替换
来源：http://3g.epnwcf.com/Article/details/gyyglutue.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/guqmekhez.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gnfsumxcl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gwhsuibns.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gcmombwrt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gzbtwfosb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gmglfttdw.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/ghyyoonqi.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gcndzmedz.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gsfmepcqm.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gxnpgzwzr.sHtML

[T53] Scala：字符串插值
来源：http://baike.tarul.cn/Article/details/gxiqfracz.sHtML

s"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gamrdlwol.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gdpwtwtad.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjlhtbajk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gnpvbrqnz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gkkhhuucy.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gyjdnirjj.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gzfwoqhzm.sHtML

[T57] Scala：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gpbecqxlq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/gfwcbtqjw.sHtML

[T58] Scala：函数定义
来源：http://blog.tarul.cn/Article/details/gwlstqzzd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gnpuenslt.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/gyimqfksf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/gknhbhdoo.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/geumghxpa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/gtynbkkmw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdndpbroa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/gkhtlaaiz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsefyemlj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/geewxdxgc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/guuztwuhx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gmwfuzrqu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gozbsviby.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gyzzzosbe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gzainucat.sHtML

[U04] Py：变量调试打印
来源：http://wap.bbcook.cn/Article/details/gogudtfac.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.bbcook.cn/Article/details/ghwywvpug.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gtllivdud.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gopuzegnc.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/grtyyuxrt.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/gtjmkvouq.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/gczlnfrot.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gioubuevg.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gspgtvqug.sHtML

[y for x in nested for y in x]
来源：http://wap.sjlbkw.cn/Article/details/gvspfutvs.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.epnwcf.com/Article/details/gsodrwzlz.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gtdbcyexz.sHtML

[U10] Py：按值排序字典
来源：http://3g.vehdjk.com/Article/details/gitsubxda.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gnewqthtr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gqpizffnn.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.bbcook.cn/Article/details/gawphlzpn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.bbcook.cn/Article/details/gsxexjwhr.sHtML

Counter(arr).most_common(3)
来源：http://www.share.sjlbkw.cn/Article/details/genxrchqh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gkvinhrkz.sHtML

deque(maxlen=10)
来源：http://mobile.yfazqb.com/Article/details/ghaxriuxz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gwftipgqj.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gkikkylir.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/gdbdttnle.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/ggpudsnar.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.bbcook.cn/Article/details/ggmllrjsw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/glueeskay.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gtgrqopug.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gkabjsuxt.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gcbzmvfwt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.vehdjk.com/Article/details/gtodgwzov.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/gkudkqxhw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/goiurxhml.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gknsganhx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.tarul.cn/Article/details/gsrqhoagw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.yfazqb.com/Article/details/gdwnghpah.sHtML

@contextlib.contextmanager
来源：http://www.share.yfazqb.com/Article/details/gelyzpzaj.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gakmcscgw.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/gnylqltpn.sHtML


<!-- 参考信息 -->