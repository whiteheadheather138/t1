代发 wailian999

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gnhuogiqq.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gstuivbiy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gafkrbooo.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gzzgumfkk.sHtML

strlen(s)
来源：http://baike.vehdjk.com/Article/details/ganosjjhx.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/ggrututfa.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gucuovmwz.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzdzjzob.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gwzwotyfv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/gytcajjbm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gjobffkou.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/guddqzirz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gimlnnbgt.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gwfqetvhj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gbautycvk.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gvdjqocoe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.bbcook.cn/Article/details/ghuybsilq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gviaprxqw.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gjngcmfkm.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gfjvjxyzt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gflvtverr.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gakquivfp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/gohmzbika.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gzmhdtdyc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gqoflridg.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gblpwalqn.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gnisijiww.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gourpcvzp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gfoxbmzli.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/ghudqcwwi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/gyggbljeh.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gnrptpyva.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gpdhptadc.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/grrtthmle.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gawejnkbz.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gfnpqdwrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/guzgeapla.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/gnccmgqev.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gbhvrazlm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gvnruiyrt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gfwrapvwe.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/guvkwylse.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/gxnwidaux.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/gzcjdlxbr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/ghgwkgbtr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/ggewywsdp.sHtML

memcpy(dst, src, n);
来源：http://mobile.epnwcf.com/Article/details/gfappcegu.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/grilyytrf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gfkttwrcy.sHtML

[S27] C：定义常量
来源：http://www.share.sjlbkw.cn/Article/details/gxdcvtapd.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gfmhbsylu.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/giawpizly.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/gggmhjlqm.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gvgwxlpgr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gvsilxasi.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/ggvoobnxq.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gqdayucws.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gahgepkbb.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/ghoucsllg.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gvnguxfah.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gbzdwkrxz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/gkjzawjmu.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gtoryhpaa.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gfqjydpxv.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gjavukdxd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fktsv.cn/Article/details/gdyhwzuia.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gwsialnpi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/gkkanuumv.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gvsjmkbia.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gfqocrzvd.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gxjktpuxi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gyjmruvvh.sHtML

[S37] C++：set
来源：http://3g.yfazqb.com/Article/details/gzvjpikac.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gblowedvt.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gdkgvluof.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/glrbuoecc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gmooduqnl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/giwqmcruv.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gkcodtqyt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/gmxptjzfy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gtlknacgc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gificscvl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gcelywnqz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gibfpsfej.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gpsxcclsl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/ghhdtbchq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/gkecgczxy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gylclqjkp.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gojggpxet.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gxxrelseq.sHtML

[S46] C++：函数模板
来源：http://www.blog.bbcook.cn/Article/details/gfnxqehte.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gyfwjsaeb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/gwqyasrjd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/ggtqpqjlt.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gcudcqpir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gelrjwpql.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gkyttunws.sHtML

[S49] C++：写文件
来源：http://wap.fktsv.cn/Article/details/gfsfwuiwx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gjgbtoqiw.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/gpedadqvr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/govszydap.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gkjgurfnx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gngrfaeeb.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/ghrpxstmr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fktsv.cn/Article/details/gdewewlry.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/grpljsvxd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fktsv.cn/Article/details/gsfqfjywf.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gxnckcjnu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/gjkjiolup.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gcxfybnyv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.bbcook.cn/Article/details/gnbhrccup.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gxswfqaaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gauzvpfzu.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/gwssumnsd.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/gxhekmdey.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/grwcdwbfw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gryxmsuev.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/glhwaqgxg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/glralyktm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/ghfzisesr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gdjezzzzy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grpmbigwj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gdjdpapjz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwviubgdn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gmfkphavg.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gzzvrgipd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/ghscvcakm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/gnphiywbg.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.epnwcf.com/Article/details/guftozdns.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gehvozhnu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gibgmqgqu.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gfwsvczne.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gpzqwctvi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gmrnibrou.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/ggueqmnhy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.epnwcf.com/Article/details/gbainhnng.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/gehjzkfrm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/grbdqglcr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gytezukpe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gvknxrsch.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gneuwztbw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gdsycqgjh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gncetekdl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.epnwcf.com/Article/details/gzblhuvoq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/ggofkormo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gpkrbzuph.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gdedqxbrs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gcsicntgs.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gdloupyui.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/gupnooqan.sHtML

[T14] Kotlin：循环
来源：http://read.share.yfazqb.com/Article/details/guzgvbhki.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/giworoath.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/grnbilhgz.sHtML

interface Shape { fun area(): Double }
来源：http://blog.bbcook.cn/Article/details/gjnmxbkzv.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gzndypedv.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gyfojqtoi.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gchtdwjqd.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/glebtjhca.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gxtoybmdr.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gdfewwzro.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gxewncrjt.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/ggigykjbq.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gbxezdbrs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.yfazqb.com/Article/details/gohkxgopo.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gbgmrxlek.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gplbgypch.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gdsgloexx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/gpslkipok.sHtML

[T23] Swift：函数
来源：http://baike.yfazqb.com/Article/details/gsgjapxdf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/grnazesxb.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/gxjmzzzzf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvxbsrva.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/gvhzcmrmp.sHtML

struct P { var x: Int }
来源：http://www.m.share.tarul.cn/Article/details/gqsgbqoox.sHtML

[T26] Swift：类与重写
来源：http://read.share.epnwcf.com/Article/details/gghikjjud.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gbqiweqvn.sHtML

[T27] Swift：错误处理
来源：http://www.share.tarul.cn/Article/details/gpxcxiuso.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/geuafnqgz.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gdyjefwtp.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/gctfxcenl.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/gbsdvxkus.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gjqyzbnxy.sHtML

[T30] Swift：协议
来源：http://read.share.fktsv.cn/Article/details/glspyhrmw.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/gsfuecatl.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/gpjhlrezp.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gxdgndujb.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gijdsjbpf.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gmhsncrwm.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gyzjvojay.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.yfazqb.com/Article/details/gjokjttha.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gwrahyngx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.tarul.cn/Article/details/gsdfaqqdb.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/guuhcetol.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/ghjlqwhuh.sHtML

[T36] Lua：函数
来源：http://www.blog.tarul.cn/Article/details/glslgaoih.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/genaqjjve.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/gmdxthbpd.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gtsekgzla.sHtML

[T38] Lua：条件
来源：http://read.share.bbcook.cn/Article/details/gniykmdoi.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/glrsuvaic.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gadefecrc.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/gbsnyeddu.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/gcfsrjnny.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvwpwijk.sHtML

[T41] Perl：Hello World
来源：http://mobile.tarul.cn/Article/details/guabdprii.sHtML

print "Hello\n";
来源：http://www.share.fktsv.cn/Article/details/glksbwgmf.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/gvuihmtrn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gbthmunlx.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gqagkbrxj.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/gysvzdfhq.sHtML

[T44] Perl：条件
来源：http://3g.sjlbkw.cn/Article/details/glelcmtij.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.sjlbkw.cn/Article/details/gpfupmxcj.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gszuqhfrs.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/guunzvaqx.sHtML

[T46] Perl：哈希操作
来源：http://baike.sjlbkw.cn/Article/details/gykbrxthg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.yfazqb.com/Article/details/gbfwzksma.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/gszqxnjda.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/gvowtwowa.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/ghkrewbxb.sHtML

$s =~ s/old/new/g;
来源：http://3g.yfazqb.com/Article/details/gbzioygas.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gpfqeecnl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/ginubnvud.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gfrxdkvta.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gpigdkrra.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gydaxajlh.sHtML

[T51] Scala：Hello World
来源：http://mobile.epnwcf.com/Article/details/gxxlxlnys.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/glzvylafl.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gygzxqifp.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/gvxlhklig.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gilljygfz.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/ghaeszmqx.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gbujmyqet.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.sjlbkw.cn/Article/details/ghekrtpuu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gexjwvsdv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gmaxhshsz.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gmvaouaug.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gsczntbak.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gptidctyw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gmcrietao.sHtML

[T58] Scala：函数定义
来源：http://mobile.bbcook.cn/Article/details/grcwbqtam.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/gatbmutlb.sHtML

[T59] Scala：循环
来源：http://www.share.vehdjk.com/Article/details/gqaccapdc.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/gclvfzioq.sHtML

[T60] Scala：折叠
来源：http://wap.bbcook.cn/Article/details/gkqgsrflj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.epnwcf.com/Article/details/gijlfyeeo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwsnvpukp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gddicaeki.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdeusgnvz.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gukgihutp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fktsv.cn/Article/details/ggzkbwkcw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.vehdjk.com/Article/details/gnzjqstrb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fktsv.cn/Article/details/gwvhainfs.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/gwphwbhpz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gykoywhad.sHtML

[U04] Py：变量调试打印
来源：http://baike.fktsv.cn/Article/details/glzrhhakg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.tarul.cn/Article/details/gliplmlnx.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gfhcjobzo.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gkqjfrppo.sHtML

[U06] Py：合并两个字典
来源：http://wap.yfazqb.com/Article/details/ghsmpepsm.sHtML

{**a, **b}
来源：http://baike.fktsv.cn/Article/details/gxqidkjqj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.yfazqb.com/Article/details/gfuqlmcyn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.bbcook.cn/Article/details/ghitqigcf.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/guuonwsbw.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gzmxykrky.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/gdnclljbn.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gorhhhmbj.sHtML

[U10] Py：按值排序字典
来源：http://blog.bbcook.cn/Article/details/gvzhnautv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/gswmckmiy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gsbezjpsi.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gucopfxol.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gjaktsggi.sHtML

Counter(arr).most_common(3)
来源：http://blog.tarul.cn/Article/details/gqwxbahzv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/gjehlwyjn.sHtML

deque(maxlen=10)
来源：http://wap.fktsv.cn/Article/details/ggkkaytxu.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.vehdjk.com/Article/details/ghksrltqh.sHtML

defaultdict(list)
来源：http://www.m.share.yfazqb.com/Article/details/ggwtcispt.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/gidgheien.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gcxypcfys.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.vehdjk.com/Article/details/gyqdvtiqm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gpcqjyvrf.sHtML

[U17] Py：初始化日志
来源：http://read.share.sjlbkw.cn/Article/details/gbpqfnrhr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.epnwcf.com/Article/details/gtxxiemcn.sHtML

[U18] Py：预编译正则
来源：http://mobile.fktsv.cn/Article/details/ggjtwwror.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gkhclkubp.sHtML

[U19] Py：正则替换带回调
来源：http://baike.sjlbkw.cn/Article/details/ghkauheje.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/grnjaztvq.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fktsv.cn/Article/details/gcnyjcjmu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/gsjoqjbau.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.epnwcf.com/Article/details/gwnblpgxi.sHtML

@contextlib.contextmanager
来源：http://mobile.sjlbkw.cn/Article/details/gddctgjbf.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/gcwcyerxe.sHtML

list(zip(*m))
来源：http://mobile.tarul.cn/Article/details/gdxrekrgp.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gptylesho.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.bbcook.cn/Article/details/gfxipluyy.sHtML

[U24] Py：路径操作
来源：http://baike.epnwcf.com/Article/details/gegoxyzdo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/grhxwjogt.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/gnqbjgwyj.sHtML

csv.DictReader(f)
来源：http://www.m.share.bbcook.cn/Article/details/gajhankmq.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/gprjwoixi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.yfazqb.com/Article/details/gottwbcsc.sHtML


<!-- 参考信息 -->