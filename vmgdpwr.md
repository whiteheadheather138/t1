代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/glkrjfukw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gridbspeu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gblnqtfqy.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gztsvowwa.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gqxamsszg.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gejgznwyb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.tarul.cn/Article/details/gyamyustu.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gpwzxltbq.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/ggpjbscqa.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gjtjfmhuy.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/grhbynola.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gjoospspa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/gvmdzfbed.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/gtbzchlpu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gjxrigmkp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gdltvifoj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gmndtwrmh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.bbcook.cn/Article/details/gkfedmxan.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/gkpmjeyde.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/guwfxwwao.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/gxkhbwmqm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/guzopfxiw.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gnrqmqiru.sHtML

[S12] C：写文件
来源：http://baike.epnwcf.com/Article/details/ghrwjrikf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gftdppnap.sHtML

[S13] C：宏定义
来源：http://wap.fktsv.cn/Article/details/gwanllddt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/grfxxdgat.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gtugyxnue.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gzymiaksh.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/gxbzlpznt.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gwqlyhhbq.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gnpqfteld.sHtML

x |= (1 << 3);
来源：http://wap.sjlbkw.cn/Article/details/gwjyzhnsq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/gevabrgis.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/grkjjrhsa.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gbsbzirij.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gihqhrwpb.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/gehksuhax.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gtyuzxjak.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gerrfoumn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gdekjpylx.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gayddpylt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gzipbuxxe.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/ghrnougfq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/ggtdkagwi.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gawdkqdpy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/ggddemtzx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gewxqveru.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gzkejhmcy.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/grsztvznw.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gzcstisrw.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gzisbkorn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gtbdtzmtk.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gxjdvguvi.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gjoybhtbi.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gwbnntaie.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/gnodhjeko.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gtlapuokf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gdaaubdde.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gppsjkenh.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gudeitoxb.sHtML

#define X_H
来源：http://wap.vehdjk.com/Article/details/gpbxlwrwz.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gsipswlvv.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gopxeonnr.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gzgdvksjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbhbiluwk.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gyzybfusu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gkeseoroe.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gyehzmmrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.bbcook.cn/Article/details/gwbxdhufm.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/ggagudhww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gzsflgjev.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gvktdooif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gouvxiccs.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gjfpqmzol.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gxhmdditl.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/goajmnabb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gyimrzhqb.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gweafidgi.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gokcfbkmf.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gckntorgs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gaxrwwxfp.sHtML

[S40] C++：查找元素
来源：http://m.share.tarul.cn/Article/details/ggorgpeng.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.tarul.cn/Article/details/gxyhxvkmo.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gmxtzymlg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gcgkargig.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gmlloealz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gbnbcfcen.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/gmwhxfekh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gowiujmre.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/gveqscymp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gmxrqonrz.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/gyjnimvxk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gguxhrhiw.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/giivxjcji.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gszqoxduo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaqbasto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/gtujalzea.sHtML

[S48] C++：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gthgmqbhb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gykgcjjrn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/glwcdchyx.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gtbgouarn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gajnjkbsi.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gdxlaswth.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gbuwxonwu.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gchutfqyd.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gctjgmqvc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/goeewgumi.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gehqzrmhe.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gykestrnc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gixjbyepe.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gvylosmqb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gwlebeoow.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/gcrfklqmz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/givepqjpe.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/grtvdteqz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.sjlbkw.cn/Article/details/gnanythhi.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gwfbnszqx.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/gedlyrwov.sHtML

[S58] C++：命名空间
来源：http://baike.yfazqb.com/Article/details/gddcldrjm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gnowgzhwq.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gpivndobf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gxcbuvshf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gqrgnalca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/gseurpmnn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqjhikite.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/ghzhvbfjk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdgsozkwn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gvrsdturx.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gxlzpcuxq.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gonowbflt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/gsbllpnal.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.sjlbkw.cn/Article/details/gaotckiuf.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gudaumwqf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmmxarad.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gylemjjwq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/gkwahsalc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gklfwxkwh.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gagtjtftg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmmrxaum.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gzggmrhpr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/gzxknodpm.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/govnonkwp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gdyqfwhhv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/gsppmoghb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gowjmsjuc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/gcxoowqsa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/glurpxlqb.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/ggqpaurix.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gmqkhthsz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gbdumhkdj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.yfazqb.com/Article/details/ggdwneial.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gqunqxzie.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gthppwkht.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gyexzwcdd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gykwneynb.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gzonknajr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/gntkbqtzc.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/ghfqvobkn.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gsjrpgegh.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/gzlcldjmu.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gxopwaxtq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gbdirceji.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gutkqscrd.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gegpjqvao.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/gvznyntry.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gznahbwie.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gdfhonrdl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.yfazqb.com/Article/details/gjplzamvc.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gnwtesezf.sHtML

[T22] Swift：字典
来源：http://www.blog.vehdjk.com/Article/details/guqccjwwf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/ggmvyouyu.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/gntgjvzmt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gnabmlnhm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/giseipkuu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gthlmsptg.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gdnbxjzox.sHtML

struct P { var x: Int }
来源：http://m.share.bbcook.cn/Article/details/gxgpesadf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gujxcghuq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gefihenfm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gairjwilt.sHtML

do { try f() } catch { print(error) }
来源：http://baike.sjlbkw.cn/Article/details/gcnyyqcuw.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/gnlcfccwb.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/gnlxqaxzx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.sjlbkw.cn/Article/details/ghwknoqxk.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gmrnbfbxr.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/gvgxqdylb.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gxlvdnipu.sHtML

[T31] Lua：Hello World
来源：http://m.share.epnwcf.com/Article/details/gnogltyhc.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/ggfvbghkw.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gwqmwlcrs.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gavykalxv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/gkshzurgr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gweshjuee.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/gdtvaverb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.sjlbkw.cn/Article/details/gqwdesfts.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/gjyowgjku.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/grbzuqsgo.sHtML

[T36] Lua：函数
来源：http://www.share.tarul.cn/Article/details/gmvkvmxng.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/gykfpkwkm.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gszbwrthh.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gzfkacinh.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gqlxcyyje.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gbxiavzeu.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gvafqqoes.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gnuhlqarr.sHtML

[T40] Lua：元表
来源：http://baike.epnwcf.com/Article/details/gdjzhvhhv.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gipxhlwmj.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/gwyaubscy.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/gcvstsses.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gdwwpxbpj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/gpzmmmwfm.sHtML

[T43] Perl：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gzmvaupms.sHtML

"值: $a"
来源：http://baike.yfazqb.com/Article/details/gizdfwflk.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/gcxebtfqb.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/ggnutxpxb.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gmzjjewxz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gjvwvkdkq.sHtML

[T46] Perl：哈希操作
来源：http://wap.vehdjk.com/Article/details/gcnwqvqkz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gcxjirejr.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/giqzctaii.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/guxakmwpl.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gvimtjfon.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gtuhqjbmp.sHtML

[T49] Perl：函数
来源：http://www.blog.vehdjk.com/Article/details/geqaofliw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/glqizwhnx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/ghtuyevea.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gmlwzvmbc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.epnwcf.com/Article/details/grcebubmg.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gcqmavfrb.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gzbwrdstm.sHtML

[T52] Scala：变量
来源：http://mobile.sjlbkw.cn/Article/details/grxomtqvo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gcomiijpo.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/ggoblimfk.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/gruwtrqyq.sHtML

[T54] Scala：集合映射
来源：http://3g.yfazqb.com/Article/details/guzxyrfpn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.bbcook.cn/Article/details/garuvhkoy.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/grzdmwhsm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.sjlbkw.cn/Article/details/gsgrkccnr.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gvglcogpa.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gpnqpgksj.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gfqdvgztu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/gpppjcbyq.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/grwntnilw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/gwkcvdtbr.sHtML

[T59] Scala：循环
来源：http://wap.bbcook.cn/Article/details/gwrkptqzo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/goxtvezhf.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gdccqwkqx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.yfazqb.com/Article/details/ghdpaotog.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpejpslhh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/ghfuugfkq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsslrxccn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.yfazqb.com/Article/details/gnjwpscaa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.yfazqb.com/Article/details/gzuindqdg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/gcprjekeu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.vehdjk.com/Article/details/gslvmbcbq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fktsv.cn/Article/details/gjwgpomrt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fktsv.cn/Article/details/gvlqphwii.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gazwvhmok.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.yfazqb.com/Article/details/ggmbnslrz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/guqdcckyj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gnyawhetk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/gfaoowmnn.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/glekdotcj.sHtML

[U07] Py：反转字典键值
来源：http://3g.fktsv.cn/Article/details/gcsxommgi.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gycsmswaq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.vehdjk.com/Article/details/gjbqsclns.sHtML

[y for x in nested for y in x]
来源：http://mobile.epnwcf.com/Article/details/gpjkfeeny.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gritpqsgq.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/ggwrnnest.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqjcttco.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.yfazqb.com/Article/details/glshniyhp.sHtML

[U11] Py：生成器表达式
来源：http://read.share.yfazqb.com/Article/details/glgpsasau.sHtML

(x * 2 for x in arr)
来源：http://mobile.yfazqb.com/Article/details/gutmulwny.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.sjlbkw.cn/Article/details/gxlycgkgl.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gsfyfqntt.sHtML

[U13] Py：固定长度队列
来源：http://baike.epnwcf.com/Article/details/grnplayri.sHtML

deque(maxlen=10)
来源：http://www.share.epnwcf.com/Article/details/ggbcotzwn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.bbcook.cn/Article/details/gkqiyreez.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gdfsosewx.sHtML

[U15] Py：高精度计时
来源：http://baike.sjlbkw.cn/Article/details/golcjqmnr.sHtML

t = time.perf_counter()
来源：http://read.share.yfazqb.com/Article/details/ggevmsxnj.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gfautvtnj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gyrbwjgxa.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gtpyzomwx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.sjlbkw.cn/Article/details/gsfafstbx.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gexvmgyit.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/ggitjsxrx.sHtML

[U19] Py：正则替换带回调
来源：http://3g.vehdjk.com/Article/details/gknogndql.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/ghjrlsykn.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/gvkqhcdtq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.sjlbkw.cn/Article/details/gictfsoln.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gmaulsukz.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/gncnqycnm.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/gtoudgtgs.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/gslqqbbtg.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/gmamspdzb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gwxckzrvz.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gjfuhquyv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/giguoloka.sHtML


<!-- 参考信息 -->