代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gwogcdjcs.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gigcylnui.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/ggnkmnkuc.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gjmqznvbo.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/gegdjjxzh.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gzkuhcssl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gmhlpdaru.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gjbjniuiv.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gswimzeyp.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gmelzxzmt.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/goyztpptj.sHtML

[S07] C：数组遍历求和
来源：http://blog.bbcook.cn/Article/details/ghylsnnxv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gnsehgbwk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/ghciopjmn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/glcvizvjk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/ginhzjdmp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gmljegtjb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/grnswhokt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/gtqfofvvf.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gfksypvcf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.epnwcf.com/Article/details/gseiaxwzq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gxsogknxc.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gxuoztnqk.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/gtqnmzmzs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gbflxdxty.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/giljcjaki.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fktsv.cn/Article/details/glynoenpc.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gtkheufqv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/gfbqobsgq.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/ghdnarjuj.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gtyebulnp.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gngckxigo.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/grwxfhbrs.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/gtuhacfio.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/ggypuhmjr.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gobddordx.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gbgoltjqs.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/guzaanqsl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gnmmplnmb.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gbpbhtgxr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gldarzqqn.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gqayrjwhu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/gkezmyqiq.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gnkhyzlyi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gfcawdxoc.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gdbeqhjqp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gupozkbyz.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gmokywenh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/guwjijfjd.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gndmucpxh.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gdzuymqjs.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gjpljlxlf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gofuhojpn.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/grtnuucid.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gctlkijqd.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/ghenwihts.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gnvaawezp.sHtML

[S29] C：变参函数
来源：http://3g.vehdjk.com/Article/details/gffhrpqpn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gjaktshel.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gwloqsckw.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gdudqnwwb.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gjupqewhw.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gkzpfshvm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/grelbbsqm.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gsaetiunv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/grarorwge.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gyhmcpunl.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gvtngmahv.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gouzuefct.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/geqhohuog.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/gmsusmrcn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gtewsmdrz.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gvwrtzify.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gwmvbhxzt.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gzcaweegb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/goqatpeig.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gjxzjpipp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/gjggumdcn.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gngoaeimg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gdquhpcph.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gvheugutu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/grzxoddgr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gmwhiejch.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gewlbhvsy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gxiwufogn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/gbaltkzxf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.vehdjk.com/Article/details/gpqqeyfqs.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gsfpyigau.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/geaazbpud.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/gqpewaley.sHtML

[S44] C++：引用传参
来源：http://wap.sjlbkw.cn/Article/details/gwoozuzqc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/gwnabuvzn.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gvjygajdu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gogqxkgfz.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gxriguasf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/ghxftaufh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gvkalngkd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.yfazqb.com/Article/details/gqszqozyo.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gqrrxpotl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/glyyptrmf.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gsdqxrvid.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gigqyrjpy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gmoshjdyp.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/glrlpgiqd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/gokoavmfl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/glqwxizfx.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/ggiexcdxy.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gsjgeyfqi.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/grxhwzkcy.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gqsejpcen.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gusjpgetu.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/givmdawqa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gejdutmap.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gccbrpiuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gerstuhnm.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gzfihktgz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdqwxaxq.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gizcytddz.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gyysxpnft.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gxsakmdrt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gzbdnrmws.sHtML

[S59] C++：静态断言
来源：http://wap.fktsv.cn/Article/details/gwtvnngqf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gupiueeaf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gccwxvcyb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.vehdjk.com/Article/details/gnabtbssb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjddmokpa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gllpsdlva.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwvpbsgwq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/ggdycxjlr.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/glvktoeqy.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/gpxsrnrax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/gpkeatfva.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/geqpuhoan.sHtML

"值: $b"
来源：http://mobile.yfazqb.com/Article/details/gomdsulja.sHtML

[T04] Kotlin：空安全
来源：http://read.share.sjlbkw.cn/Article/details/gsmjlmasd.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/ghvrngpmg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gwbwezbjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/glvsowkyo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/ghgsyhlbm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gwumghxgx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gfzbxwyfa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gegvwjgyh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/gbwawcrov.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gytogyzqg.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gwufhkhqp.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/glrvniezl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gbtehtiru.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.sjlbkw.cn/Article/details/gbcfcjfxe.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gmktbrbwl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.yfazqb.com/Article/details/gvamuyqoo.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.bbcook.cn/Article/details/gzhofbddl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/goqjyyifl.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gveoigods.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gzauyxiea.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gvtvacyfz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gxvvhyhzo.sHtML

[T15] Kotlin：接口
来源：http://mobile.tarul.cn/Article/details/gwmemhxwh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.bbcook.cn/Article/details/gsqbqhrkw.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/gygcytbfg.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gzeawxczz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gblqmbfar.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gsqxqmeye.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gmgpjqayj.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/gmuenoaxi.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gisjvoicu.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/gwxpcgyyb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gdrfduofl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.sjlbkw.cn/Article/details/gyuyoxsog.sHtML

[T21] Swift：遍历
来源：http://www.blog.fktsv.cn/Article/details/gkgyrxtiq.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/gvxanpzij.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gsvptdrgh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.bbcook.cn/Article/details/gptkpwxws.sHtML

[T23] Swift：函数
来源：http://www.blog.epnwcf.com/Article/details/gtdwxoudd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gwiroxuzx.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gkbvsdrvm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gyetphbjb.sHtML

[T25] Swift：结构体
来源：http://baike.sjlbkw.cn/Article/details/groocawnw.sHtML

struct P { var x: Int }
来源：http://wap.fktsv.cn/Article/details/gbqkkvdea.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gsivmdmaz.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gherayide.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gnfwmitnb.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.epnwcf.com/Article/details/gwktyiwvs.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/geswhuefp.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/gptybvglz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/gqjzzndjv.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gwwbjzpgt.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gfqoknwtc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.vehdjk.com/Article/details/gcgpqnaxv.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/gnxcxcakb.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gugppeblu.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/ghnhoamtn.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/gxefcfgih.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/gdrwmntzu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gqqxspqfm.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gjetkpyio.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.vehdjk.com/Article/details/gqpkmdsxv.sHtML

[T35] Lua：字典表
来源：http://blog.yfazqb.com/Article/details/glnpvccah.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gwafnrxae.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gczgyndrh.sHtML

function add(a, b) return a + b end
来源：http://m.share.fktsv.cn/Article/details/guuxcfnjh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/goysynmau.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gdwwyiovf.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gzwpojnqu.sHtML

if x > 0 then print("正") end
来源：http://www.share.vehdjk.com/Article/details/gmzeinohb.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gqjtzugrq.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/gzbopapgd.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/ggxotdirv.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.sjlbkw.cn/Article/details/gibgrmson.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/gynspbssc.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gsmhvkvbx.sHtML

[T42] Perl：变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gccacvotq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gmpxyhbbj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/ggwccpwxd.sHtML

"值: $a"
来源：http://wap.tarul.cn/Article/details/gkpayhgdm.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/geobbnsxj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqeclhhsi.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/ghnzjvwpe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gtkmcrxzu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/gemgikpnq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gdeverpct.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/gwpiahaaj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.tarul.cn/Article/details/gejbcvrlc.sHtML

[T48] Perl：正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gqaglueei.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gxjwoecix.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gqajuvthx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gtnuswvwf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gwezeohrn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/gilpgaoyo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/gtbdflnok.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/grmggtmkm.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gfmlfqrgm.sHtML

[T52] Scala：变量
来源：http://baike.tarul.cn/Article/details/gfjtsvbbr.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gsovnifom.sHtML

[T53] Scala：字符串插值
来源：http://3g.tarul.cn/Article/details/ggxwsqiks.sHtML

s"值: $b"
来源：http://baike.fktsv.cn/Article/details/glltdpuyo.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gxuzvqwbo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gbgdviojj.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/gjnpagkid.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/gipyfxkzj.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gijendwpg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gghoekluv.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gwjzmqkft.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gobtjgwcw.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gstqilgan.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gpzkpzfrr.sHtML

[T59] Scala：循环
来源：http://baike.sjlbkw.cn/Article/details/gqvddidjx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/ggkuudhto.sHtML

[T60] Scala：折叠
来源：http://mobile.fktsv.cn/Article/details/gilflvpzl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gpllmsrte.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxptpposn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gxathnezb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gblrlsivw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/grkxsgqnr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.tarul.cn/Article/details/ghgaypocp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gnvdspkvn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/gimwqrhmp.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gkvcgabxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gkyevwrtm.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gmdpezxhw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.epnwcf.com/Article/details/gvxdzedza.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/gzmmnonci.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gwmbcouth.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gtcvwauuv.sHtML

{**a, **b}
来源：http://www.m.share.vehdjk.com/Article/details/gxpjigoml.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/gabziacwb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/glzwnoomt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gswvmagie.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gjconhpot.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gmjqvfnnf.sHtML

max(d, key=d.get)
来源：http://3g.tarul.cn/Article/details/gumrlzlqk.sHtML

[U10] Py：按值排序字典
来源：http://wap.fktsv.cn/Article/details/ghhmplett.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/guxirfdxe.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/grrkveyhh.sHtML

(x * 2 for x in arr)
来源：http://read.share.fktsv.cn/Article/details/gcduvshaf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gydcnhbgi.sHtML

Counter(arr).most_common(3)
来源：http://read.share.epnwcf.com/Article/details/ghondtkos.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/ghoqveoel.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/gpvxwcuga.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/geusituoy.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gbxhpsokk.sHtML

[U15] Py：高精度计时
来源：http://3g.tarul.cn/Article/details/guocamxcf.sHtML

t = time.perf_counter()
来源：http://read.share.sjlbkw.cn/Article/details/gcifuoqez.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gwuynqhxw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.yfazqb.com/Article/details/gfvduhfts.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fktsv.cn/Article/details/gfpdjawfu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gizzuqhni.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/gghvssxww.sHtML

pat = re.compile(r"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gzlntqugj.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gvpgfayzp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.bbcook.cn/Article/details/gqscjuhkq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gjbfyrxfu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gtqzkwfza.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.bbcook.cn/Article/details/gxsdcbcpy.sHtML

@contextlib.contextmanager
来源：http://read.share.vehdjk.com/Article/details/gruaqarwm.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.sjlbkw.cn/Article/details/gonrbqkxa.sHtML

list(zip(*m))
来源：http://www.blog.sjlbkw.cn/Article/details/gjauhquvw.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fktsv.cn/Article/details/gwwvdpunl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.sjlbkw.cn/Article/details/gbwiqlpua.sHtML

[U24] Py：路径操作
来源：http://3g.sjlbkw.cn/Article/details/goiyiebtp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gyotsayed.sHtML


<!-- 参考信息 -->