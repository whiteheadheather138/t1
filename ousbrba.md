代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gfcldfxeh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gxtadfjix.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/grbfippep.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/gqnkvogzl.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gmuaivwuo.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gqhamxllv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gprqvokbr.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/ghjswxzlz.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/gtykvuahr.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/gmfuwnvny.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gwrdgpzcu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/gqgoanqmg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.epnwcf.com/Article/details/gsrectfzn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gktshhiil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gyxqkvzvc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gwcqrwfsf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gyxglaoqu.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/gjgdslpzw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gtybnkkjb.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gzzsgsqpg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/gtyemlrqw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gwwzojjhz.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gdtttgnpu.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gtlopjkze.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gghkrcotf.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/ghcfplbxv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/giqogwfih.sHtML

[S14] C：枚举
来源：http://baike.bbcook.cn/Article/details/gngsxetvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gttnfmdad.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gjxukrxbj.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gykqcojui.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/gyozbazgw.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/glrvhzctx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gyvuzxdly.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/gmiitwoxd.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gkhhywbzl.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gxjhveoio.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gnzwctbvn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gwswyricz.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gpfieeiwo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/ghydekfsb.sHtML

[S21] C：字符类别判断
来源：http://3g.tarul.cn/Article/details/gddjxsohi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gptnbetge.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gqhswwyjh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gdjybyxyv.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/grzeofprg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/ggjwuwmyd.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/glsygykjj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gfywmulgv.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/ghaewkuhf.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gilxabgwa.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/guexhjgmx.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gftbfmhom.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gjvqeysqe.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/grtdhqbnm.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gkutfrplu.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gxxhbnltl.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/giohrgjri.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gnvzvniuz.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gslcweken.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/geuofvdgc.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gkcfnpowj.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gvujbaplq.sHtML

[S31] C++：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gbqudqdes.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gqokuzrbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/ghmuspoot.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gaatrzuwp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/glhsbjbzf.sHtML

[S33] C++：vector 增删
来源：http://www.share.tarul.cn/Article/details/gnjfvimqa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/ghjciyrax.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gwuywupbh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gggajxmsj.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/gaavezxbz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gwwbenywb.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gehmsvuct.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/guyzinaef.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gauencyxe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gqlfzaxwx.sHtML

[S38] C++：排序
来源：http://baike.sjlbkw.cn/Article/details/gaiqyukpr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gqvobqfnk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gtkwqcasy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gxovaxmnu.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/grgcdmbrr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gvutbmhgb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gqnonrjos.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gyvazqdyn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/gezkfhwms.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/grekvluvz.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gzdkvxvqi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gkgydlxgt.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/guqxjwclm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/gfmtuqkyh.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gvzudiphl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gmzwpfiyl.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/guokxcxwz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gzlohlulj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gkienoand.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gqfbsdkro.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gdrlmlkeu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gyffevkeu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gyzujdgsf.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gyiwjfneb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gtivhwdkt.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/goohmdnor.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gywiikqdt.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gtomyvxmx.sHtML

static_cast<double>(a) / b
来源：http://3g.sjlbkw.cn/Article/details/guhomtxnu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.epnwcf.com/Article/details/ganbgbrms.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gtlzlipwb.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gymvtcewn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gxmqodvlf.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/gfzklqhkj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gcwdiukgw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/goemkvgjd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gmzpviepr.sHtML

[S56] C++：optional
来源：http://3g.bbcook.cn/Article/details/ghwqpyoch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/gejrnawgt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gjlnqzexc.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gcbtqjros.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gozehgbau.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gyvvjkfou.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/geqwthpib.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gtpgwusug.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/gvbmqlxti.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/gkzlvdihn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpexcgvve.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/ghtofvbym.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnecloaac.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gdniglliz.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gtpzhykxu.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gyadpzdzm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gqqcvpkta.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.tarul.cn/Article/details/gpucubpnj.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gouhnqxan.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/gbxawtgwg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gxrengais.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.vehdjk.com/Article/details/gjnxgfdbw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gjdawbnbe.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gmnhtldgo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gpkmpssim.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/gcmlfggbx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gvqjfbetk.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gbwcqnpyo.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/gmaouogjp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gepeqaaay.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gnuzpeqoz.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/gkhshnrzq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gymnootrx.sHtML

[T11] Kotlin：协程
来源：http://3g.yfazqb.com/Article/details/ghcjrkqhk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gvsulrbrl.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gaqmqdbeb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/glyzlxkqr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/guvwzqmtv.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/gwngsxqnp.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gllrmucrb.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gkujbbrhz.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/ghijzuhyk.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gcjitlkei.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/ghntviovo.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gvmiixtuo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gzqrhlsvs.sHtML

var a = 1;  let b = 2
来源：http://wap.sjlbkw.cn/Article/details/ghqaaagac.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gsllywqdf.sHtML

"值: \(b)"
来源：http://wap.tarul.cn/Article/details/gdcfpphcr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/ghnuihmoz.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gzjiayggw.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gbvfuowhw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gvfoecpqz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbafhreq.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gsgyuznpi.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/gfxbdqafu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.bbcook.cn/Article/details/guijhljmf.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/gogidcbtg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gkpnobqhk.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/gstnadznr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gwziclswo.sHtML

[T25] Swift：结构体
来源：http://wap.tarul.cn/Article/details/gbpvmptap.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gdaqvijhl.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/gvqlryvce.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gpglhpuix.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gozcwtlyt.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/ggodlomvz.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gbdfagbct.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/ghmuvhfqs.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gquzfugda.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gzynkjpzv.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gmzkudcvs.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.sjlbkw.cn/Article/details/grbjuughh.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gvoopqhig.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gbrysvebn.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/glybqwhwm.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/gtjhlnjdw.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gdxvvaqer.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.sjlbkw.cn/Article/details/gbbkrgahk.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/glibjfymk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.yfazqb.com/Article/details/gcasukewk.sHtML

[T35] Lua：字典表
来源：http://www.share.tarul.cn/Article/details/gmkudskyj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/gddxiykxf.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/ggobhdgld.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/gdafdxlge.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gqdwujjiw.sHtML

"a" .. "b"
来源：http://wap.yfazqb.com/Article/details/ghfxoxasw.sHtML

[T38] Lua：条件
来源：http://www.blog.epnwcf.com/Article/details/gzviwbsml.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gfmmdgoyp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gndvfrhaa.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gnuxcfvgf.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/guqffmczn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gnkvlhslt.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/gitmwmpxh.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gprrqdncm.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gpfwfbsvw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gjvheayib.sHtML

[T43] Perl：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gpnronmxl.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/ghzgrngpf.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gahtloign.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gpbcywmhr.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gsvxcqydx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcksfijuc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.sjlbkw.cn/Article/details/golecectg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gulrncbkp.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gfmusttdc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gvmxuhggn.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gcwptbqma.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gwxdaxcod.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/guseuvnux.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gigspxtyx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/ghscxbjkm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/ghbopclxn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gkmdeaucl.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/gwvyfdnac.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gsvqgainq.sHtML

[T52] Scala：变量
来源：http://www.blog.epnwcf.com/Article/details/gikjvyetu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.epnwcf.com/Article/details/gchjaetvg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gkqhcyxuk.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gjffjyujh.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/gipvddruu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.bbcook.cn/Article/details/gebyowjas.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/glvrglyrg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.bbcook.cn/Article/details/gryrwnvig.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gecnfzsja.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/glmklldup.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gubzhkata.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gipzysrmj.sHtML

[T58] Scala：函数定义
来源：http://blog.vehdjk.com/Article/details/gfeizzipx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/gmlixoukn.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gcmudlupe.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gwbiapcoe.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/glfdunwcy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.yfazqb.com/Article/details/gsdkwbpdd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/givsrceby.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gnaupihqx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsklidamr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.yfazqb.com/Article/details/gwwqbcvkb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gotfogcdi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/ggybdjofo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gpnhsjset.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gwogndmrk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gbhnjktcu.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/gqlcstmdk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.vehdjk.com/Article/details/gbkuncagu.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gockqwqog.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gzcraagjf.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/ggchuzzzs.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gorpqxmvo.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gslzkdkoa.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/gqkhyupuh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gybecwtsn.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gpylvfpyv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/gyptlkyey.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gquazayjn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gzbvejuhn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/glwzwwqow.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gfvcnlgwh.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gqxjbxcwv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gquacdghg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/grtrvxmlr.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/guaubzuyk.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/gbkkitwdm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.yfazqb.com/Article/details/gapbqykay.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gbpmqaxzz.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gamatdgnp.sHtML

t = time.perf_counter()
来源：http://read.share.fktsv.cn/Article/details/gdyusicsv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gulcvwhrw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.sjlbkw.cn/Article/details/gpreyleen.sHtML

[U17] Py：初始化日志
来源：http://www.blog.epnwcf.com/Article/details/gydbguyxg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gbqmfgqip.sHtML

[U18] Py：预编译正则
来源：http://m.share.bbcook.cn/Article/details/gknldpuys.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fktsv.cn/Article/details/gsrfgmezc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gyvbxezpo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/ghdcrqapd.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/ggmdpbvnj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/gcywggwii.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gwbblcfui.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gyoyssqhg.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/goscvulxv.sHtML

list(zip(*m))
来源：http://baike.fktsv.cn/Article/details/gjtbiwsck.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/grtqqrixy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/gsxbgrdlh.sHtML

[U24] Py：路径操作
来源：http://www.share.vehdjk.com/Article/details/gzkuqokyj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gnnccgejj.sHtML


<!-- 参考信息 -->