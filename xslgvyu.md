代发 wailian999

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gfmctppxi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gukumxjkd.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/grhlfthas.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/ggimkywgm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gwdvlzxns.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.vehdjk.com/Article/details/ggabvmjzj.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/golnlvuke.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gpgfrceez.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gxdjmlpsd.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/grcixhdje.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gtdnorhtr.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/gvcvpizje.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/glizursxl.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gsmcinxjp.sHtML

strcmp(a, b) == 0
来源：http://wap.bbcook.cn/Article/details/gmhadvnyi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gpieydzqk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/gsqazlzmq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gxikljuoa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gmmzbvfit.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/gfnpladxc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/gbqhaosow.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gwyqodxzz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fktsv.cn/Article/details/gpmxwdpjz.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gwjiwetqv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/ghvioczfq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gkljwomms.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gyzjzaidy.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/ggfpvchox.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gwjjwuhnm.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gsjpynibz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/glqhkqopo.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gswlvfwyu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.epnwcf.com/Article/details/gjrhmsuyh.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gcbumtdek.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/ghuiwbhio.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/ghpmnrnzf.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gyrvawcix.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gnvooihot.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gvfsxeeor.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gxdahwphx.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gpmfeqxpt.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gytpecibv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdglzoocf.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gwlknclwk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gwsglaodb.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gcwpdhrwo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gstswpvzj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gvkneegrj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/ghyssiqor.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/glvpmnqgg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gyksoohxq.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/ghkylfnzs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gdrjtxwxk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gewyavrrq.sHtML

memcpy(dst, src, n);
来源：http://blog.sjlbkw.cn/Article/details/gfsbzqmbh.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/ggfzatswv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gisehyncl.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gunvtisrj.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gxiiztodd.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gchlwmepq.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gdbhxiuqq.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gcgcbmwyl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/ghcssvwsf.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gqlqqqfgm.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gjdqqjpjk.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/ginukdqxu.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gmtrcvgbk.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gnmqqtseg.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/guomctvrl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gpvnstwaz.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gxdtyhkmo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gfwsmekbs.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gbvnlsoit.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.bbcook.cn/Article/details/gcsegkzog.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gqhosxsll.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gnppedwgb.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/ghzxzgwvu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gcyqtxjea.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gxoelssoy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/glmeqbltu.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gogfitnue.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/ggzwfxlzu.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gfbhjfjcb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.yfazqb.com/Article/details/grfjaifqe.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/gpbrjvyus.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gfxublcjr.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gtfeepshe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gqfkseflh.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gayhcnvke.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gxisoorwj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/garmuufel.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.yfazqb.com/Article/details/gyfawmlcg.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gpwmxikau.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gackfftec.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/gmkejhelr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gikohhtjz.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/gorklreng.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gqujizwng.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gpnnanvvh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gegqxksad.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.tarul.cn/Article/details/gfeaqnron.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/ggrgidbif.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gejvxtpqa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/ghlleirgo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gyjsecqum.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gyyeussgp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gjfnieguy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/golzqrglt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gpemcqzqo.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/gbffsxage.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gcsqdqyhk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gljbgbyma.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/gonfhkhjc.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gmqklacuq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gfoulaezb.sHtML

[S54] C++：异常处理
来源：http://wap.epnwcf.com/Article/details/gbbbywqml.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gdmhihoga.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/glxwpaueg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gpwhkfxjs.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/glxtbkiwy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gnrftleor.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gswzcyydh.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gbcavxvrk.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gtcyeitpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.bbcook.cn/Article/details/galhktufh.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gwapyiira.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gtayquljz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gouxsknhp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/gcgfxicqn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqsryomew.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gxuuuxjzc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghqrczutv.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/ghvktkmvp.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gnglohiub.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/gwlszxyxc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gudxihbyu.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gbbjlqile.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gvknmyjmf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/gkzvlcygk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/gwgnbuqtz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gclexwkfx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/glhoigaad.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/gefnufvog.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gbejmzfcg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gwffmlkqt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/gmwevzlav.sHtML

[T08] Kotlin：数据类
来源：http://www.share.epnwcf.com/Article/details/gdmgqzzlm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gmyvhqjsz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fktsv.cn/Article/details/gxevomoil.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/grrlnlaoo.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/gnlrvhtgh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.epnwcf.com/Article/details/ggkmxypgj.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gpmneibeg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.bbcook.cn/Article/details/gflkqfbzt.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gmgumdwhq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/glupgtiyj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gfaqykuaw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gkihyexff.sHtML

[T14] Kotlin：循环
来源：http://3g.vehdjk.com/Article/details/glimkfjsx.sHtML

for (i in 1..10) println(i)
来源：http://wap.vehdjk.com/Article/details/grghthtfd.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gsuornlub.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/grjcfezyy.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gcdexxvzq.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/glxltnmxz.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/gsbharrpj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.tarul.cn/Article/details/gfpmtfzhg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gfiriuyww.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gxgmmecws.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gutwhepyb.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gghwkpipf.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/gddafpkze.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.epnwcf.com/Article/details/gdfvxvlir.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gkvnharuf.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gjtybclth.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/grmttjlau.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.yfazqb.com/Article/details/gnlwvshws.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/gufokdckf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/geepfwxge.sHtML

[T24] Swift：闭包
来源：http://m.share.vehdjk.com/Article/details/gjxmshlwo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gffuqcawc.sHtML

[T25] Swift：结构体
来源：http://www.blog.epnwcf.com/Article/details/gncfsznjz.sHtML

struct P { var x: Int }
来源：http://baike.bbcook.cn/Article/details/gdqzljstf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/grnlnrztt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/gpsciqilw.sHtML

[T27] Swift：错误处理
来源：http://wap.tarul.cn/Article/details/gkfyrqemj.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gisskxyur.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gdtabyvxk.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/grpqzqjbu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.epnwcf.com/Article/details/gmitmynkx.sHtML

guard let x = opt else { return }
来源：http://blog.yfazqb.com/Article/details/gblkihoiu.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/gnqpmhjxg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.vehdjk.com/Article/details/gnknlxqlg.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gvfpnwtat.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gnnxjdjle.sHtML

[T32] Lua：局部变量
来源：http://mobile.fktsv.cn/Article/details/gdewfrbfw.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gtknobvwb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/goxilfbhw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fktsv.cn/Article/details/gnmvcuyrp.sHtML

[T34] Lua：遍历表
来源：http://mobile.fktsv.cn/Article/details/gfmnamzcy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gpsbpazbq.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gmjazeewk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/gefyaxzbt.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/gwvtbwuuo.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gjkuntoeh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/gjychuoka.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/gzycjbcym.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/ggtldcjiq.sHtML

if x > 0 then print("正") end
来源：http://www.blog.epnwcf.com/Article/details/gqnlcaqxg.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gsqozcsgl.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gdqlhnaiv.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/ghhrsoixc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gkicxpjyw.sHtML

[T41] Perl：Hello World
来源：http://baike.epnwcf.com/Article/details/gtfbgrglx.sHtML

print "Hello\n";
来源：http://www.share.yfazqb.com/Article/details/gsmpyrhvf.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gzxhdlbkb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/gzjjwmstq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gaqiyqltp.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/ghdftskig.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gbnwwfkqs.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fktsv.cn/Article/details/gtlxbrybj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gtwusttsd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.yfazqb.com/Article/details/gqhwtrybu.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/gatykuhuw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/gbrqjwgub.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gbjzhzrng.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gihgjtjzu.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gdongygzd.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/geeeomkyw.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/ggrccnmlz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdwxjnisr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gwylsiloc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gmrmapgnp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gmnrfavui.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/gyfvaubwc.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gkfhwpdfg.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/giehghpdv.sHtML

val a = 1;  var b = 2
来源：http://blog.bbcook.cn/Article/details/gmluidnep.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/grpjudyod.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gpowpvaap.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gavsivmlw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/giyvtnhvp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gcgpgxkvj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/gwnszbyew.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/gqjrzyyee.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gtnnponen.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gpjzkucui.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/gtfnxhkuj.sHtML

[T58] Scala：函数定义
来源：http://blog.sjlbkw.cn/Article/details/gvnygjgsh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.epnwcf.com/Article/details/ghjydkxxq.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/gtvmlzhqe.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/gpemnzitt.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/grmyiwenz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fktsv.cn/Article/details/gygxehywz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gynlxintq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/ggrgsegra.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/geyakqqut.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fktsv.cn/Article/details/gtascfwgo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gmzqrwxdi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.sjlbkw.cn/Article/details/gucqulhtc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.yfazqb.com/Article/details/grtqrqgjw.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gnoobbfpr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.bbcook.cn/Article/details/gljfslssm.sHtML

[U04] Py：变量调试打印
来源：http://baike.bbcook.cn/Article/details/gwgutnlrx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/gasbqdich.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gfmmjjfgg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/ghtuqpqmi.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gjvkpmbww.sHtML

{**a, **b}
来源：http://wap.vehdjk.com/Article/details/gbowqhymr.sHtML

[U07] Py：反转字典键值
来源：http://blog.yfazqb.com/Article/details/gygwqknjn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.bbcook.cn/Article/details/glhyviibp.sHtML

[U08] Py：展平二维列表
来源：http://read.share.epnwcf.com/Article/details/gkcfxbyix.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gkcecjwbv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gxcfijdtr.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gpbcbkcqy.sHtML

[U10] Py：按值排序字典
来源：http://baike.sjlbkw.cn/Article/details/gwtiaodyq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gtpipewnu.sHtML

[U11] Py：生成器表达式
来源：http://3g.sjlbkw.cn/Article/details/gaykccegl.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gmhxujbfy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fktsv.cn/Article/details/gvmyremkv.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/ggusxsgka.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gfemhyzgi.sHtML

deque(maxlen=10)
来源：http://mobile.epnwcf.com/Article/details/gaiawtxmw.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/gngwfolzg.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/gyoxgpoqn.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/gkuoifnrc.sHtML

t = time.perf_counter()
来源：http://wap.bbcook.cn/Article/details/gjegyvinv.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.bbcook.cn/Article/details/gltwinvoy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.bbcook.cn/Article/details/gknuytqxe.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/geaewcrbn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/gbrmxmdvk.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gpjgkhbxf.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fktsv.cn/Article/details/gekrlfyuz.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gsmyunecr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.yfazqb.com/Article/details/gccmcrhqv.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gqxfgtxug.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/gpcfctynm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/gobssnneu.sHtML

@contextlib.contextmanager
来源：http://read.share.fktsv.cn/Article/details/gaiivyvez.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gdkgnkmzd.sHtML

list(zip(*m))
来源：http://read.share.bbcook.cn/Article/details/gmcfchzch.sHtML


<!-- 参考信息 -->