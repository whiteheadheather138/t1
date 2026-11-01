代发 wailian999

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/gccczgpgz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpnmagjbe.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gdlvchhqa.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gjtwgozfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/ghvmybwyq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gsneunykm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fktsv.cn/Article/details/gipngjywv.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/ghjgzbkcw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/grubnikbc.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/gzedigwyz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/ghdeztuwi.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/goqfqwpbk.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gxamwvmka.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/ghsjxrgrw.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gwfdpkipd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gbmgzrllk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/gdhqclfem.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gxksdxtyj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gnzerdrsl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gxuemgztb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gfupjibwr.sHtML

[S10] C：指针与解引用
来源：http://mobile.yfazqb.com/Article/details/gronqnimz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gvrpobyuf.sHtML

[S11] C：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gyprdmcwb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/giihqbrug.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gkgqwfjeu.sHtML

fclose(f);
来源：http://baike.tarul.cn/Article/details/gqpzwxtkz.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/gvonkccbx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gedypfvzl.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gfnwchnyr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gtxydwzof.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/ggltpqtqt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gllhdrrry.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gphyzprey.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gflybmyka.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gladieqnk.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gbgvsximq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/guuuujobs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/ghlqsdnwk.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gkxfsylew.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gtwfguqna.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/guhtbcjzr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/ggeybipct.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/gzclmyglr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/guhvscoos.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gdvjkdiew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/grjbpfvxy.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gmuhvagnb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/gwlyeoypn.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gdlmhphzf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gotnqfhep.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/godwdznng.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gdmrzrxct.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gqvkejtdq.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gxkqsxaqj.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gdcwksvwz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gouucafwl.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gdsrkjnrg.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/glelosfhm.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gqcbbskjq.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gbebasowh.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/gymeuujlz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gxptbdluj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gtnkzecvk.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/ggrpkbuvu.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gnzlgpqmz.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gdqbkdstb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ghychqrds.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/gxbhoxedn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/gyhhgmueb.sHtML

[S32] C++：字符串
来源：http://3g.epnwcf.com/Article/details/gvvtxxmnz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gfepczqww.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gqfmtcrbn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gclonrlrq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gbikznixy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gnllmpgmq.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gksazzgcm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gqdwqtzxy.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gqwxjmule.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gojdlrpir.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/gechgvomb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gbaziexpj.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gqakeeolr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gpdldpqrl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/ghsuxqfxm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gxjovcqsi.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/goqhtjorf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/gwaithkjp.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gabozmklo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gepnvcorr.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gvvczlgjg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gfvlepanx.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gdveauffg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gykubbczn.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/ggvmswrvo.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/godapkhvx.sHtML

[S45] C++：lambda
来源：http://www.blog.fktsv.cn/Article/details/gzothprpy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gnslepqyb.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gcqfngjfj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gvwqxheuw.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/gvfznerxe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/givxhixut.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gmareflcp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.vehdjk.com/Article/details/gywocsqus.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/glgbyltfo.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/ggmrfpnff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gdisbgveu.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/gshfgpzum.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gvjamffzc.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/gxdbzrtjw.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gssswxekm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gmfhrbwxt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gbzxhqnhy.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gwyahwjvu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gtzwmhmdi.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gjcmigppm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gqdeacnkc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fktsv.cn/Article/details/gaczubcnm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.epnwcf.com/Article/details/gwlvftrtf.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gqckopjae.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gzhjtmlky.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gnzemjypx.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gdjwlogwt.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gnhxwvmyq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.epnwcf.com/Article/details/gjkaqjkjh.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gjxcckddw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.vehdjk.com/Article/details/gyuphqrgr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gxweflgfy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gmrlpqwqb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvqbsyvnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gixqpvkcl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdugxvcxk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/gjrzlaele.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/glfcuhfix.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gzlvzelee.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/grslfrsxb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/gjxgtotez.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gxtgiazli.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gdgfhlxws.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gilpbogmk.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.epnwcf.com/Article/details/gzgpwuqyp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gfpgcrneb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gvqhassgf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/ghdsaawjm.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/gdsfredlv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/ggrtaccmk.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/grpuvjuaf.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/godefqhig.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gfwfhsubc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fktsv.cn/Article/details/gmeevvdql.sHtML

[T10] Kotlin：默认参数
来源：http://3g.yfazqb.com/Article/details/gyzctucqb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.bbcook.cn/Article/details/gxtykdyvd.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/gwqdnixgn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gkbchnuxb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/ghqtzprwe.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/gvuwylciq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gqjerjpmc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gtvxrlhex.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/guvxqguav.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gmfpptiqy.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gzsdkwqtn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.bbcook.cn/Article/details/gwojadzxf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gofdmapdz.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/glfewclis.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/gdwasoxtf.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/gumckdtbo.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gudbaakrm.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gujuzrtkt.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gxpbqyrdw.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/gaceqmanv.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gydqsiwyl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gucloxcpz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.epnwcf.com/Article/details/ggqqxxbwt.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gsylfwxoq.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gzrnlpnuh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/grghfpcnm.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/gvfobkjiy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gnqsntwsq.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gutkkpdml.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.epnwcf.com/Article/details/giuqutmhs.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gvxzqmexh.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gtviijaog.sHtML

[T26] Swift：类与重写
来源：http://baike.tarul.cn/Article/details/gmqkurozp.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/gasmtocln.sHtML

[T27] Swift：错误处理
来源：http://www.blog.bbcook.cn/Article/details/gkwakgcyd.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/gqctgtgqc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gihlkjrmg.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gkbfdcrlb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/grirsekbt.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/gmltgmcli.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gpemgszym.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/gmqlbwuxm.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gjsdziiex.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/govxopboj.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gujqpfzsq.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gpesrdslg.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gkkxjhekj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gilmptstm.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/gmlyqpzms.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.bbcook.cn/Article/details/gnhwnuplc.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gnodheuuu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.bbcook.cn/Article/details/gilhhvjlq.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/ghrlvfxlr.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxflofyf.sHtML

[T37] Lua：字符串拼接
来源：http://blog.yfazqb.com/Article/details/gevjyusee.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/gyubtvrxe.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/ggygxnwib.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gannokipe.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/grnbjqpjp.sHtML

string.find(s, "%d+")
来源：http://blog.sjlbkw.cn/Article/details/gfdycxgof.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gzlrhhfmy.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fktsv.cn/Article/details/gqrzcnswr.sHtML

[T41] Perl：Hello World
来源：http://blog.epnwcf.com/Article/details/gyoxlejrd.sHtML

print "Hello\n";
来源：http://3g.epnwcf.com/Article/details/gfbguscau.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gutyzplqp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gktkaoiex.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gucydixhx.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/gblkgmfoq.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gjjmsjfgi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gmukoyqzs.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gjciaibnw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/glqwdvokm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.tarul.cn/Article/details/gwjbewdbj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/glabyicuk.sHtML

[T47] Perl：正则捕获
来源：http://wap.vehdjk.com/Article/details/giwjkmxsw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/gbhqosymd.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gyxrlzfko.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gmwjsawsv.sHtML

[T49] Perl：函数
来源：http://m.share.epnwcf.com/Article/details/gtuchbagz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gdkytsluw.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gjfvvhnvf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gqzlrcace.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/ggsqgrgpp.sHtML

[T51] Scala：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gejisngxx.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/ggvhgchsf.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/glzhrihtl.sHtML

val a = 1;  var b = 2
来源：http://www.share.vehdjk.com/Article/details/glecheqwe.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gmrclrzwx.sHtML

s"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gtjqinwbz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gltoogqsb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/ghuhgxikx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/gjktciwpb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gllrzzhvu.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/gozcmtuwx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gyzlonhkr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gmcnojqhd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gawziachf.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/giwhcqegq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.bbcook.cn/Article/details/ggisjggjv.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/ghxiyzdfw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/glvmidnmw.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/gprqyqfvo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/gokuavdnu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkypsanmw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gyknairlj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsqecbojh.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gbvbzouid.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.epnwcf.com/Article/details/gnslpthke.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.bbcook.cn/Article/details/gfleuzsei.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gftycywvk.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fktsv.cn/Article/details/gxqqinnpr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/gxzixcvqd.sHtML

[U04] Py：变量调试打印
来源：http://wap.fktsv.cn/Article/details/gqhtvyepq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/gazkhrxzk.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gcixjouaf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gbdsbpnxk.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gaemcfuds.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gyxjiygzd.sHtML

[U07] Py：反转字典键值
来源：http://www.share.bbcook.cn/Article/details/gpabalrpc.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gdtgaiifq.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/gwgeczlln.sHtML

[y for x in nested for y in x]
来源：http://baike.yfazqb.com/Article/details/gzjbfzsqk.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.tarul.cn/Article/details/gueslhkok.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gqkadcviw.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.vehdjk.com/Article/details/gjszjqkog.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/ghhurfmct.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/goahakstz.sHtML

(x * 2 for x in arr)
来源：http://wap.epnwcf.com/Article/details/gymmnpkar.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.tarul.cn/Article/details/gpsnpsend.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gcikqqzxx.sHtML

[U13] Py：固定长度队列
来源：http://m.share.epnwcf.com/Article/details/gvklgqedo.sHtML

deque(maxlen=10)
来源：http://baike.vehdjk.com/Article/details/grbqpifxb.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.sjlbkw.cn/Article/details/ghnaowgca.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gojcwjddo.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/gyqieneuc.sHtML

t = time.perf_counter()
来源：http://www.blog.fktsv.cn/Article/details/gwondnosd.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/goafmaedt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.tarul.cn/Article/details/gcofhpals.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/guuiodeqa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.bbcook.cn/Article/details/gynqvrsbu.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gdshiywtv.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gxaguoutz.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/giclfnnpo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.tarul.cn/Article/details/gomazvcoo.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gnqpyzpei.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/goyabmhtk.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.vehdjk.com/Article/details/gammgnkwn.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/ggvbsailg.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gjvyxoywr.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/ggnycdonv.sHtML


<!-- 参考信息 -->