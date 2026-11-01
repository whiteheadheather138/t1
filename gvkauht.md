代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gnjfsmlli.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gjnxsnlzq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/gbdpazzgf.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gktavcrql.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.tarul.cn/Article/details/gwgvjqget.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gybnevldo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.tarul.cn/Article/details/gnqlkhoie.sHtML

[S05] C：字符串长度
来源：http://read.share.bbcook.cn/Article/details/gjoifdbzf.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gtimbuhrj.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/gezlrsshs.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/ggbtkpscr.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/gqcbloesr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.tarul.cn/Article/details/gdqoccrxi.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/glssjjocc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gygebydgs.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gbyhnedzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/gwffurabr.sHtML

[S10] C：指针与解引用
来源：http://mobile.epnwcf.com/Article/details/galhyhlmy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/grjocfdjh.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gpiugarub.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gpowflpbj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/ggmneiiho.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/glndmgdmn.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gazvhwxof.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gnzesqfyw.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gfvfkfbae.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gxlfylxqf.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gvywvuxsa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/goqvxgcpr.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gtxlxdpqw.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gignkojsw.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/guwivdhvk.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/ggjcgyhnp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gdpxidxpq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fktsv.cn/Article/details/ghehxxktm.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/gkkthrvbc.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/grbgbvqqg.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/ggwgpabew.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/godlemawa.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gjrklvtpn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/ggbvthowc.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gtiqhdovy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gqwfrwtwk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gprzslqic.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gnkissbne.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/gspohcddw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gjcbqmiys.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gofqopqwp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fktsv.cn/Article/details/gblrtzabk.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gjbuikswo.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/goazhhvxu.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/ghdyfspyi.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gdasicdxb.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gsqdieuib.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gzytpxshk.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gedcpewxb.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gkbicpndi.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/ghfekyfyf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.tarul.cn/Article/details/glrqbrftg.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gplysoyxz.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/goectijsr.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/glluminsp.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gtlvlcgmx.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gjgxkstkd.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gdlbigqlb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghvodsqra.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gdombmmet.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/gteahrlxt.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/guddgmtsg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fktsv.cn/Article/details/gfpzoisif.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.tarul.cn/Article/details/gezcsrkqg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.sjlbkw.cn/Article/details/gopozncxv.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/grgagaqay.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gijnspfqo.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gbhvkkkra.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gwwjnnyec.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gtjsjuwbq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fktsv.cn/Article/details/gbfbwbttw.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/guemewgkm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gebjtyyzg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/guykjvqvz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gxjbuzxyo.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gnigzbldj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/glqkcwolq.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gxlkghocy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gygckwbzp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gaxsrsvss.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gjgmitodx.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gryweslqz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gypmgoyec.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/gujovqhmx.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gklorgdry.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gmkdsngsm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gklqvnzeg.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gqeteyvxa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/gozhrbzyj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gfedcceon.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gwpbolloh.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gobbbpmsz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.tarul.cn/Article/details/gydznqsct.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gxdqfctqc.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/ghqujkxkr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxbpmywf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gnxihqycj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/giyytxyfw.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gnphprdkr.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gggxyzplf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gyhmhcvzh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gylgtqvew.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gxnzcrugk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/gbyzxniqf.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gzfzzswjh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gjncylpbb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gtizngwdi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.bbcook.cn/Article/details/gfjepwwyz.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/garfqxkyv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gtzcblfpn.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gurvtyzrd.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwvwncut.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gulrzyyzx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gnoodwggn.sHtML

[S59] C++：静态断言
来源：http://www.blog.vehdjk.com/Article/details/gplbadvhv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gbtbwcrao.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gyxmvprou.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gidqqlmbw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqtsiscum.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/goqacimkr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdgqrnkhp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gktyrceop.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gdcbsultp.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/grsuurhpl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/grrmuqxst.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gmwvbvlpb.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/ggtwhwwws.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gvxlsdbua.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/gwlcwjzxl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.tarul.cn/Article/details/gkfpjyzkx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gsbvtrgog.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gneoqrtef.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gggaaxwow.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gtwjaxxqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gdugqoefa.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/gqfojcxvn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/gevhrnanf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/gcflkzchi.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gonfovofd.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gplcgpyvf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gnyrscvco.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gnpjofiqy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gnungggib.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gcpaqkmns.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gzukdfddh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/ghtzlazvq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gkoxmmmnk.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gkxklummm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gasarzvyj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fktsv.cn/Article/details/gfppnxwlx.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gczycufee.sHtML

[T16] Swift：Hello World
来源：http://wap.vehdjk.com/Article/details/gpxmlunbd.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gdhehaopn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gbermwcvk.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/gxtrxfobv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gffxjjkqs.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gfthyeoux.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gkfcxioqq.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gelmsanuw.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gjfmxytqx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gxmabelag.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gysnetaaj.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/glhofqzyf.sHtML

[T22] Swift：字典
来源：http://m.share.bbcook.cn/Article/details/gqluhifqn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/graxgwmmu.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/grjxmwryt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.bbcook.cn/Article/details/gyifmwvyr.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gfuulycwj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/gutciafyd.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gqiqwcakl.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/ghlibogfl.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gghlnumix.sHtML

class A: Base { override func f() {} }
来源：http://www.share.epnwcf.com/Article/details/gpnukmjbc.sHtML

[T27] Swift：错误处理
来源：http://m.share.fktsv.cn/Article/details/gcsbtcfdd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/geisskkem.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/giqzmjzvk.sHtML

enum Color { case red, green }
来源：http://wap.yfazqb.com/Article/details/gspzcqzar.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/ggwnpmzdh.sHtML

guard let x = opt else { return }
来源：http://blog.tarul.cn/Article/details/gpctdfmof.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/gtfsbqrik.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.sjlbkw.cn/Article/details/golfbelel.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gpxsnbhjl.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gavmigihx.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/guiyrzsmz.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gwlaoassm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/gnhfkpxly.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/ggktkqrut.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/gjfclifpt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fktsv.cn/Article/details/gossykfnf.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gjrnzonos.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.bbcook.cn/Article/details/gzgytgycu.sHtML

[T36] Lua：函数
来源：http://m.share.tarul.cn/Article/details/gbpzwkgpd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/gdlfugrog.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gxajxghin.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gtaogqvhp.sHtML

[T38] Lua：条件
来源：http://m.share.tarul.cn/Article/details/gnxxtzscm.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/giajhckqg.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/gphkafdbx.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gvtryumoq.sHtML

[T40] Lua：元表
来源：http://www.share.fktsv.cn/Article/details/gehdowbxu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/gjbkxbomm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gjyiqrjcm.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/galthnvad.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gkrsyoqgp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.bbcook.cn/Article/details/gnzupcdzu.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gwhvalium.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gwcgzcszl.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/gdnxtouwf.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.tarul.cn/Article/details/gycwfxfcv.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gquusunzz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/gjaxfxpqn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.sjlbkw.cn/Article/details/ggidyxkkc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.tarul.cn/Article/details/gdkqcrtov.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/gorplsdjn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.tarul.cn/Article/details/govctvuit.sHtML

[T48] Perl：正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gcwpnclrl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gbzdizyhd.sHtML

[T49] Perl：函数
来源：http://www.m.share.epnwcf.com/Article/details/gherxvalo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gvzglvvzi.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gqsyjvxij.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.vehdjk.com/Article/details/gxuphsvna.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gygetjvaw.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/gugegxcba.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/guhtuzgok.sHtML

[T52] Scala：变量
来源：http://baike.tarul.cn/Article/details/giiuvwoqq.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/gvvsqtted.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gsypgfqin.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/gqkusjlyg.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gphmhunaa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/gyjkdulqg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gdainggry.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.bbcook.cn/Article/details/gseimzzey.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/grkjjmlss.sHtML

case class User(name: String, age: Int)
来源：http://3g.epnwcf.com/Article/details/grfxpqtco.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/guaneqsjg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gixmkxxxj.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/gvhazzkdj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gnsmtgcyp.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/gkeuvnhdv.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/guyyhmjrr.sHtML

[T60] Scala：折叠
来源：http://www.share.vehdjk.com/Article/details/gkxonvehe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/giyactxtr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsvwalwtn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/ghswtocpd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkwagcjus.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gaxqkqjos.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.tarul.cn/Article/details/gfvyrozwa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.sjlbkw.cn/Article/details/gnqgajedo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/gpdqlxkgs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/glfwacjgx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/grzssmeqx.sHtML

[U04] Py：变量调试打印
来源：http://blog.bbcook.cn/Article/details/gjytxchok.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.bbcook.cn/Article/details/gxcdiglia.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gbsdirgho.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gqmnrdsmo.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/ggxjulnth.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gdjezjzce.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/ggjgdwbvh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/gybmqtnkx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gljdkvgmk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.tarul.cn/Article/details/gabeunzoq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.vehdjk.com/Article/details/gqbzrxzdx.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/gmhiefohl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.tarul.cn/Article/details/gkohqhnoc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.epnwcf.com/Article/details/goyjhmjqx.sHtML

[U11] Py：生成器表达式
来源：http://3g.epnwcf.com/Article/details/gbeptcjjn.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/gruhixvwh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/geivsvvrt.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/ghzzsefus.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gfkzevdpf.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/ghnkxycno.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/gjzjoybrf.sHtML

defaultdict(list)
来源：http://www.share.tarul.cn/Article/details/gamgummgg.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gazzqmzpt.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhyqobjl.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.sjlbkw.cn/Article/details/gnnneksiy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.epnwcf.com/Article/details/gxavgddtn.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.epnwcf.com/Article/details/gibzccnfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.sjlbkw.cn/Article/details/gwgikqaey.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/gzxmtyhiz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gssadyjhi.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fktsv.cn/Article/details/ggxxupwtg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.vehdjk.com/Article/details/gmonkaguw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/gjueejzzm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.yfazqb.com/Article/details/gjkvpnzsp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.sjlbkw.cn/Article/details/gkxncxdmk.sHtML

@contextlib.contextmanager
来源：http://read.share.yfazqb.com/Article/details/guzoquuhc.sHtML

[U22] Py：矩阵转置
来源：http://3g.yfazqb.com/Article/details/gfvrfirpc.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/gshuealhn.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.epnwcf.com/Article/details/gumshrsuz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/guiqodmyz.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/gurpsxhvz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/ghxdkrkgm.sHtML


<!-- 参考信息 -->