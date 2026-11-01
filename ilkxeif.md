代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/glvflzjwd.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/gnzxenpaq.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/gwabrevuy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpavfnkaf.sHtML

S. C / C++ 专题
来源：http://3g.vehdjk.com/Article/details/gcrvoaemm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjbnaemkl.sHtML

[S01] C：Hello World
来源：http://www.m.share.tarul.cn/Article/details/giuxzozpu.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gjmmnnxpe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/glnsplpzj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gzmeziace.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gzvktlgaq.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gmqxnqfod.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gikngxfnn.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/grsfbzykl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gwseoyszi.sHtML

[S05] C：字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gjaqvtypx.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/gacjfjput.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/gvnyicxie.sHtML

strcmp(a, b) == 0
来源：http://mobile.tarul.cn/Article/details/glghhdmke.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/gzzxthgfe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/glkciszwo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/giovhflui.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/gpebpzbog.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gevpfogfy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.tarul.cn/Article/details/govphlovq.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/gqchbxgls.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gukjtwicn.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gsakuolwa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gmwhaszrh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gplbutytz.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gwbzoaxjs.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gvklrkwhs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gjigsscex.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gxjmaymnw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gwqbhxcep.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gzdbiwpme.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gxzglyehi.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gvgluxnst.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/glvxmmefw.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/grckognvf.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/glbcaytlu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gybgonrvy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/grtcfjfly.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/ggebsfffe.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gtdiostvh.sHtML

[S19] C：快速排序
来源：http://www.blog.tarul.cn/Article/details/givpfsmrq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gfntiemjn.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gjfksbsgp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/ghzyzspwy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gsnmzzxlj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gqdoeydst.sHtML

[S22] C：字符串转数字
来源：http://blog.epnwcf.com/Article/details/gwuriweiv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gzenxshwc.sHtML

[S23] C：随机数
来源：http://www.blog.vehdjk.com/Article/details/gjlmxeeoo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/getqigewe.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gpxoyozki.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gxodvrheo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gfgoaaodk.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gefymykrz.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gjrdbjjqo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gnwprsoba.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gndmrxdrx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/ghenfuunf.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gjgqegpew.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/gayirowmi.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gyybpwbgr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gocrdkmzy.sHtML

[S30] C：头文件保护
来源：http://mobile.yfazqb.com/Article/details/gzcgvofae.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/ghrdeahjc.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/glkkoyonw.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gzxsrqsyo.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/grmiafshh.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gwiwggtre.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gybakvsna.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/gaituoowe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/goxcizaja.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/grmluijzr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/gzfhxexcl.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/giztzlqth.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gjfagtakb.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/gbhhldygz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gonrgnfzd.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gjrymogza.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gqvhxioup.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gsigpmlry.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/ghubtdfln.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/gfsotcays.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/getziquda.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gasvotmjm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/giicwtvcu.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/gsggqrimc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gaffypvqf.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gdusvmnnz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gdmafqkjb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/gyaafnqah.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/gpupwhaea.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/gwxiiiyqc.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.sjlbkw.cn/Article/details/gwmmyzkpq.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gvylcehdn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/gqpdeqvsu.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gxbojyyus.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/ggierhhjp.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gyzdugpjj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gfmwwgpff.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gzqwfumst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/gpuweyjsn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gmusxlbkd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gzshoponu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/gbpezkeed.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gyynnhucz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gcytkfofc.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/goopgmyro.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gqhdbpanb.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gsogkbyae.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/ginywermg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gqpiixgnc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/glngqmzcx.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gfeyiymjd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gfywmxacp.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gsralojml.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gclkgeici.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/grvfgyeqt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gbzjdkkgs.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gwlzwtexi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gpjacsakz.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gwkytuzle.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gptxjoqfo.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/galwfxgty.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gfjkqgmnn.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gspknazdi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/gaedjxfgj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gndcchsut.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.yfazqb.com/Article/details/gmctoccjk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqvdzwpyc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gydttszjq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwbhmxghf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gaaeuagrm.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/grvjbwnsa.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/glkrcxhbv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/gmcjdwpsd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/gjdnrboug.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gsiyfgtpo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gfzvejpyh.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/grqffqyig.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gsktrfnip.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gctegmvuv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gftylrfuo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/goxrddezg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/grqmhluql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/gvltfbhum.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gfjiiolzi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/ghupitcpi.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/gprdltopg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/gvruvnjjs.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gwluahvvx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gbvuumtrf.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gavymfdyg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/grvrqfzpu.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/ghxngqgni.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gzwzmtglb.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gvaiirnll.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/grorpunns.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gyfggmaog.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gwhzdyprn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gfqeeptoa.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gjeqjqdvg.sHtML

[T16] Swift：Hello World
来源：http://3g.vehdjk.com/Article/details/gotsytxss.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gujxehhmo.sHtML

[T17] Swift：变量与常量
来源：http://m.share.sjlbkw.cn/Article/details/gghhtxbin.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gezijowwu.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gwgndfqzm.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gvheuxmrh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/ghihdnige.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gvlkdspey.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/gjdbusteh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/gpvyngzib.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/ggtsshyha.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/ghyjtaftm.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gzjtryqfg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gjpbswlui.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/giaynmsdp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gdvxqsytp.sHtML

[T24] Swift：闭包
来源：http://www.share.vehdjk.com/Article/details/gazhqppyi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gbbraoute.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/goygrnmwv.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gyrvvbyxp.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gpxgqvcnv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/gqayvwxpb.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gxanfkfmj.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gmkloihgh.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/gvsnheayp.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/gnzxfgfnv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gslpkzhus.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/gmnhjgidi.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/guvnieuqq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gbbrkupkq.sHtML

[T31] Lua：Hello World
来源：http://3g.yfazqb.com/Article/details/gvacweszf.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gskifmojy.sHtML

[T32] Lua：局部变量
来源：http://blog.vehdjk.com/Article/details/gtyuwdqiw.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gawnltngn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fktsv.cn/Article/details/govaowdmn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gohbdebhh.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/ggsbtcbnd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gccbbeuls.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/ggbmhxdid.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gajawegxg.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gmhflydha.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gqijsdxyl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/ghkwqtddw.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gcllszols.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gaufxgtvl.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gnppctpdn.sHtML

[T39] Lua：模式匹配
来源：http://3g.bbcook.cn/Article/details/giqvwrqcu.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/ghtkobtdd.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/gyuxiecpl.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.sjlbkw.cn/Article/details/goirqpxfg.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/ghcwphckp.sHtML

print "Hello\n";
来源：http://blog.bbcook.cn/Article/details/grwapemcj.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gpbxpifeq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/givaeiuoz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gklmmwpkw.sHtML

"值: $a"
来源：http://blog.sjlbkw.cn/Article/details/gctoacdyr.sHtML

[T44] Perl：条件
来源：http://blog.epnwcf.com/Article/details/glayvnakf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gosioasre.sHtML

[T45] Perl：数组遍历
来源：http://baike.sjlbkw.cn/Article/details/glzamrdej.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fktsv.cn/Article/details/gojcvkeyl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/gcandgngv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.bbcook.cn/Article/details/gjbiatpbb.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/gojbcgyzo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.bbcook.cn/Article/details/gugqerdry.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/gwlljvnqw.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fktsv.cn/Article/details/gzyqeplsa.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gkkhhrbak.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/giucblmrf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gxeqqefro.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gvyweudve.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.epnwcf.com/Article/details/glkvgbclh.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gfxsnpyva.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gbttirqvm.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/gpxrrgfpb.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gxatbyzlo.sHtML

[T53] Scala：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gprpolzjj.sHtML

s"值: $b"
来源：http://blog.vehdjk.com/Article/details/gbfznlbjn.sHtML

[T54] Scala：集合映射
来源：http://blog.yfazqb.com/Article/details/gdupurtol.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/givfxfhmf.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gfibmvggf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/gluyyjiuj.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gjwapjfzc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/ghmvuoeif.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/goptvxdvd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gieqfrszz.sHtML

[T58] Scala：函数定义
来源：http://mobile.tarul.cn/Article/details/gksxchoks.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gcfqsnqmn.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gzrpmjqjw.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fktsv.cn/Article/details/gaawkenep.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gpeppenti.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/grslwicsi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdweejfcw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.yfazqb.com/Article/details/glzxotxer.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkqyygtxi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.sjlbkw.cn/Article/details/gvtltelsp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.yfazqb.com/Article/details/gtzudjyhh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.bbcook.cn/Article/details/ggcdayvxs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gonapxrgf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gqfvourej.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.yfazqb.com/Article/details/gatjecpai.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/gwkubnsbt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gkzuwsqcl.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.epnwcf.com/Article/details/gsgccemno.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gtgkfqhdu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gasxcciuo.sHtML

{**a, **b}
来源：http://read.share.epnwcf.com/Article/details/gpvuurjjz.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/giqzpzbqx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gdazbuqgz.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gtltylras.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/gtebdbtxi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/gjjtofnfg.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/gbkyyhiwy.sHtML

[U10] Py：按值排序字典
来源：http://wap.tarul.cn/Article/details/gbbvvktjv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.epnwcf.com/Article/details/geinsusyo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gpkuwkwof.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gcikgzyak.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/gnerzbyov.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/gzdtfbbfq.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/ghuqiaejt.sHtML

deque(maxlen=10)
来源：http://blog.bbcook.cn/Article/details/gknvrzhto.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.vehdjk.com/Article/details/gpvucorvz.sHtML

defaultdict(list)
来源：http://wap.fktsv.cn/Article/details/gtatavkho.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/gygvcrsnx.sHtML

t = time.perf_counter()
来源：http://mobile.fktsv.cn/Article/details/gnjrvfowm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/gmupnkkxg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.tarul.cn/Article/details/gumqziizj.sHtML

[U17] Py：初始化日志
来源：http://3g.sjlbkw.cn/Article/details/gqbbehovb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwkvfygx.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gppmzuezq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/goadstlzd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gmbtfqdxw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.epnwcf.com/Article/details/grakbsutp.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/ggswxjxni.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.epnwcf.com/Article/details/gyeylflwf.sHtML


<!-- 参考信息 -->