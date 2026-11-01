代发 wailian999

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/gazxxoipl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gevahzgxi.sHtML

[S01] C：Hello World
来源：http://read.share.yfazqb.com/Article/details/gscyufxwb.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/grscifgfa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gjgtqddyq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjontoxy.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gbawdjyou.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gbnqxwjjh.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gsuwauheq.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/ggfoqjkih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/geqqwgigs.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gslbqeecq.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gsvtbjzdj.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gewletpsq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/ggffyqjqr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.bbcook.cn/Article/details/gjctyproo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gjqjszdtn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gvmpkjcmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/gxlsspddu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/gulpfwace.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gvfszlqok.sHtML

[S10] C：指针与解引用
来源：http://blog.epnwcf.com/Article/details/guovdlism.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gnerxgxiq.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gfkrypvju.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gvbrictqq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gkzjuhhct.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gedfeuidj.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/geirvyjvk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gmdidacsi.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gdlgjqcso.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gseqqeehc.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gbkoekdhv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.epnwcf.com/Article/details/gaftogcyu.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/ghizbanah.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/gicxjutjs.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/ggpfopssl.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/ggiftssnk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/grltsoqmk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/genztftak.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gwgdrahwf.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gzemqkdgr.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/gjpfrapof.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gxjfzpifm.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gwzroryzn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gmfdspgrk.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gmihuhtvv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/gwyhhjomx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gyiwgmrbg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/gdhxmsapg.sHtML

[S23] C：随机数
来源：http://mobile.bbcook.cn/Article/details/gnadavorz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gufsfcbyb.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/gddskxwjg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/glbrrilxo.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gxrwhuxuc.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gomlcizzx.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gcqlriuyk.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/ghmzagdfs.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gvtunlecn.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gpyhfnknt.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gjruitrby.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/gguynenkc.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gntbhcirx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/gmnetbwov.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gyfiexqms.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/gonzpplsv.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/ghbpinzvf.sHtML

#endif
来源：http://read.share.epnwcf.com/Article/details/grcakktas.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gvuxjuyyg.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gondhnsmb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gmhxnyxhf.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gkkakgbiu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjoecvgu.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/giangzmyw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.tarul.cn/Article/details/gachbtvdx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gkpyftzyz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gabbbpmqi.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gfxecwfgh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gxipqujnq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gylkfuwco.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gzqojwkhg.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/gcfnuiigd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/grasepolp.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/gxghexgvd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gxyaaullj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gnyvqltbg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gcndvdwzw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/gsfdvrndt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/guldfzkdm.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gskummuff.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/geomkmgms.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gptazglxl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gqosczwxk.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gastadiof.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gtkxofupl.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gromuwukq.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gltfhospm.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gfbboiksd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gjnssflru.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gzabeuvgy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gtrelpoeb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/ggkojudjr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gcxnqlmlr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gitpzqfbt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gpifekakp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gbjtinhiu.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gxkgkgjpq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gwihumdtz.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/ghxtvenqm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gzdjkqqti.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gbzsshyiq.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gqrsxirce.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gfgaoncyi.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/grfqyvdns.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gbmekcvpw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.yfazqb.com/Article/details/gtrzkigll.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/ghztwzksf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gzxhcccmn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gpqqcfbwq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gifgsufrp.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gklcpljcr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gbgftbgua.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbmyarjt.sHtML

constexpr int N = 10;
来源：http://mobile.yfazqb.com/Article/details/gwuplbqne.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gzjwbpnum.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/ghncbgwee.sHtML

[S59] C++：静态断言
来源：http://wap.yfazqb.com/Article/details/gypmxexvj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.epnwcf.com/Article/details/gckdtibzd.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/gqwcbqflg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gkdtggecy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpfqxfxlg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gwcbfucib.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdkljtert.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gkwwsdxyt.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gpcfenubw.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gujwwqclx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gtpeevdxu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gdtxvccwb.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gayweabnt.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gyimmcesl.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gdrgyrjuz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/ghdymkndw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gyltjxoti.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gadldivhu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gmodjunyv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gtihxnwez.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.vehdjk.com/Article/details/gbungiitu.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gwxxxwgqa.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gqohbewpz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gftoqmevg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gjmejvbwr.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gujexnfyj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gwuqjsisu.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gdlqmqkjs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gibcxohnq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/gcgrfqwry.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gxlxcpccv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gpcfvmbcm.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/gaxbtaxzo.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/gpvnlznky.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gslryhafc.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gddgnwfyt.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/goxizoxzw.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gqmumhkgc.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gjcdflhvl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.vehdjk.com/Article/details/ghvynrbwo.sHtML

var a = 1;  let b = 2
来源：http://wap.yfazqb.com/Article/details/guvdxqyqk.sHtML

[T18] Swift：字符串插值
来源：http://blog.vehdjk.com/Article/details/glwvlzsfr.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gluyvfoyq.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/gwsmtdbqz.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gyqjotkep.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gnektuali.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gbegawfjb.sHtML

[T21] Swift：遍历
来源：http://3g.epnwcf.com/Article/details/gqfckmuhh.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/ggwarltuw.sHtML

[T22] Swift：字典
来源：http://blog.bbcook.cn/Article/details/gybajkieb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gwmrailgt.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gndrybguf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gquxwxjgv.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gjxtyvmmd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gdrgvlgqd.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gqklyfrha.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gwnjfonns.sHtML

[T26] Swift：类与重写
来源：http://m.share.vehdjk.com/Article/details/gzpceiqhl.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gkjlmizzx.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gkkjgbwwm.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/glnwpszui.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/ghvxofrpn.sHtML

enum Color { case red, green }
来源：http://mobile.sjlbkw.cn/Article/details/gvsepaeym.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.yfazqb.com/Article/details/glumfckik.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/gugutphqm.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gxeihvzom.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjwoyfak.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gkwnirzdt.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gnkleqojt.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gxrrixoaw.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gnlndqhky.sHtML

[T33] Lua：表（数组）
来源：http://wap.fktsv.cn/Article/details/goqzqygod.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fktsv.cn/Article/details/geeefmsed.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/galqacgiw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.tarul.cn/Article/details/gpudmgyte.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/grqedvipm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gedbyhxxb.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/gomoqqidt.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gvilpwkrp.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gvpbdlrwz.sHtML

"a" .. "b"
来源：http://www.blog.bbcook.cn/Article/details/glumlqtgu.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/ginrqcxoa.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gmrntjatu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gnajqyrzm.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/ghakbomoh.sHtML

[T40] Lua：元表
来源：http://mobile.sjlbkw.cn/Article/details/gxyellsyz.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/gywgrilqk.sHtML

[T41] Perl：Hello World
来源：http://www.share.tarul.cn/Article/details/gcwpihirx.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gksolfzwe.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gpaovmqva.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.epnwcf.com/Article/details/girmspqiq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gqspwvebn.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/guyydwies.sHtML

[T44] Perl：条件
来源：http://www.share.epnwcf.com/Article/details/gyhcftpkg.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.epnwcf.com/Article/details/gznxtvini.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/gyenytbpx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/gyxkcvhym.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gghbhtasi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/gntjmesep.sHtML

[T47] Perl：正则捕获
来源：http://mobile.sjlbkw.cn/Article/details/gdtxvbgqy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.vehdjk.com/Article/details/ghcethznb.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/gcoawvwgf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.sjlbkw.cn/Article/details/gnrygnlsp.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gxnvisosu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gaupiaarh.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbixauvs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/gwwkwzohc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gxvczmopp.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/guycgmqtf.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gdjqarkeh.sHtML

[T52] Scala：变量
来源：http://3g.vehdjk.com/Article/details/gwcbxwyyg.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gevgecdmx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gajwvvtvd.sHtML

s"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gesgvamlh.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gngkpxjsf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.sjlbkw.cn/Article/details/gjyigeejt.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/gyqurlzjy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/gfsncziva.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gjwqzkwqd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/ggafhyobi.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gkywcgeje.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/ggpbdmlvv.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gzrnnbdls.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.bbcook.cn/Article/details/gwzfquxhm.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gabqqdqew.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gdhysxgli.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gjtkptxeu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/grtzifjof.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/giotrsmig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/gmggnpqrk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghrobowsj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.sjlbkw.cn/Article/details/ggvanbjme.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gorpfgyfl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/grlysxuet.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gewhfbcul.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gujcjzfgv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.sjlbkw.cn/Article/details/ghdcuiidf.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gtukxawgz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gmxkioqpx.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gogloomgt.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gqunsutmu.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/ghybqxhjd.sHtML

{**a, **b}
来源：http://blog.sjlbkw.cn/Article/details/geomknjcl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.yfazqb.com/Article/details/gxvkrfwlb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gpickquan.sHtML

[U08] Py：展平二维列表
来源：http://m.share.vehdjk.com/Article/details/giyvbqhkv.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/grjmtaerr.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/gcfsgexyk.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/gtpvucmiq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gbfqyroei.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/gcrhcfiwn.sHtML

[U11] Py：生成器表达式
来源：http://mobile.yfazqb.com/Article/details/gecsbisjw.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gqyzrwgwr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/gcqwtpiib.sHtML

Counter(arr).most_common(3)
来源：http://www.share.tarul.cn/Article/details/gvqrgkkix.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/gwajyknrf.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/gpmflpmoo.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/giafdleqq.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gaulqficg.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gwjujpnzk.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/ggjsbmyiy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.vehdjk.com/Article/details/gljuafcvt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.yfazqb.com/Article/details/gxrqyazud.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/ggccaoiaa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/gsfvhoppr.sHtML

[U18] Py：预编译正则
来源：http://mobile.bbcook.cn/Article/details/gapvixxvx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/gyxeqfesu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gszrpffvd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.tarul.cn/Article/details/gpagrznqx.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.tarul.cn/Article/details/gsmlrioxk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.yfazqb.com/Article/details/gulwlxkde.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.bbcook.cn/Article/details/glqavxugu.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/guldbvbwm.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gtvqpephd.sHtML

list(zip(*m))
来源：http://m.share.bbcook.cn/Article/details/gozwrsqqy.sHtML


<!-- 参考信息 -->