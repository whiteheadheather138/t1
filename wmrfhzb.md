代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/gzdvixhcm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/giyjmcjtz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gorstxepm.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gmbypltnu.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gfddostas.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gxgcqizqj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.epnwcf.com/Article/details/gzhapitwk.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gydrqjmnh.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gghbbbren.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/geudeljkh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.epnwcf.com/Article/details/gvpbpjwco.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/gdjuqeaeo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/geiezfhmm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gtowsqwgn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gprwtulih.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gcibctgro.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/gbfdxswvv.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/giypqjmvt.sHtML

int *p = &a;  *p = 5;
来源：http://blog.yfazqb.com/Article/details/gorictnwo.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/glviexyjj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/goakpfhai.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/ghzbcdisq.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gvldrdmap.sHtML

[S12] C：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gdokguqex.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/gbraevrqj.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gbkcrpsvf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/glhfjqgsa.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gkuaqvegf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/ghtkxrufa.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/ghsazsdkf.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gogywurhe.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gtbctriao.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gbmlxzbvt.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gmkqkncka.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gvpdumwjp.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/gqkchuanu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.vehdjk.com/Article/details/gsklwaobi.sHtML

[S19] C：快速排序
来源：http://mobile.fktsv.cn/Article/details/gqplrqskb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/guwxyzvhz.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/grhfkyvrx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/ghfwraajd.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/glhuwofjo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gnjlahloz.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gjuqgyqax.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/gifbxrdry.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/gyuflpgye.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gldgkxmfg.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gdfjpmhwe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gkmhjtoyj.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gfzeuqdgj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/gboapcasj.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gdbciwwje.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gexoijion.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/ggdxxgyur.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/guuwydpmf.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gglabnbqy.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gjaecxvkv.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/gjlpyxehw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gggxeqkjz.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gpfukfhdv.sHtML

#ifndef X_H
来源：http://m.share.yfazqb.com/Article/details/gsavykhfs.sHtML

#define X_H
来源：http://3g.tarul.cn/Article/details/gqskxydtj.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/gkaljperi.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/gtqbujmkv.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/grdskbkwo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gpvrktgxm.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/gcflpytju.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/ggzrafllp.sHtML

[S33] C++：vector 增删
来源：http://www.share.epnwcf.com/Article/details/gsfbunrhv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gnfwpcoiz.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gjpwfmwcm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gfdalcfms.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gklrhqqxc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/goeoafxwm.sHtML

[S36] C++：unordered_map
来源：http://m.share.tarul.cn/Article/details/gfyoggryn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gcfdbavag.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gfvggxwnt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gykypngmq.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/gswckjzlf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gjzmwisec.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gkozqaixn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gqmzxsdrj.sHtML

[S40] C++：查找元素
来源：http://baike.vehdjk.com/Article/details/gyppbadoy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gxpnysoqg.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gggphknct.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gnnbfohri.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gwtzqecll.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.epnwcf.com/Article/details/ghjnaiupq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gjcqzwvto.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gnfwfbjke.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/grjwypgqz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/guvyvdlqa.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gdiauvnrx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gfzocwybm.sHtML

[S46] C++：函数模板
来源：http://www.share.bbcook.cn/Article/details/gafkydxgn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gukiumche.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gvfmgxueh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/guhezybqa.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gdmpkyefx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/gpwkmudoo.sHtML

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/ghrxabupy.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gmcsbbxie.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/grqtsqigr.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/geqrwazmi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gtxskaiof.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gcwzcybnc.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gbkrmooan.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/gzfoxgexy.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/gczalqzpd.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gozflbzln.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/gjurtmrqh.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/grhxrvyrq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gucppevxa.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gyzkopkpo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.bbcook.cn/Article/details/gglsxvnkn.sHtML

[S56] C++：optional
来源：http://mobile.fktsv.cn/Article/details/gyzpbnbmm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/grbqbquyc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gxmwkjufr.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/ghwbjftiu.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gcfqrurlg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gwgihpbcq.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/ggmcizoqy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/gknsnmims.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gkxnobvux.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gswrdqbvy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqnmfwwua.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/ggetmaavg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gichwnzsa.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glzozzadw.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gbijkbcof.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/gqveusoji.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gsekfjeja.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.vehdjk.com/Article/details/glpvdlrcs.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gbiukznwr.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/gxodpfgnu.sHtML

val n: String? = null;  n?.length
来源：http://baike.epnwcf.com/Article/details/gnuhqkiwj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gucyztvki.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gmltrciwr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.yfazqb.com/Article/details/gzmhjqdgd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/gcdjzbzir.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gyvwitnbd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/ghikjmiym.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/grnytkway.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/grhnifhgh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/ghgqipzoh.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gjogeaipk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/glohyvnhc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gyluntxtm.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/gdqnfmhpb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gaoqohhfh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/gcowejhvo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gtxndjlof.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.vehdjk.com/Article/details/gwcfexzzn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.vehdjk.com/Article/details/ggbakudjg.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/ggtzuaere.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gnluuxewg.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gnylfzwxp.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.bbcook.cn/Article/details/gumpzuwrb.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/gscloible.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gvwyblawn.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gbnpxoalf.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gmunjkgxe.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gyojfwqtx.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/ggouqbdst.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gdpkwzbal.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gkjnfmgxe.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gqufexola.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gzamztxya.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gdbqoovnk.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/gieshrjzy.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gboyqbnns.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/gwexgjnql.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gwvarppvj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.bbcook.cn/Article/details/gcuqyospb.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/gfgtpqdcl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gsewqwzcd.sHtML

[T25] Swift：结构体
来源：http://www.share.epnwcf.com/Article/details/giudqkaft.sHtML

struct P { var x: Int }
来源：http://www.blog.yfazqb.com/Article/details/gfluqzvks.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gvhilukeb.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gklraaujq.sHtML

[T27] Swift：错误处理
来源：http://read.share.sjlbkw.cn/Article/details/guuwdynim.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gidiegvql.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gnqbuulsk.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/giskpllpt.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.yfazqb.com/Article/details/gvsoaechp.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gfnuojhus.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gdcbyhfxe.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gyxalxobe.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/gwfhnzjpv.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gonifaumy.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkrpzztz.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gcybitrat.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/gspapnynm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gjitzoaxz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gyocipwpp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.tarul.cn/Article/details/goqmwqlfk.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gwdublada.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gktqfxlwi.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gdxqshoub.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gnieascbq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gilbkstna.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gtwubhalr.sHtML

[T38] Lua：条件
来源：http://3g.vehdjk.com/Article/details/gzrfjlcgm.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gtwlfyjpm.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gttuzeyei.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gcahnxhah.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/gazwsvgcy.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.vehdjk.com/Article/details/gbxgjmdqs.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gdhisxozg.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/gadzskwjw.sHtML

[T42] Perl：变量类型
来源：http://baike.epnwcf.com/Article/details/ghkkxxejl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/gvzknarvy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fktsv.cn/Article/details/gqloryqfs.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gwjmmzyty.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/ghehztobc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gepbjxihg.sHtML

[T45] Perl：数组遍历
来源：http://mobile.vehdjk.com/Article/details/gevtloyco.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gabqkehxa.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/grpgfylnc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gqcmnraox.sHtML

[T47] Perl：正则捕获
来源：http://wap.fktsv.cn/Article/details/gvlooodqy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gafskanhg.sHtML

[T48] Perl：正则替换
来源：http://baike.fktsv.cn/Article/details/ggeciydja.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/gteyaaxpy.sHtML

[T49] Perl：函数
来源：http://3g.tarul.cn/Article/details/gmyzmclaa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gbbcjldpi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gvmkoggir.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.vehdjk.com/Article/details/ggdewuupf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/gvooupqby.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gsquilnoq.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gipomlnwy.sHtML

[T52] Scala：变量
来源：http://blog.yfazqb.com/Article/details/gwpablhgw.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/gmljaidir.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gqoirgoxv.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gwhzpklst.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gqccnxgdc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gbswaubwq.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/gubmydugx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.tarul.cn/Article/details/gxveebdyz.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gkkkzbhia.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/geasmzhim.sHtML

[T57] Scala：模式匹配
来源：http://3g.vehdjk.com/Article/details/gwdryuopr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.yfazqb.com/Article/details/gioozkwvd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/ggaduizdy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fktsv.cn/Article/details/ghcbisowp.sHtML

[T59] Scala：循环
来源：http://wap.vehdjk.com/Article/details/gfwsqjuml.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gxditmjni.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gjernnobw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.yfazqb.com/Article/details/glyhfdege.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gknpzfqms.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.epnwcf.com/Article/details/gqmujbhpv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsvilxcrn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/gmhqauyoo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/gfyjaagmb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.tarul.cn/Article/details/gsmhceedo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gjxitwcyn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/garafpklu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/geknfrvpq.sHtML

[U04] Py：变量调试打印
来源：http://mobile.epnwcf.com/Article/details/gphztelek.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.bbcook.cn/Article/details/gdadglgwe.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.yfazqb.com/Article/details/gdbtgcxtt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gqekkwubv.sHtML

[U06] Py：合并两个字典
来源：http://baike.sjlbkw.cn/Article/details/gmxrhieql.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/gkdgburfm.sHtML

[U07] Py：反转字典键值
来源：http://wap.sjlbkw.cn/Article/details/gcromvbtn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.vehdjk.com/Article/details/gjbyzfkvv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gxcqmyolh.sHtML

[y for x in nested for y in x]
来源：http://read.share.epnwcf.com/Article/details/gokhygzne.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fktsv.cn/Article/details/gfxnhtnrc.sHtML

max(d, key=d.get)
来源：http://read.share.epnwcf.com/Article/details/goszauair.sHtML

[U10] Py：按值排序字典
来源：http://blog.sjlbkw.cn/Article/details/gfyleevqt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.epnwcf.com/Article/details/gnmgfoplp.sHtML

[U11] Py：生成器表达式
来源：http://3g.yfazqb.com/Article/details/gsxfeddef.sHtML

(x * 2 for x in arr)
来源：http://blog.fktsv.cn/Article/details/gatxikdve.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gqvoejrtz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/gvjhntixw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gbnyubpgw.sHtML

deque(maxlen=10)
来源：http://www.share.sjlbkw.cn/Article/details/gpmdbomyt.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/gxfrhfnlg.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gannepkkr.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/gyroajusa.sHtML

t = time.perf_counter()
来源：http://mobile.vehdjk.com/Article/details/gpknncjra.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/gvnnftioz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.tarul.cn/Article/details/gidupjxyp.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gabmubfjt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gomfctxji.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/gmbbdqnwg.sHtML

pat = re.compile(r"\d+")
来源：http://baike.vehdjk.com/Article/details/gugpupuiq.sHtML

[U19] Py：正则替换带回调
来源：http://wap.yfazqb.com/Article/details/gavhsfxsm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.epnwcf.com/Article/details/gaeoixoiz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/gmotxhkyl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.vehdjk.com/Article/details/ggxjxtxvn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.bbcook.cn/Article/details/goeotyvit.sHtML

@contextlib.contextmanager
来源：http://blog.yfazqb.com/Article/details/gvlyatatd.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.epnwcf.com/Article/details/gwgahgnfv.sHtML

list(zip(*m))
来源：http://3g.fktsv.cn/Article/details/gbifkfpnt.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/guqgkxqow.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.sjlbkw.cn/Article/details/ggrziejxh.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/gkopjtsxo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gfgixjdyu.sHtML


<!-- 参考信息 -->