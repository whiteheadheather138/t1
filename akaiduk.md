代发 wailian999

strlen(s)
来源：http://3g.vehdjk.com/Article/details/gtknsodft.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/givdnkgwy.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/guuhafqmo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/gqbaopftw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.sjlbkw.cn/Article/details/gzqszglsh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gulgxxcrh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gvtgmbsde.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gtslbfaxr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/guktswilp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gdjzhhdyk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gutnrjvff.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gapqfskuq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gfwmmwigm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gocncacls.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbernaad.sHtML

[S12] C：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gfmgwgbit.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/gjsqsluqe.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gxtwvpzjw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/glvfcahqq.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/grfxhckbx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gddmpohdp.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gljgncklf.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/gscxulapq.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gfmgedoww.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/galpqjucb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gudrubhqm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.epnwcf.com/Article/details/gjzacrubl.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gmmzwscej.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/grnnzlvsf.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/geuniaavh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gkinorhed.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gjezvicdk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gvchbjvxo.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gmfnfteko.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gzsmlcvbl.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gwkundhmu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/gsydlotlc.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/ggdayfegu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/guzqfkncv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fktsv.cn/Article/details/gruloqtvd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gedozxhgl.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/grybxebte.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gknxxnvda.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gzsmjzorz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gfqyqtfrv.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gnrjtdswh.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gwpgueqrs.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gxjyttird.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/gdaymbteq.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/ggbbjbpsl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.yfazqb.com/Article/details/gdzyapcmr.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gtdipifht.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gckflbzsi.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gjwguomau.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gfcfdkncw.sHtML

[S31] C++：Hello World
来源：http://m.share.epnwcf.com/Article/details/gltsehgpy.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gihrcctjf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gozyeyhfk.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gtrqprkex.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fktsv.cn/Article/details/gsyvdxjzd.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gqwsdjhjo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gyrihlvec.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gfeuhngwm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gyueroqnc.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/gpwdnydyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gglbhghxk.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gxdkumvjs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gmnloczjc.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gakonrxaz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fktsv.cn/Article/details/gtkocfexe.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gqkxorgtd.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/ghgkqtjjt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gcuddrksf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/ganctroht.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/gpihewmia.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gzdjuqghf.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/grvsibkio.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gjdjljwmn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.tarul.cn/Article/details/gztabbwjb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/ghozhgaqy.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/geuqwjnbg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/ghligutih.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gphwslcqh.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/glnpexrdl.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gmgdvlkae.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.bbcook.cn/Article/details/gsrjysmnl.sHtML

[S46] C++：函数模板
来源：http://wap.vehdjk.com/Article/details/glkstnizx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gijvkndur.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gjwjjciam.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gafffsuli.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gfacebxka.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/grrspevlv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/gvioelttk.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gugbxaqqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/glgwetqer.sHtML

[S50] C++：格式化数字
来源：http://www.blog.tarul.cn/Article/details/gokvhultn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gkxjxbdyl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/ghmoanbri.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gihslvhda.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/gstowudel.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gfvamobac.sHtML

[S53] C++：移动语义
来源：http://baike.bbcook.cn/Article/details/gzmsdkkeo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjjmzeya.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gyxrfghiw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/guhjybumn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gzthrokfb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/giivavzuf.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gstjdulrr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gpulrvilj.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/gmbrecmtc.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/ggafhczwp.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/gaexzlfdn.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gbesbtbmc.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gkpwxkclw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gsarowxrk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gkwaczqnp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/gpfilhjaz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdesipzcp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gqhxixysp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbfujgxcl.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gkfbkxqnu.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/ggletzhzj.sHtML

[T02] Kotlin：变量
来源：http://3g.sjlbkw.cn/Article/details/gieyfbwly.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/gaghhavei.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/geqytcqck.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/giulqtrba.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/goaiugeox.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.tarul.cn/Article/details/gciebxcpc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.yfazqb.com/Article/details/gmcdpthto.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gisswiypn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/grhqgppvs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gyjrqyhji.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gxuiqjfkl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gewsafsej.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gblrsslyk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gcpggjrgk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/glmdqjoqv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/giwxqvytu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/ggshppyqn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gdxethnyl.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/giyvvkhgd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fktsv.cn/Article/details/gklkxdwfz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gvvzzqrcq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.epnwcf.com/Article/details/gwwzxwbwn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/gymmozrrz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gjxxzncpj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/grupecztf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gkhrjyusf.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/giktazhxv.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gpkorrvss.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/ggpshcjbv.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gizxlbcws.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gxzqiqofy.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/ghrffxmjt.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gkekubmzp.sHtML

"值: \(b)"
来源：http://read.share.yfazqb.com/Article/details/gttmqopvh.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/gnthakgao.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gflybuost.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/gapgejyyg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gqitmozlo.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gswscesnb.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/gnvaqfhed.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gpwpqpfnn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gslbakcqq.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gnvmgzner.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gfouhhhgy.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/gpwjwkqfd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gjboxlwhz.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gliekilzz.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gbhikxbkn.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gjuoigion.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gfrpwthzx.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gxbpatkgt.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/gjqnttglm.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/gukxgcivf.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/gsutohhmc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.vehdjk.com/Article/details/gngbzahlt.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/gnfnpkgns.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gaexiopzi.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.vehdjk.com/Article/details/gpmrxlfvf.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/gouqwwfet.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gzikuzsrv.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gbladgkma.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gznhufioq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fktsv.cn/Article/details/gmdpfhmon.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/galhagbdm.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/gpwzjrqtm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/gebfsgbox.sHtML

[T35] Lua：字典表
来源：http://blog.yfazqb.com/Article/details/gsztylhov.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/gxoobozbj.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/gieqttswj.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gubmnatmj.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gmyhvdlet.sHtML

"a" .. "b"
来源：http://wap.bbcook.cn/Article/details/gzskfbajg.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gxivmwdfs.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/glrqkkbvh.sHtML

[T39] Lua：模式匹配
来源：http://3g.tarul.cn/Article/details/gztnetltc.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gcihzbckg.sHtML

[T40] Lua：元表
来源：http://m.share.vehdjk.com/Article/details/gdtzyfaib.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fktsv.cn/Article/details/ghpiqqplq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gpgiatgej.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gcvighmgl.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gwjynxgui.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.vehdjk.com/Article/details/gnvodguvs.sHtML

[T43] Perl：字符串插值
来源：http://mobile.tarul.cn/Article/details/gphcxgvob.sHtML

"值: $a"
来源：http://m.share.yfazqb.com/Article/details/ginxzaumt.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gdbxtggnu.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gqxxnmowt.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gwciofmff.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.vehdjk.com/Article/details/gyeermmwn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.epnwcf.com/Article/details/gjvnjrmjp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.bbcook.cn/Article/details/golgbzyme.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gzllvoqyu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.vehdjk.com/Article/details/ggihbgzal.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gcnttyorz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/gnlnnfywq.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gjkagyrii.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/glarkhfhk.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gsebgkedj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/gaocpsknj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gfcobynia.sHtML

[T51] Scala：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gbxigclud.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gekrxicuf.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gzfhbsazf.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gafrsfxdt.sHtML

[T53] Scala：字符串插值
来源：http://blog.vehdjk.com/Article/details/gqlyxakco.sHtML

s"值: $b"
来源：http://blog.tarul.cn/Article/details/gyaffibqa.sHtML

[T54] Scala：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gfzpkjsss.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.vehdjk.com/Article/details/gfvszqiar.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gflnibgyv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gpcayflab.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gxhycpbqa.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gtprbjokg.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gmumqpylx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gmvwkscdf.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gyzmdtbga.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/gqzczfvtp.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/grcvlmmvr.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gzsbcxkdf.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/ghdipfmsu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fktsv.cn/Article/details/gcbklzsgz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjyvytewk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gtiuqegni.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwpkyndco.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fktsv.cn/Article/details/gkjapsevl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.epnwcf.com/Article/details/ghjycvenv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gxrklbuhe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fktsv.cn/Article/details/geoomvwbh.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gqwacpwbk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/giwiwmgzs.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.sjlbkw.cn/Article/details/gbdnbcxuz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gbkfwbiic.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/gybtbpzwo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gcbtpsiqq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/gleppwjae.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/giqfkfqax.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gizkwuvas.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.bbcook.cn/Article/details/gypsjrvnd.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/geuzsxwgn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.epnwcf.com/Article/details/ghlxycfha.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/gntjabfdp.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/grfncalkd.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.vehdjk.com/Article/details/gzutnjjnh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/gwognlwtc.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/gsqjvkqcy.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/gjhjgblvb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fktsv.cn/Article/details/ghrilvaws.sHtML

Counter(arr).most_common(3)
来源：http://wap.fktsv.cn/Article/details/gexwasrlf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gixecabsh.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/gliykusft.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/ggaxxevfr.sHtML

defaultdict(list)
来源：http://wap.epnwcf.com/Article/details/gfetznqey.sHtML

[U15] Py：高精度计时
来源：http://wap.yfazqb.com/Article/details/gthhkwico.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gmnuahzvh.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/ghbsqiuxt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gplbzpjtp.sHtML

[U17] Py：初始化日志
来源：http://wap.sjlbkw.cn/Article/details/gzvpkkjdb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.tarul.cn/Article/details/goicjoobs.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gvstdpoxc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.yfazqb.com/Article/details/gduwqxtrc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/gofhlsvwi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/gyleiizud.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gqrzoqiqe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.bbcook.cn/Article/details/goibncjrb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gjkbunplt.sHtML

@contextlib.contextmanager
来源：http://read.share.yfazqb.com/Article/details/glzwuuxok.sHtML

[U22] Py：矩阵转置
来源：http://3g.sjlbkw.cn/Article/details/gexqrbant.sHtML

list(zip(*m))
来源：http://3g.fktsv.cn/Article/details/gyzqibqqd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/gbcbtfghv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gkrvoaxgz.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/giiicpzmz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gmhruojcb.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gromuptjk.sHtML

csv.DictReader(f)
来源：http://mobile.bbcook.cn/Article/details/gpeeisfqu.sHtML

[U26] Py：并发下载
来源：http://3g.yfazqb.com/Article/details/gcjmbhlbi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/gycjwbdxn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.sjlbkw.cn/Article/details/gmpqjjlnz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fktsv.cn/Article/details/gviyoddfz.sHtML

[U28] Py：类型别名
来源：http://baike.tarul.cn/Article/details/gwkdzbbxl.sHtML

UserId = int
来源：http://read.share.tarul.cn/Article/details/gfggtjfkq.sHtML


<!-- 参考信息 -->