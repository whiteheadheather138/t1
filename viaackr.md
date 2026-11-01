代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/goeucrjol.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/ggtvhaxky.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gbgskqikk.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/glzaqihnq.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gbrszonmv.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/gvooxlxzo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gmqmzwbhu.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gkpqlpupg.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gxllycrjm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gguywzxpy.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gpmirxtoq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/gvlrscvtk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.vehdjk.com/Article/details/gcpwobmpr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gvipnwdan.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/giiivpuar.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gzaugqgbr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fktsv.cn/Article/details/gzyjzoazs.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/gtnvanctw.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gfkqplenf.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gwtsmgbnh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gyfxaxquq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.vehdjk.com/Article/details/gxktcnwcl.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/giqbrigla.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gwrvljgvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gxtmtxkxo.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gyxaizmsc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/ghgwxwybw.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gkijygync.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fktsv.cn/Article/details/gdgjozqrs.sHtML

[S15] C：类型转换
来源：http://mobile.vehdjk.com/Article/details/gfkjbxdpg.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gqtwhlbnh.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gcfapgplc.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gykqrfglt.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/gfvgkzveu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gdlatrbkc.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/ghxtaqwyg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gxvlqknas.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/gpqhdtaob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/grirsokbh.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gryojjspo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gcfwtpgpj.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gauhtzvvg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gsphzvvls.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gdqrdjwnx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/grndkbexi.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gtznsrbtj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gmaheyzcc.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/geftvgppz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/grqjqycpa.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/gpmndkhkr.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gkqyhqina.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/glpzconaq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/grrskypyw.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/ghvbfiftu.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/govlupilg.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/gwhubvmae.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gbiwtuwsh.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gyargcmwi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gasccmlyy.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gkgmndgny.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gxkdpuhkb.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/gqazmozlp.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/goizkcqyy.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gonnsmrmq.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gjyupurvb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gzuxaghmq.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/ggakricuf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gikdrfrle.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gaxcukiql.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gjhrplklb.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gzdtgiqlu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/gdxfikjow.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gxqjrfupr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gpcohmopc.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gbwdsfmpn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/geijbsbzd.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/gqlhpljlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gmdbvsbwh.sHtML

[S38] C++：排序
来源：http://www.blog.yfazqb.com/Article/details/ginqnkknm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gkbesxaou.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gewktlnzr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gdqcgjqmq.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gzgglplow.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gimipwwsv.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gmfygswpt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/guhzregjv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gdcbdyiwn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.epnwcf.com/Article/details/gbawavvkk.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/gctakmcmr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gkwqkfoby.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/gukkazerg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/giepyajnt.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gceceorum.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/gjqmmtjnk.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gjeixvfem.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gemxzjgjf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gkpclltqs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gqbthqwxe.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gmvjzfilt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gtfyejlmx.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/geiwhnoqn.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gvzvkqcjt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/ghhhslgcv.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gljlxqpug.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.vehdjk.com/Article/details/gomfcxjcu.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gzpeerirz.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gprwsiyqi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gzrtlsqcu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gvzyodqlk.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gaolrynld.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gjmaxvhdy.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/glllxiwsz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gpsojqkyy.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gpzahcvjz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gymxfwovg.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gsbkqvyqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gpwtgpfsw.sHtML

[S57] C++：编译期常量
来源：http://baike.vehdjk.com/Article/details/gtfhwfzkx.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/gpboyedmd.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/goqtbwsdg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gscwdkgcn.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gtymceket.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/giswyqarr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.vehdjk.com/Article/details/gmmgubsmk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gmcywqwub.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcbqwguf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gudnqiawk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gcsnelwwv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/grdwzbbhg.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/glxcfvrfc.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gjiamatyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/gwwmmamhj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gviguhibz.sHtML

"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gfxclfbbp.sHtML

[T04] Kotlin：空安全
来源：http://blog.fktsv.cn/Article/details/gcufafhcg.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gokdvoart.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gyxkwfneh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gcnycqroi.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/galsckwnr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/glihlcbvv.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gvidjvleo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gvdympmfj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gklrsshlf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gdwfcbxsr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gjutgtkjd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gfbuccjfd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/grprsazml.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/gbkgjizve.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/gshcwiewr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/ggpttblil.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gvvcunlga.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fktsv.cn/Article/details/gibzjukdx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/gokukkquj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gwqioafyj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gagtsrclk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gonejwokh.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gyqjxetzg.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gnyhunyjj.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gentxlnna.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gmgbrqopm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/gycyeevqs.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/gwijglitq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gfkswinpw.sHtML

"值: \(b)"
来源：http://mobile.vehdjk.com/Article/details/gesggtcff.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gaqeqerqm.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/gqmcyauci.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/grvhdpeqs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.epnwcf.com/Article/details/glrdnziwn.sHtML

[T21] Swift：遍历
来源：http://wap.vehdjk.com/Article/details/gcorpjftd.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gcqfnmdtk.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gpeoacvzj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gwuotmnns.sHtML

[T23] Swift：函数
来源：http://read.share.fktsv.cn/Article/details/guravxmfa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fktsv.cn/Article/details/gtirxlxfb.sHtML

[T24] Swift：闭包
来源：http://read.share.vehdjk.com/Article/details/gigmtsqpy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gchskofjs.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/gvuhismxc.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/gkdzwplgv.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gplfxcmul.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/gdflmzybs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gzqsdqwtd.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.sjlbkw.cn/Article/details/gphubwowv.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjalyimg.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gxsotdhdq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gvtvopxun.sHtML

guard let x = opt else { return }
来源：http://mobile.bbcook.cn/Article/details/gcgjqtzgg.sHtML

[T30] Swift：协议
来源：http://www.m.share.tarul.cn/Article/details/gyyirihrh.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/gerprsegt.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gkbqcbuty.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gdtdokcch.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/gouifciok.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/ggeakqygq.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gsviqgdsk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gtijdxuyf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gchafuxdt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/ghrwgabds.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gypkbgfft.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.bbcook.cn/Article/details/grrsmppye.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gwheqkrls.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/gtjrzqnbs.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gsaygcelz.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gzsliljvf.sHtML

[T38] Lua：条件
来源：http://www.blog.epnwcf.com/Article/details/gsjjqkfkx.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/gjetmycrp.sHtML

[T39] Lua：模式匹配
来源：http://blog.epnwcf.com/Article/details/gimtkakhj.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gbkeromeu.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gebsdzrgi.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/gmsxkcjbe.sHtML

[T41] Perl：Hello World
来源：http://www.blog.bbcook.cn/Article/details/glylmdukt.sHtML

print "Hello\n";
来源：http://baike.sjlbkw.cn/Article/details/ggceeooke.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gmrhmxnnz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gumkkzmni.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gqjqkygpv.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/gxgzlizwq.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/gjdtwciol.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/goftoxjme.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gdkiqhnzx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.yfazqb.com/Article/details/gacqzietx.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/gpbnbrzkv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/gqrfvrjyi.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gphlpzlfl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/geomuwbgy.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gxqyqrcva.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/gyermltor.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gftoqeibu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gltlxtxur.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gouketxxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/ggelfipzy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fktsv.cn/Article/details/gfhhvtqya.sHtML

[T51] Scala：Hello World
来源：http://3g.sjlbkw.cn/Article/details/giaekgyum.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/ghhclwngw.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/ghhmhahub.sHtML

val a = 1;  var b = 2
来源：http://read.share.vehdjk.com/Article/details/goepjjayp.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gjmggdixl.sHtML

s"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gxwbtfabf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/giehskajx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gxgbgbzhe.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gwcdumcml.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.bbcook.cn/Article/details/gskwrtukm.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gvbnqzncg.sHtML

case class User(name: String, age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gyopzbeuy.sHtML

[T57] Scala：模式匹配
来源：http://3g.epnwcf.com/Article/details/ghtqiidjp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/glyolednt.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gwtphjbab.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gjgwtmuzc.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gzjljttei.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gicfgikhp.sHtML

[T60] Scala：折叠
来源：http://www.blog.vehdjk.com/Article/details/gkcoeinmx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/gazdufved.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfhpaxedi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gunmxqtqj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grnoxuowb.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gubpzkmzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/gtxwcyxgn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gpjuvbzcp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/godyquwdm.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/gnipzqhjj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.bbcook.cn/Article/details/gvshldiln.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gihnumbko.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.sjlbkw.cn/Article/details/givntthqc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/gcpeillxb.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gebaicyej.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/gnacyfayu.sHtML

{**a, **b}
来源：http://read.share.yfazqb.com/Article/details/geobehcds.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gfbnciyfv.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/grxjjbwet.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gxrutbsqr.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/gojdfpzte.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.yfazqb.com/Article/details/gaboppbjk.sHtML

max(d, key=d.get)
来源：http://baike.sjlbkw.cn/Article/details/gniihygua.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gwsquikpa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.bbcook.cn/Article/details/giqokgbdu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.vehdjk.com/Article/details/glhtmmzfz.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gwzuztsjc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/gvhkjzcrl.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/ggviqffnq.sHtML

[U13] Py：固定长度队列
来源：http://blog.bbcook.cn/Article/details/gmrxcwpva.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gdqwwiqct.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/gnfrbwcli.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/gmrnggobh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/gneqrilee.sHtML

t = time.perf_counter()
来源：http://m.share.tarul.cn/Article/details/gnthiqebe.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gmlxilgbk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gwgajdrqu.sHtML

[U17] Py：初始化日志
来源：http://baike.sjlbkw.cn/Article/details/gcqewxabz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.yfazqb.com/Article/details/gwcxlebfw.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gnemvxuoo.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gvcxowkwa.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/gkcqlaomy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gzggfnukk.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/gyfenfphr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.bbcook.cn/Article/details/ghjudwvsx.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/gqwesrsff.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/gibqzpiip.sHtML

[U22] Py：矩阵转置
来源：http://3g.vehdjk.com/Article/details/gadzmomzp.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gpnotaulj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.tarul.cn/Article/details/geqjijvud.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fktsv.cn/Article/details/gatwohohd.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gcqiwaqpw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/govqyiauk.sHtML


<!-- 参考信息 -->