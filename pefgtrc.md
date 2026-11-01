代发 wailian999

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gmlmdsvap.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gtnaexgfm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gikwqfkcl.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/genjrilwo.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gixlplmzf.sHtML

[S06] C：字符串比较
来源：http://mobile.yfazqb.com/Article/details/gbdyylcjx.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/gwynwoxbp.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/gnihunibq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/ggypiebfn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gulogmkmc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gkrwvywix.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gixeokmgi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gbycldmdn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gozidcxka.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gefxwwhvo.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gdgcocqhs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gwmqhlxgt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/govhumbju.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gzuxjrmnz.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/ggoicoxxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/gdvgpxmzt.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/gcyplyoze.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gwitkuyid.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/govypsbux.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.sjlbkw.cn/Article/details/gbukovhus.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gcrzndssg.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/gjjttozny.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gowrbhuhi.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/gzrtizpcs.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/getvluujk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gcyrtyjzw.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gcdllatzt.sHtML

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/giwkeijff.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gaflvzkej.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gqzibkvfm.sHtML

[S20] C：二分查找
来源：http://wap.bbcook.cn/Article/details/gdtoavreg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/ghyvvzuuo.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gjgqlbiol.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gmqiqesmw.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhqywnux.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gvuflcfyk.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gnwqltqsl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/ghmwfgimv.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/ggkrrdytz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/gmwlvwzcv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gulekkhpw.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/glrxmuxjb.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/gcqsiiore.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gpngxagqw.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gehnrpbhm.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gknmocgte.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gksuulfso.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/ghltedbbi.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/glmyaeype.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gnxuenbov.sHtML

[S30] C：头文件保护
来源：http://www.blog.bbcook.cn/Article/details/gwpgutijl.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/glgkcjjda.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gpnaalvqk.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/grjvyfqsy.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gjtydavyg.sHtML

#include <iostream>
来源：http://wap.vehdjk.com/Article/details/geubwtvck.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gfpnbgeav.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gijyqcphd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gaycyusmr.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gyuxjfdmq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gvwwppatp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gtqsjzono.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gtlxcwjug.sHtML

[S35] C++：map
来源：http://www.blog.bbcook.cn/Article/details/gjuzlfmub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gnovbddmq.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gtompugnq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gxvyhnltz.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/gdvxalqdh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/ghjrrsxfp.sHtML

[S38] C++：排序
来源：http://www.share.bbcook.cn/Article/details/gzjhjmtaf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gcqmviyau.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gkoixjlaz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/ggppzlvcy.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gwxbmndzs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gaankudro.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gkoubctps.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gxyzeboql.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/grosgqnhn.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gbpgjsolt.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gtpjongze.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/guliklptd.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/gbwrjlmbh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gwudymzin.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gmgczhugi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.tarul.cn/Article/details/gssertqxy.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gumyizmun.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/gntjvnjtt.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gxczvfdks.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gfrcfgecq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gnbyjiduj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/goiehpbok.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gahcopyyw.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gyamamulc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gapvvkfvt.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gokmvsxdq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/gbjkyckus.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/gjtzjyfok.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gkslytrnc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gxtvlndba.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gxiebpxvb.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gkiybjfdn.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gmelguopr.sHtML

[S54] C++：异常处理
来源：http://m.share.bbcook.cn/Article/details/grfxqqxcj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gogrbumxw.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gcuereuku.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.sjlbkw.cn/Article/details/gtewzbgcr.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gbrahjoin.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.yfazqb.com/Article/details/gnoknhqbd.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gascargcc.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gaifnjjhu.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gonxvrbun.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/giocfpqrl.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gdncqusnw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gxswmeniu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gzpscuknm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gcbmxkaxb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjotfkkzg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/godwzgfnw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gycvmfzki.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gagbeogvt.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gqirbqcef.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/gygknnqbw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gcmjzyfoy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/geyyjekfh.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/guwmdywin.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gcqtofahr.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gajnrncrb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gwmamuyqf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gevwipsmz.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/ghoyandrz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/guyhfuunn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/guptuiqfz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gbgrgayuq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gtyejhuma.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gslqbuayk.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gydolkoor.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/gagahgakb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gtqgojmtr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/gibuawzmo.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gfubwenns.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.vehdjk.com/Article/details/gtgqnvwpo.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gxdgdlsey.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gpdnmckjb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/gnuvznjpk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/groocpgim.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/gcfpklmmo.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gzyslemfu.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/gbkroadel.sHtML

interface Shape { fun area(): Double }
来源：http://blog.yfazqb.com/Article/details/ggfkfiiyf.sHtML

[T16] Swift：Hello World
来源：http://read.share.bbcook.cn/Article/details/gosvwksui.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gssdcifcu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/grbtpdsyr.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/ghqxjvabg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gnjcyomgb.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gjndflvak.sHtML

[T19] Swift：可选绑定
来源：http://baike.sjlbkw.cn/Article/details/gjuhkalpf.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/geuxzhooi.sHtML

[T20] Swift：数组操作
来源：http://3g.tarul.cn/Article/details/gdhjmlxmh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gdncizjvv.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/gwtfrowiw.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/gdpcbmlfy.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gflwwnkml.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/gdevkngfy.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/gpkhnbrfv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fktsv.cn/Article/details/glimcdfpf.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gmrdckntu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gputtsugz.sHtML

[T25] Swift：结构体
来源：http://baike.epnwcf.com/Article/details/gueiuqucz.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gkdgagzun.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/grynwpirh.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/ggrepnrjz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gwsiaysbm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.sjlbkw.cn/Article/details/glvtgolnx.sHtML

[T28] Swift：枚举
来源：http://m.share.sjlbkw.cn/Article/details/grsajkjkf.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/ghwkygnmc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gejtaytxw.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gswozwzcv.sHtML

[T30] Swift：协议
来源：http://m.share.yfazqb.com/Article/details/gsxmzmoqo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.sjlbkw.cn/Article/details/geytkspea.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gdxmyflfp.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/goibjzmtm.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gntpyjndb.sHtML

local a = 1
来源：http://3g.sjlbkw.cn/Article/details/glwdzlgiq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gqvmzplac.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/gpighrmil.sHtML

[T34] Lua：遍历表
来源：http://wap.yfazqb.com/Article/details/gkmhftyfy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/ghtcjnyem.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/gdtidggos.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/gfwkjchrq.sHtML

[T36] Lua：函数
来源：http://blog.yfazqb.com/Article/details/gespdjvbt.sHtML

function add(a, b) return a + b end
来源：http://www.share.fktsv.cn/Article/details/gxzyjzdsp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/ggzjudewg.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gxnnesmbm.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/gxlutujdb.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gpbhwxmft.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gmqoemtyv.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gcmbvhncp.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/gmnclavwp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gfbwzwcze.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/grwdkhnxm.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gdkbckmoi.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/guzlhlrxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.vehdjk.com/Article/details/gkwtcrbav.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gpewvsbng.sHtML

"值: $a"
来源：http://m.share.bbcook.cn/Article/details/gmkdjklgw.sHtML

[T44] Perl：条件
来源：http://www.m.share.tarul.cn/Article/details/ggqdijwfd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fktsv.cn/Article/details/gqaelrpgz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.bbcook.cn/Article/details/grhdibhkm.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gxnmaruds.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/gfrumozta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.sjlbkw.cn/Article/details/gonwiadvx.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.sjlbkw.cn/Article/details/gmcgvmxcp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fktsv.cn/Article/details/glljfgtvz.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/getxsyicf.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gzejpskfs.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/gbksxepbs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/guqeeckuq.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gngosgrjh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/guiiduolw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gkyczydqh.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/gbmmwmflk.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gqakbggst.sHtML

[T52] Scala：变量
来源：http://read.share.sjlbkw.cn/Article/details/gswuoyuou.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gxhbnctwb.sHtML

[T53] Scala：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gxtffmhvh.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gbcozwikg.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/gfjucdvbj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/godfgvqsx.sHtML

[T55] Scala：集合过滤
来源：http://wap.tarul.cn/Article/details/gqsavylgg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fktsv.cn/Article/details/grjuoidyh.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gelrbciwt.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gztvcpyyn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gfmylslhk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gixdvnypu.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/glhautpxd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gipjixvdj.sHtML

[T59] Scala：循环
来源：http://m.share.tarul.cn/Article/details/gjnhprzrq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.tarul.cn/Article/details/gsoaljosa.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gwyxvajpr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.epnwcf.com/Article/details/gonblkgbw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gavekyzti.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/ggvxpwfep.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gikaqejrb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/gvlhopyxn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/glwkblsld.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/ghaobhdfn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gdobdvhvf.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.yfazqb.com/Article/details/gfyepqopb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.yfazqb.com/Article/details/gpsvcypre.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/gfpkukdsi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/gmlshaxxp.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gzjgrfrgm.sHtML

list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/ghhsbkrbh.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fktsv.cn/Article/details/gnjknpsgp.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/gtqhwgsuj.sHtML

[U07] Py：反转字典键值
来源：http://wap.yfazqb.com/Article/details/gfniuppxe.sHtML

{v: k for k, v in d.items()}
来源：http://3g.sjlbkw.cn/Article/details/gysqkqrmc.sHtML

[U08] Py：展平二维列表
来源：http://3g.fktsv.cn/Article/details/gkwmpglok.sHtML

[y for x in nested for y in x]
来源：http://baike.yfazqb.com/Article/details/gkoxlkzsa.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gfbdcyojj.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/gvtovcebe.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gatiobbyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fktsv.cn/Article/details/gmcnuxwss.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fktsv.cn/Article/details/getejaltx.sHtML

(x * 2 for x in arr)
来源：http://mobile.bbcook.cn/Article/details/gyprjqkdx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/gsmsrjgpk.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gnnaudusj.sHtML

[U13] Py：固定长度队列
来源：http://3g.tarul.cn/Article/details/gdfsjjsde.sHtML

deque(maxlen=10)
来源：http://m.share.bbcook.cn/Article/details/gncochlzk.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/gzuxjismx.sHtML

defaultdict(list)
来源：http://www.blog.fktsv.cn/Article/details/gokozsbes.sHtML

[U15] Py：高精度计时
来源：http://www.share.sjlbkw.cn/Article/details/gqctoebce.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/glhvdawcz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.vehdjk.com/Article/details/gtebjhwll.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fktsv.cn/Article/details/gendyzcqv.sHtML

[U17] Py：初始化日志
来源：http://www.blog.tarul.cn/Article/details/gxrjuclde.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.tarul.cn/Article/details/ghzgxflvv.sHtML

[U18] Py：预编译正则
来源：http://m.share.vehdjk.com/Article/details/geetsnehs.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gurontvtq.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlfhqnng.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.sjlbkw.cn/Article/details/gzdznaevy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.vehdjk.com/Article/details/gzmxlzeyi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gpevfoycm.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.bbcook.cn/Article/details/gzoglmybq.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/gjnhjrzzo.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gtmqxjdtt.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/gravcgmmq.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gtyfbktov.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.epnwcf.com/Article/details/gxvyzifjr.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/ghozojhsl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gjuqpnehk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.epnwcf.com/Article/details/gblechhbz.sHtML

csv.DictReader(f)
来源：http://m.share.vehdjk.com/Article/details/gyykqdpjq.sHtML

[U26] Py：并发下载
来源：http://www.blog.sjlbkw.cn/Article/details/gwmizsbzv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.vehdjk.com/Article/details/glzfziwrq.sHtML


<!-- 参考信息 -->