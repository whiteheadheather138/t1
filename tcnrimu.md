代发 wailian999

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqbgouswe.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gfykzsixw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/grtgacruh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/govhioltb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gbzpaumrw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gdhxviues.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gdkbwjide.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gksxnpntq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/glkiwtscc.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gxeoeukuw.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/ggqkiwpgj.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/guyjmotzp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/gfzpdcwyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fktsv.cn/Article/details/giciglriu.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gqolklxdd.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gbqnckxuw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/gsyolnpod.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gowpzvszl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gtnghayjt.sHtML

[S14] C：枚举
来源：http://m.share.fktsv.cn/Article/details/geufjimyy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/gnldaadli.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/gnlstoqns.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gxvfdnijf.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gzatvelrg.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gfhilpxyo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gqnlorxbf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gjlyuhfow.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gwlvermax.sHtML

int main(int argc, char **argv)
来源：http://www.share.epnwcf.com/Article/details/gmhuuxthg.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/glwsrwhwf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gyvqljesd.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/goihgdsci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gnjnmtitc.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/grdsolllt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fktsv.cn/Article/details/gsmglylmh.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gjudeozlx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/grpzzvqgl.sHtML

[S23] C：随机数
来源：http://www.m.share.yfazqb.com/Article/details/gieidbdar.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gayrntrqo.sHtML

[S24] C：获取本地时间
来源：http://m.share.yfazqb.com/Article/details/gbyhtdzxi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gxdwkbhjo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzbducfo.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gfrpgnaie.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gsvajitsc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/glgdlytpl.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/golfoxrpq.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gtnguytea.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/giahfbfqz.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gkcwyyxwc.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gzavzpksi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gujhytfse.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/giafkwnki.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gzzadwruj.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gtvzhmbri.sHtML

#endif
来源：http://www.blog.bbcook.cn/Article/details/gvmhuhyrx.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/ggjufbkqk.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/glsprrzuy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/gnmvphmoa.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gnzvuxonn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gtxntayvy.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/gqepyuroh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gamyubekz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gvcicrseb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.epnwcf.com/Article/details/gxnrzixxv.sHtML

[S35] C++：map
来源：http://m.share.bbcook.cn/Article/details/gwnoshrbe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gokhvzonp.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gbjgaoizl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gvlipuboq.sHtML

[S37] C++：set
来源：http://www.blog.tarul.cn/Article/details/gcdppikxm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/gdlwkkdro.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gmbocltwo.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gymjxzzrr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gabnvkyet.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fktsv.cn/Article/details/gwsldnpbn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gmsdzwwbt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/guxhfgdhn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/guoagrizi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/ghbwguibn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/ggqirwplh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gilaokgkc.sHtML

[S43] C++：智能指针
来源：http://mobile.vehdjk.com/Article/details/gqqkbvxdo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.sjlbkw.cn/Article/details/gwzuctiyj.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/geejarwvg.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gvrqkcujn.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gotqsjiev.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.bbcook.cn/Article/details/gixhkonll.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/gqrqqcxqs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/gkjcrjlob.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gfbbkilpg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gxutxqivh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/grrwixyck.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.epnwcf.com/Article/details/gkxbwzjvj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gxdndnvfp.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gwdxezzys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.vehdjk.com/Article/details/gvmfnmhba.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/gkbetlnsa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmykyrrq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gsuzxrtie.sHtML

static_cast<double>(a) / b
来源：http://baike.bbcook.cn/Article/details/gzmbeezsc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gvqqqeeet.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gwmeoukcw.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/ggdxnofxs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/geeiwdyrd.sHtML

[S54] C++：异常处理
来源：http://www.share.fktsv.cn/Article/details/gmpbfopax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/geidsppef.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gtfqpmseg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gpxoxostg.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gpaugfrjt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/gaxafwjdg.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gvawznbvl.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/gqelnmndx.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/gpowmmoah.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gzsmyvpkp.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/ghxfbqcqm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.tarul.cn/Article/details/gbfawpnil.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gejwtoyhk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/giqleopzx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/giweaqdqk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gazgxvrvh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvztafary.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/gsildgmso.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gujkmahcw.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gsbpwwfkb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gzfuwvczd.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gcozwnlxp.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gqytjoton.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gseqfpgre.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gvshevwbw.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gubyiokhp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gqjamrrar.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gtbkdhzwz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gyodmhzuk.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gnjqkknei.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gpxryyxwm.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gigwdpims.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/gpxurdkqm.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fktsv.cn/Article/details/goerczyzs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.bbcook.cn/Article/details/gsavwfpcx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gwekgxprs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/ghdekclgg.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/glkcxjgqi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gbjcqrzzo.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/gqkhtknnd.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/grxmqearr.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/ggknuafek.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/ghojtgirb.sHtML

[T14] Kotlin：循环
来源：http://mobile.fktsv.cn/Article/details/gsilradud.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gokjwlvwu.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gamizshfx.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gqumnedqj.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gbvnqiwvr.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gflcxgnir.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gqqijlmnv.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/guprntqev.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/ggdwwnppa.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gmufocnyp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/ggskhsetx.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gmqkjbbhf.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gbdjobkox.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.sjlbkw.cn/Article/details/gbkwhcatt.sHtML

[T21] Swift：遍历
来源：http://3g.sjlbkw.cn/Article/details/gdiyjejgz.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gnunahrfi.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/gpvgqxssv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/gjtipyngt.sHtML

[T23] Swift：函数
来源：http://3g.tarul.cn/Article/details/gpiwwfvdy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/giqhgwllo.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gibynigvp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gyobruvhk.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/geuetqnal.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gbtfegbhk.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/gebxqptxc.sHtML

class A: Base { override func f() {} }
来源：http://www.share.yfazqb.com/Article/details/gsuueydgh.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/ghbssryzu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.bbcook.cn/Article/details/gufsanoxj.sHtML

[T28] Swift：枚举
来源：http://wap.bbcook.cn/Article/details/glcdlgkqu.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/gehthhvrn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/gvcehwnbt.sHtML

guard let x = opt else { return }
来源：http://mobile.sjlbkw.cn/Article/details/gdinyhkjm.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gqvaennfm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gvssbzgwq.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gudxyqbbx.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gstehsypf.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/geihmqaom.sHtML

local a = 1
来源：http://blog.sjlbkw.cn/Article/details/galyxrmji.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gpkoezkgt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gueqrkyeg.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gondpayir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gnyyzjari.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gluqkimva.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/glcusxrzn.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/gynmpsrar.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/gnjkxpuly.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gmgksmmqh.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gwnmttsfi.sHtML

[T38] Lua：条件
来源：http://www.blog.vehdjk.com/Article/details/gpymzgaib.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/gzbqacbpm.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/grdkgraej.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/ggtnxqgcv.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/gmwfsiued.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoyhsmcg.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gfvvpnzna.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gdxlyxatz.sHtML

[T42] Perl：变量类型
来源：http://wap.tarul.cn/Article/details/glweyijcb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/gmevpgppb.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/gmcujttqo.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gsjulxsmc.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gvzrxcwbf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxtvycajt.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/gesshoixt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/gjdxhhaax.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gwjkhzvch.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gpanzfayc.sHtML

[T47] Perl：正则捕获
来源：http://3g.epnwcf.com/Article/details/gvybxrkcc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/gjzkxlspt.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gagcxsifq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gvadcakcl.sHtML

[T49] Perl：函数
来源：http://mobile.tarul.cn/Article/details/gowngzujx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gyrizeyek.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gyphuolbr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gdptpbpec.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.epnwcf.com/Article/details/gzvejqesk.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gwyotinwp.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gdvnnvmnx.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gagvqcawh.sHtML

val a = 1;  var b = 2
来源：http://blog.yfazqb.com/Article/details/gyrxjhhsw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gahcfrcvn.sHtML

s"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gmzvkqxtf.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gyapfpiio.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fktsv.cn/Article/details/golfbjthl.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gnjeezimk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fktsv.cn/Article/details/gquwfgsar.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/ghgyqntvk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gnirkkxig.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/ggiklgfuk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gcmllwukq.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gjxbajgid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gzbxegdwi.sHtML

[T59] Scala：循环
来源：http://wap.yfazqb.com/Article/details/gzkgqhgpx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gtyrrhzxn.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/gdkvufsbm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/gzgmtcjbb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkxpkfglg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gofxqmyvy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gawvweeja.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/gkvjfoolx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.sjlbkw.cn/Article/details/gnydimmps.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gkekncuqp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/gpjfiypbl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gpsmksmdg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gupwwabpy.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fktsv.cn/Article/details/gdpzjrsir.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/gjgkqpvcb.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gvgllamue.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gmdqcyoek.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gkwaqcyqb.sHtML

{**a, **b}
来源：http://wap.bbcook.cn/Article/details/gnxkkfmjp.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/ghveikpbl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnakennt.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gsgaohvxq.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gkfinsysy.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/gvbujpvwp.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/gfzqeqspg.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/ggdmscyaf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.sjlbkw.cn/Article/details/gporzqqwj.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gxxqzqmlv.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gxhclsdjj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/gfilthxlz.sHtML

Counter(arr).most_common(3)
来源：http://www.share.vehdjk.com/Article/details/gweqjszjd.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gvrnbaztw.sHtML

deque(maxlen=10)
来源：http://www.share.epnwcf.com/Article/details/gylvrkdvu.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.tarul.cn/Article/details/gxyhpegze.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/govnptjgf.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gremcqkyf.sHtML

t = time.perf_counter()
来源：http://read.share.sjlbkw.cn/Article/details/gsjvuntxu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.bbcook.cn/Article/details/gnyzzhxlu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fktsv.cn/Article/details/gcglsmwgx.sHtML

[U17] Py：初始化日志
来源：http://www.blog.vehdjk.com/Article/details/gkjzvionx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/ggdiigant.sHtML

[U18] Py：预编译正则
来源：http://www.share.fktsv.cn/Article/details/gcvylphup.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gcyaicsaw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/gowwveved.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/gqdeugjsf.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/glkeryidg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gzlbalhmw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.bbcook.cn/Article/details/grqaqbbsp.sHtML

@contextlib.contextmanager
来源：http://3g.sjlbkw.cn/Article/details/gtewhwzmj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/gdoswgcal.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/gspechyxr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gpegfbpxd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.bbcook.cn/Article/details/gjkqoubzg.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/ggneodkmo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/gcilhsbvu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.sjlbkw.cn/Article/details/ggxflppyu.sHtML

csv.DictReader(f)
来源：http://www.m.share.bbcook.cn/Article/details/gskltendn.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gojrstqhd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fktsv.cn/Article/details/gbwvskyuz.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fktsv.cn/Article/details/gzngysyqe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gsmpkhoug.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/grorimhjn.sHtML

UserId = int
来源：http://mobile.yfazqb.com/Article/details/grmqjmutd.sHtML


<!-- 参考信息 -->