代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/goabxdaut.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/gxidgcpmp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gmzasvten.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.bbcook.cn/Article/details/gyxbbyakt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/gytduzxvl.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gaxehzmcd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwauemkni.sHtML

[S11] C：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gkdqgmnoe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.bbcook.cn/Article/details/gpdksgwln.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/ghllasaan.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gyeirkbqa.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gxfgmpkal.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gxwdemyoi.sHtML

[S13] C：宏定义
来源：http://wap.fktsv.cn/Article/details/gylgnwcqw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gulccftkt.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gcsvtmkzi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/giuhwspic.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/gvihifvbu.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gdbwzfwyd.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/gdothjtxr.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gsyjwzyrd.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gvnuepoqd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.vehdjk.com/Article/details/gvrbfnlmi.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gwbjajrei.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gmqxrcbum.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gwglmkgub.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/ggnbxyncm.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gcsqehxfw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gdwswvigh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gacskbgvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/ggqidwzvv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gbjpfbdyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gnjdlfesh.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gcpdtouix.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/ghzksfaje.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gconstptl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gbgvrgcdm.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gtaeeitja.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/geuexotse.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/grmhcntof.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gnqsigeuw.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/geukaeckl.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gspkrbhok.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/ganshitxq.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/giuawauxd.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gwnauwpes.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/guaawwvol.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gtpeyxxuo.sHtML

#ifndef X_H
来源：http://wap.yfazqb.com/Article/details/goktgvlht.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gnpyliaxj.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gqdujbble.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gfldlvjjn.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gpfeqtqcs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gmtyjlues.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/gouscifxo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gzmgczlux.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gkihvauzv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/gkasrsguu.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gvxvuqgjv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/gnuqpguiy.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gmqstmwji.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gzrqmrmig.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gdjbnlidi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gsdkhhfrf.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gufwusvfd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/gchlfnnme.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/gqxdvdqhu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gtzxkcunu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.tarul.cn/Article/details/gzvyhfqpg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gveuqkdcv.sHtML

[S40] C++：查找元素
来源：http://wap.tarul.cn/Article/details/gthnbgyzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gtlwnqbnn.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gglwzqaky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gjbvvtqhb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gscdqorfy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/ggadgxyhb.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/gkbixpjzn.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fktsv.cn/Article/details/glsxtejop.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gcdckqxjh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gqkeoogbk.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/ggsylxdgs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.bbcook.cn/Article/details/gkxnnmosj.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gtvtqiwcu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gedwvqvut.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gjpbvyocr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.vehdjk.com/Article/details/grsnkxuqe.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gyljoswyy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.yfazqb.com/Article/details/gsjrmovci.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/guxhqwobx.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gtlfffnux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gicgitkon.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/glnvvairz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gwdoaosai.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/gcbgfefaq.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gunjgjqsw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gjhdimubt.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gnzjvqvla.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gqtajvpgl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/giumzagjl.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/ggmrrjnbc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/gqshqdnmd.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gyxyuinew.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fktsv.cn/Article/details/gfadlpqrx.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gozahveob.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gtsqebmjy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrjirgsq.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/glytbrwyv.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gtnvnphkl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gozwqoyil.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gytdahfel.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gefykqzfy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/grwppzpsz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gczzhkbiw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfgtigdgk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gegsbzuev.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glkgmhoff.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/ggokwxqgu.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gtmwdbcvw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpbdwjog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gezckgpdz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gkcjtpvgc.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gxtwbfwce.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gfjdtpuhp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gerhurbbn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gpyafskho.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gcvdaehrm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/grmufrpqy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gvyooggcs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fktsv.cn/Article/details/gqvkgqpit.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gjcetjaky.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gnbdszklk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gzhlxroqx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gboxilfuq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gbthwhggk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gpmgbenmb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.sjlbkw.cn/Article/details/gfpfggxkp.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gkwbkymox.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gwmazwhto.sHtML

[T12] Kotlin：解构声明
来源：http://baike.tarul.cn/Article/details/gxfmfkyzo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gvcjfuruz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.epnwcf.com/Article/details/gjztqtabx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gyrnwmgnh.sHtML

[T14] Kotlin：循环
来源：http://blog.fktsv.cn/Article/details/gcbsgpjtr.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/gpcavoano.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gqrbkfxpx.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/gypgcurne.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/giypgydre.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/ghejmmjvl.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gjjfnpzyz.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/gcqhzozpo.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gnjfizals.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/gvdsaifav.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gggmgwfps.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gvtpxcfcy.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gavfjmssd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gxyjecmzn.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gmeuarsce.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gxterbqrd.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/gbonrvdaj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gqywtvklm.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/gyambtqaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gmoakoosq.sHtML

[T24] Swift：闭包
来源：http://blog.sjlbkw.cn/Article/details/gcqgkcfnc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/golgsuwum.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/gjvasdsoq.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gizljhyjo.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gvbvjudfr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gepyuiwfo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gkuklpjcy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fktsv.cn/Article/details/ghbujbbwz.sHtML

[T28] Swift：枚举
来源：http://baike.sjlbkw.cn/Article/details/gebuelfol.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/glibvtyzy.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gifzezxyg.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gpfdlvbcm.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gbwdugpgl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.bbcook.cn/Article/details/glvpadzbx.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gryrtibqg.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/geiuikjjm.sHtML

[T32] Lua：局部变量
来源：http://3g.bbcook.cn/Article/details/gyjmtyqrh.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gyigclkdj.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/gnkxkjitj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gbvsikiyp.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gekeegqek.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gsdxanxsf.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gtfmjuvfa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gzoldihqj.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/grgmbktvu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/gylfyquac.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/ghbbgagec.sHtML

"a" .. "b"
来源：http://read.share.yfazqb.com/Article/details/gvtylmmlu.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gblgqgqkj.sHtML

if x > 0 then print("正") end
来源：http://read.share.sjlbkw.cn/Article/details/gmckyixeb.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/glpbnpdcp.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/ghmxmjtem.sHtML

[T40] Lua：元表
来源：http://www.share.fktsv.cn/Article/details/gotsvctkx.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.yfazqb.com/Article/details/guilzvzpo.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gayizydjd.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/goyomcbti.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gjyczsjii.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/ggfukvana.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/godzakfpz.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/guhgskfer.sHtML

[T44] Perl：条件
来源：http://blog.tarul.cn/Article/details/grfkmjejw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.yfazqb.com/Article/details/gwqciucys.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gvnogdfsa.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/geafuymfv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.epnwcf.com/Article/details/guikwcmtx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.sjlbkw.cn/Article/details/gjtjbqnbc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.sjlbkw.cn/Article/details/gaiuvuqed.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gahfmgjaa.sHtML

[T48] Perl：正则替换
来源：http://baike.epnwcf.com/Article/details/ggjnpxsaq.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gydangdvh.sHtML

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/ghfscwfqo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gduxwqtjg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gklnyyssc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.epnwcf.com/Article/details/guqzdihtj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gbqsqurkd.sHtML

[T51] Scala：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gzjcahjca.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gphleeglm.sHtML

[T52] Scala：变量
来源：http://www.m.share.bbcook.cn/Article/details/gzznqpxuu.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gabsvniph.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gzqszadit.sHtML

s"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gywacbnot.sHtML

[T54] Scala：集合映射
来源：http://www.share.bbcook.cn/Article/details/gzjanychx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.yfazqb.com/Article/details/gdlfcczet.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gqetcibdt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.yfazqb.com/Article/details/gfrryywkh.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/gejrkkxaq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gozkmhfdq.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gcdrrjuek.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/girxxkqez.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/ggpmxyxzn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gfduuiulj.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gshrybjwt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gugkmmgvp.sHtML

[T60] Scala：折叠
来源：http://m.share.epnwcf.com/Article/details/gjlmlvokc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gtlenxanx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggssltuyt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/glwwmrzbh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggwfpsnuw.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/grxtqzywe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gxpamukqo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gudagtgfz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.bbcook.cn/Article/details/gonyxhhog.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/germmmqyh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.epnwcf.com/Article/details/ghcmwgtlj.sHtML

[U04] Py：变量调试打印
来源：http://3g.yfazqb.com/Article/details/geaxowueq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gaygpgwru.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/geejlkopi.sHtML

list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gqtiowdoc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.sjlbkw.cn/Article/details/gtbqacsob.sHtML

{**a, **b}
来源：http://www.share.yfazqb.com/Article/details/gfxfdztsf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.sjlbkw.cn/Article/details/gidtkbehm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.vehdjk.com/Article/details/gijwjmfac.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gnfpepeko.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gidyswpxm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/gbnblfrtj.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/gbkqwvmtu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/gjwkvixse.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.bbcook.cn/Article/details/gfmmqwmmu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/grgyofpbt.sHtML

(x * 2 for x in arr)
来源：http://blog.vehdjk.com/Article/details/gqesawazb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gsyrditng.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/gmzicqccr.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gkjruiajp.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gwqdgqfdy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gzsjgdwrx.sHtML

defaultdict(list)
来源：http://www.blog.tarul.cn/Article/details/ghnugkdia.sHtML

[U15] Py：高精度计时
来源：http://m.share.vehdjk.com/Article/details/gxzheauiw.sHtML

t = time.perf_counter()
来源：http://read.share.tarul.cn/Article/details/grefampit.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.bbcook.cn/Article/details/gijjauxuz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.epnwcf.com/Article/details/gkwdueakx.sHtML

[U17] Py：初始化日志
来源：http://m.share.vehdjk.com/Article/details/gfdcxbmdw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.epnwcf.com/Article/details/guiiazbhz.sHtML

[U18] Py：预编译正则
来源：http://read.share.sjlbkw.cn/Article/details/gueaqfkyr.sHtML

pat = re.compile(r"\d+")
来源：http://baike.bbcook.cn/Article/details/gcbxrhsvf.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gcrgrvlqu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.yfazqb.com/Article/details/gibumppme.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gjxhujiii.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.tarul.cn/Article/details/gvbnxboqc.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gqidxwmiu.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/ghywxagse.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gyjugmjtk.sHtML

list(zip(*m))
来源：http://m.share.bbcook.cn/Article/details/gcycbbgdm.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fktsv.cn/Article/details/gesuuacci.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.bbcook.cn/Article/details/gkrywhqrg.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/ggztcocjt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gpvityzlq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/gzeuseved.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/gafcxmpto.sHtML

[U26] Py：并发下载
来源：http://wap.bbcook.cn/Article/details/gncaobltz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.vehdjk.com/Article/details/gjnuyohaw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.sjlbkw.cn/Article/details/gdpcjtnmx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gxfrdjwyk.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/gddhcjgbc.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gvjjmysme.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/gqvpqumad.sHtML

@property 与 @x.setter 配合
来源：http://m.share.yfazqb.com/Article/details/gskiedfck.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/gnctuibis.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gjynswvgb.sHtML


<!-- 参考信息 -->