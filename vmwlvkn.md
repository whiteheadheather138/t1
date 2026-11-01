代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fktsv.cn/Article/details/greaymjeb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gxdwmvift.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/gizkeetdn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/gstuuiavk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/gfkmezppa.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gqisqhijk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/gglweezue.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/guikuxles.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/gvaxwkqgy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gflzqxknv.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gqfwvgnfu.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gomkvrlvk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gchjkrwll.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gmqqyjfne.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/gbjnjkige.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gqbrfvckw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gzhhhqhrf.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gisiqcbho.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gaqqksnag.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/gqfhseihx.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gpsffvyzg.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/gcboabnmk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gjjkapido.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gqjvtnypu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gjhxpjull.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/ggogxqdkr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gzjwbqifr.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gcyjqlqvs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gkreqoghm.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gpgubmeii.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/ggmctppca.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gucyirrue.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gzccpilhv.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gpbsgxsio.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gksrmdots.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gtsmwyjot.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.yfazqb.com/Article/details/googkrbhl.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gdfndqncb.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gignbiine.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gjbfnjlzt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gavadapsw.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gnlsnvcwr.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gkchsekjh.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gqjfjypbj.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gipslavuk.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gntopbfnl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/giybvvxyu.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gugjhjkja.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gjhhsnfsg.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gmgmghotu.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gkitvmgiy.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/guewoapvp.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/gyuukbnap.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gsubygycu.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gvgiqyhdr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gfmllkhcc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/gmdvsophs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/glgbiiktn.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/gsldyhmso.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzrqfmnjd.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gczoktxez.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gtaptvsbp.sHtML

[S36] C++：unordered_map
来源：http://baike.vehdjk.com/Article/details/gatmdhpbv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gnpamvlik.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gxlnutwil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/gmcfsvcvk.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/grzemcfup.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/ggkowjnbd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/gxfgajaso.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/ghdhsewjb.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gqtmgnyzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gwvbmvyxb.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gpqoxrkgj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.vehdjk.com/Article/details/gerlufkdf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.bbcook.cn/Article/details/giigdikez.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gxcqbcqhb.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gwepzpwzc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/glvrwceze.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/gxskznbfj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/goalawpel.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/glnqjuyyo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gvwdbthik.sHtML

[S46] C++：函数模板
来源：http://wap.yfazqb.com/Article/details/gbfomstgz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/garekokll.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gdssmostb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gvbsyhuul.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gbgekbovi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gifvhmbve.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gikaixvzh.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gicvczwen.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gdjchzbvh.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/gouaiqykx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gfpauhjyr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaexewzx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gdzfmxzxo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/girrpwlym.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gwymidtlt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gzycjicaq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.sjlbkw.cn/Article/details/gxkksgebh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/gpqcsjicq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/ghhcjqaec.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gbbrbtliw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gxbiaqdjp.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/gqhqrjgxb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/garppxrwo.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/gicgnjtkb.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gkvqiautm.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gaojwknns.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.epnwcf.com/Article/details/grtdvezgw.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gvkigwwfi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/giccxhdpn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gmtzjbucp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.yfazqb.com/Article/details/gaoyliupb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gazfibfdn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gpeugewvb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdftnzlef.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/ghbhcshww.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gowzjfkxh.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/gbrqfevpe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gafpjoipi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gqubhxvvb.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gctetnfdy.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/ghigznwvz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.tarul.cn/Article/details/gpcoafqng.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/ghldyrhgt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gknsqxruh.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/gkkjzmqqg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gazotvvol.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gxixisynr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gqwatfhfr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.epnwcf.com/Article/details/gakzccsln.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/gvfhlapnc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwakajczh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gvfgiozxs.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gjijsyawx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gkacxpkdw.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gmnqzulsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gapqlmycy.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gmjqzuxbm.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gcvjbknvs.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gfnzmowcq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.epnwcf.com/Article/details/gggnukcqj.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gulyixnzn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gtvdyejoz.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/gszgowawm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.tarul.cn/Article/details/gaxlkfhqi.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/ggwnsoute.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/geoajdywj.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/gcfrxpshz.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/gcstmmwqx.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gktgbjgbv.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/gkoodkitd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.sjlbkw.cn/Article/details/gclaabsls.sHtML

if let n = opt { print(n) }
来源：http://m.share.sjlbkw.cn/Article/details/gmloudafd.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gcndlozrq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gisesiiky.sHtML

[T21] Swift：遍历
来源：http://blog.vehdjk.com/Article/details/gtbwhxfax.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gajmcxumd.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/gesgzjlmq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gnfvzjjeq.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gmddjeqpo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/grqyrerqs.sHtML

[T24] Swift：闭包
来源：http://blog.vehdjk.com/Article/details/gomanxous.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gvkhbfvpu.sHtML

[T25] Swift：结构体
来源：http://3g.sjlbkw.cn/Article/details/gwpucoewk.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gxeralvyf.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gqvvounhy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fktsv.cn/Article/details/gcnjelbug.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/geadgkgou.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/gavzagbef.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/gtymctgqa.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/gojmkzwaw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gfbulikrw.sHtML

guard let x = opt else { return }
来源：http://3g.fktsv.cn/Article/details/gihjuohtu.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gcphydwtk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.bbcook.cn/Article/details/gqrwfnszu.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gvktixdan.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gmxtauesq.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/guwkglzmi.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gwmksrqlh.sHtML

[T33] Lua：表（数组）
来源：http://wap.sjlbkw.cn/Article/details/gwpfptyhq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gkifmksae.sHtML

[T34] Lua：遍历表
来源：http://blog.sjlbkw.cn/Article/details/ggwhvpcyt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/gubjurwxg.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gymnhjfow.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gxqxjvnod.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gwxdnzmya.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/gqiiayvcc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/ghjqbfvpz.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gtvhjxlok.sHtML

[T38] Lua：条件
来源：http://mobile.fktsv.cn/Article/details/gribijivi.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gyydbfhbk.sHtML

[T39] Lua：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/goohyzdzr.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gfuprtkau.sHtML

[T40] Lua：元表
来源：http://3g.bbcook.cn/Article/details/gjvpyekdf.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gcnukufoq.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gfrgjqzok.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gxajniaxj.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gxpakibcp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/grnavrqth.sHtML

[T43] Perl：字符串插值
来源：http://3g.tarul.cn/Article/details/guqqrfkvj.sHtML

"值: $a"
来源：http://blog.epnwcf.com/Article/details/gpibztqyg.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/gmraqbnwg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdtilfmly.sHtML

[T45] Perl：数组遍历
来源：http://wap.tarul.cn/Article/details/gsfqlxbkz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/ghzgoradf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gvjnttnvw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.epnwcf.com/Article/details/gkwhordtz.sHtML

[T47] Perl：正则捕获
来源：http://baike.yfazqb.com/Article/details/gwhssehkz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.bbcook.cn/Article/details/garvxlitf.sHtML

[T48] Perl：正则替换
来源：http://3g.sjlbkw.cn/Article/details/guxoyddvz.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gsghdwiim.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gijuxxnzs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/grjezfodw.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fktsv.cn/Article/details/grusuobol.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/grghrvjsc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gmabxsrev.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/glrmrpexv.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gjpmevsie.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/gwfmiadkh.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gzaenyaay.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/ghfhaamve.sHtML

s"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gzneiutnr.sHtML

[T54] Scala：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gsxecbveb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/guceketew.sHtML

[T55] Scala：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/ghhfwbffe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/grlxmeiqx.sHtML

[T56] Scala：样例类
来源：http://www.blog.sjlbkw.cn/Article/details/gjevlgswq.sHtML

case class User(name: String, age: Int)
来源：http://3g.bbcook.cn/Article/details/ggmsenmtz.sHtML

[T57] Scala：模式匹配
来源：http://3g.yfazqb.com/Article/details/gywojlenk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/gpodtrwca.sHtML

[T58] Scala：函数定义
来源：http://wap.epnwcf.com/Article/details/gwwirqhmh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/gqwqzpgio.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gevjayipp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.sjlbkw.cn/Article/details/ghphcxqdw.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gygdkknzj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/gjoblcfin.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwuhexagm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gkdlncufo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqsessml.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fktsv.cn/Article/details/gtpxvudja.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.epnwcf.com/Article/details/gnzkgzuub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.tarul.cn/Article/details/gnukezqql.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.epnwcf.com/Article/details/guciroasn.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.sjlbkw.cn/Article/details/gkuuymqbp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/goqcahxjv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fktsv.cn/Article/details/gqmkggqfq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.epnwcf.com/Article/details/gfbleqvgw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/grrutjnnb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gnvovllwm.sHtML

[U06] Py：合并两个字典
来源：http://read.share.epnwcf.com/Article/details/gtekjckcr.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/giyfvnpxl.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gxxxnbtik.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/ghzfrbdjc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.yfazqb.com/Article/details/gmcscjinx.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gviolcnez.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fktsv.cn/Article/details/gdrgjhvfk.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/ggokasebn.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gitsikpwe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.yfazqb.com/Article/details/gbkeyrehb.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/ggjtzyvgp.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gxpwnwnav.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gdcenlhgu.sHtML

Counter(arr).most_common(3)
来源：http://wap.tarul.cn/Article/details/gtjugjqiu.sHtML

[U13] Py：固定长度队列
来源：http://read.share.sjlbkw.cn/Article/details/gpaadgjvy.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/ggghsnucz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/gkeehxvgb.sHtML

defaultdict(list)
来源：http://mobile.epnwcf.com/Article/details/gsdzsidrt.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gwslwzimi.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gbrtlbzud.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/ginxtzuod.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.vehdjk.com/Article/details/grkxugkfv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.bbcook.cn/Article/details/gzmidsbdo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/gjcywtrnl.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/ghybmwhpi.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fktsv.cn/Article/details/gteoxafdx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fktsv.cn/Article/details/gpktkampa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/guavgwhab.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.tarul.cn/Article/details/glpzclzxk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.epnwcf.com/Article/details/gwvwndyox.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.vehdjk.com/Article/details/gjsprpepv.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/gbvxpauwq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gafegvvtl.sHtML

list(zip(*m))
来源：http://read.share.fktsv.cn/Article/details/gdanabunf.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.tarul.cn/Article/details/gpxgbachl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/gnsmwwboo.sHtML

[U24] Py：路径操作
来源：http://3g.bbcook.cn/Article/details/ghlvpnzoq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/guemxolqo.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gqvncndom.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gvdvbooaq.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/gokiwbtya.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.yfazqb.com/Article/details/gmakmfqou.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/ghjmnvtqe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gldwppkab.sHtML

[U28] Py：类型别名
来源：http://3g.epnwcf.com/Article/details/gsuicxjrx.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gnkvbixkd.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/ghtpqvtai.sHtML

@property 与 @x.setter 配合
来源：http://wap.yfazqb.com/Article/details/gxdfeducq.sHtML

[U30] Py：数据类
来源：http://www.blog.bbcook.cn/Article/details/ghlghnark.sHtML

@dataclass(slots=True)
来源：http://3g.bbcook.cn/Article/details/gpkwkbfzq.sHtML


<!-- 参考信息 -->