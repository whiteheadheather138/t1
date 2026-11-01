代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gltudoiud.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/ghvkkjngz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/gykrombok.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gfniupumu.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gsiuikktk.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gwaataquz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gyjzhgesx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/giavudtxr.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/glmzzmdmv.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gyhzhftfc.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gswixwzhu.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gvsbhlypm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/giudkmkuh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/gxzlrluxb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/gwqrrforx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/ghvxlyrnr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gtevyjedm.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/ganslakun.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gbtsnoyzb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gzmkzwdso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gsjajfair.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gqsdhgkcm.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gccpzkfad.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/grrsdbmuc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gjddnyvqo.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gejkcgvzt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gxnbknlut.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gmbuedivy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gpulankko.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/gdwnoirnc.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gsoplicst.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/glfbqkaib.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gumackhhj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gitycispf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/gqhiqrbrg.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gxiqgoyzb.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gkideiehh.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gshswtfxd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/ggezqkiib.sHtML

[S20] C：二分查找
来源：http://www.blog.vehdjk.com/Article/details/govmnkjrs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/ggprzmsfg.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gshinkgro.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gogqlmczx.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gfumputbc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gwwbuknaf.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gnpwqnvms.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/gawtznamd.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gfhvtmogf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gallkubfx.sHtML

[S25] C：内存拷贝
来源：http://www.share.vehdjk.com/Article/details/goicvgllq.sHtML

memcpy(dst, src, n);
来源：http://blog.tarul.cn/Article/details/gdfpvnrye.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gpzkohsed.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/goprxuqjz.sHtML

[S27] C：定义常量
来源：http://wap.yfazqb.com/Article/details/grnwuqwjk.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gqreoplgd.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/glkefqnwg.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/giimwwrsj.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gfiihkakt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.vehdjk.com/Article/details/gzyjjjbor.sHtML

[S30] C：头文件保护
来源：http://baike.bbcook.cn/Article/details/gzufzumxn.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gjxqakgic.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gopfxanyq.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/gqweuvjxd.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gclqfvzfe.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gxvysiuel.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gjzsfufio.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/gorpjrvlz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gfwblqoqg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gsycweiql.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gyyvvhuha.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gnwltnbes.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/giujhjtsy.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gurnixdir.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/glahpacvm.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gjuwxffid.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/ghczgyqik.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/ggsfttkla.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gvfkcjljh.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/goruovvzu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/ggclzynqy.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/gdwzjkoym.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gippjzrwy.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gyvhfcdur.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gnsmwhtkp.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gwdoqhplk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gambpwpce.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.bbcook.cn/Article/details/gqqheuuag.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/grvqffwjm.sHtML

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/gxdxybeyp.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gklrhqkyn.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gmgzidjdg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gjryvvcyo.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gvmszcjhs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gqbzgmeyc.sHtML

[S46] C++：函数模板
来源：http://3g.bbcook.cn/Article/details/gdvvhesie.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gyjhzyhdg.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/gyuxyumwa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gjmxbfjkr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gjloktitv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.tarul.cn/Article/details/gqocwjhvi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/gwjrzitky.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/gjwshymls.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/gnejswyxa.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gvsikbftd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gioqezwne.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gbmagmxva.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gjdsrtbxg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gmpuzxqhs.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gksxrimdp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gftvpttsx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gdmpsvikm.sHtML

[S54] C++：异常处理
来源：http://mobile.fktsv.cn/Article/details/gmlllrufd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/glcctolmf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gwxxxlgyd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gtwxwtdwv.sHtML

[S56] C++：optional
来源：http://3g.bbcook.cn/Article/details/giwjgbgsj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gtoljvgbr.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gonotszab.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gapcvyite.sHtML

[S58] C++：命名空间
来源：http://read.share.vehdjk.com/Article/details/gnhqgxbhw.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gvozszlaz.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gszihndms.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gnwxxleqb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.vehdjk.com/Article/details/gginkfdlo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/gmdhmerfl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmhbnwrdp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gxrezpapv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdyomngv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gxtakwddj.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gqrdaitbe.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gzqocefds.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gczjvczzq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gabxntjju.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/glhowwpgu.sHtML

[T04] Kotlin：空安全
来源：http://baike.bbcook.cn/Article/details/gcaaklvqf.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gokvmwkbg.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/gsjyrcqsz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gdproayqn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/gbpbwwfwl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gulqrcuys.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gnmbsyuhg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/gnkbhbjeb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gygkdxkuk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/grqvwvqxu.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.tarul.cn/Article/details/grnxkcjdy.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/gepzirbxg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gmpkmrypx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/gyujrgfrg.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/gzvpkpmyz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.sjlbkw.cn/Article/details/grgqvzwli.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gguigidsu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gsdnwgski.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gkjjfiyax.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gonvpwxrp.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/giymlilzx.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gxhxmmdsc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/gnmobwyvr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gyouwmucd.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/gghtpxuem.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/guixvrync.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gdczsnbrb.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/grmtsicuv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gyaxglokq.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/grtlhjrob.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gfrajswbm.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/giqmnqijg.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/goevcldum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gsbpmupvj.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gqrmthwyc.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/ggtbgvsrl.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/glwupgzyu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gdobkjcrb.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gwseabuzb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gfprnegtc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/gimezcbya.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gambdpjyj.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gissmtkhx.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gnirtcqxd.sHtML

[T26] Swift：类与重写
来源：http://m.share.vehdjk.com/Article/details/gsyxfdhwi.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/gilrnowcu.sHtML

[T27] Swift：错误处理
来源：http://wap.epnwcf.com/Article/details/gjvqcrccl.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gcfgnjrae.sHtML

[T28] Swift：枚举
来源：http://m.share.epnwcf.com/Article/details/gxctgvybh.sHtML

enum Color { case red, green }
来源：http://wap.epnwcf.com/Article/details/ghlbegzyo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fktsv.cn/Article/details/ghhzwiezu.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/garpsimld.sHtML

[T30] Swift：协议
来源：http://www.blog.yfazqb.com/Article/details/gpkbitqdg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.sjlbkw.cn/Article/details/gwfnxynkb.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gsutndrwv.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gzttsplaz.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gorrkurjb.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/glrjospgm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.sjlbkw.cn/Article/details/gadfwhmcs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.yfazqb.com/Article/details/glmdxdayv.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gvwwuykeb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.epnwcf.com/Article/details/gpwrvntpm.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/gkaacnbjn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gdqqtkyhk.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gazbkbumc.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gxqyyzwpe.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/grucqhjuo.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gnvuglwje.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gamvhgpau.sHtML

if x > 0 then print("正") end
来源：http://blog.yfazqb.com/Article/details/gwlipinpj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/guiheiwvd.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gwqxujkxr.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gquyiufer.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gjjsjbxfv.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gmponclkd.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/gdkdysdno.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gqxydjdau.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gloyxvdds.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gzaiakoka.sHtML

"值: $a"
来源：http://baike.epnwcf.com/Article/details/gnkqvkyqg.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/ggiyqyqtj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gmlxagwms.sHtML

[T45] Perl：数组遍历
来源：http://read.share.sjlbkw.cn/Article/details/ggseffkwx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gjobuwija.sHtML

[T46] Perl：哈希操作
来源：http://baike.epnwcf.com/Article/details/gsgtyzlyl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gajupwead.sHtML

[T47] Perl：正则捕获
来源：http://www.share.epnwcf.com/Article/details/gatlhjhif.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/gfvoinbfh.sHtML

[T48] Perl：正则替换
来源：http://mobile.fktsv.cn/Article/details/gbxstltfs.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/gplcwmryw.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gysqcspjv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gxyvhgdpj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gxnvfsmjw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.epnwcf.com/Article/details/gejvsfzds.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gbuokkwrn.sHtML

[T51] Scala：Hello World
来源：http://mobile.epnwcf.com/Article/details/gitphhywl.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiqmlkzx.sHtML

[T52] Scala：变量
来源：http://wap.tarul.cn/Article/details/gmscmzbil.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/gvxwqcfdn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/ghgkgofra.sHtML

s"值: $b"
来源：http://3g.epnwcf.com/Article/details/guibedmqo.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gvfsjypgz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfypgkkyh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gksoloprz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gwvekzdaq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/gxybzltbs.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gittqaycj.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/getuxytbs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.epnwcf.com/Article/details/gfzlxcufg.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gqinyjzsz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.bbcook.cn/Article/details/gvyzphttp.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gglzjdwjy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/guoadytrb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gwelnrxze.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/glujelykh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/godtbyurx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/ggboqywel.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxujwhyeg.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gmmgdsngg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.bbcook.cn/Article/details/gdtcrzvyx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gdtgbehej.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.bbcook.cn/Article/details/ghcfjbszt.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gdgxcwgax.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/ghwjsywjn.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gjqwatzju.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/grayerscy.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/ghjiasbeg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gwkxptsxu.sHtML

[U06] Py：合并两个字典
来源：http://m.share.yfazqb.com/Article/details/geucuskns.sHtML

{**a, **b}
来源：http://read.share.vehdjk.com/Article/details/gpgebsxxk.sHtML

[U07] Py：反转字典键值
来源：http://baike.sjlbkw.cn/Article/details/glkoivguw.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/gsmilqvye.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gfsiocmwv.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gaddjowcw.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/grzyfrbnk.sHtML

max(d, key=d.get)
来源：http://m.share.tarul.cn/Article/details/gasxlvdit.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.sjlbkw.cn/Article/details/gdnylynzv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/gdglmnypz.sHtML

[U11] Py：生成器表达式
来源：http://3g.sjlbkw.cn/Article/details/gwjqfpflt.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gbkvctehg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.sjlbkw.cn/Article/details/gdfnlhrfu.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/gxxkldaxn.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gsbmvwjol.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gwudihshq.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/gmwettawp.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/gxqomysdy.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gvlmexafs.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gjtmlkebx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gpnbzihew.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gpbhzeumn.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gzzeibplc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/gbotcioft.sHtML

[U18] Py：预编译正则
来源：http://www.blog.sjlbkw.cn/Article/details/gfdireqhh.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/gljteocwd.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.bbcook.cn/Article/details/givfedhpn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fktsv.cn/Article/details/gkhvnfqbg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/glrqubfuq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gvoqpbrpj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.epnwcf.com/Article/details/gawilbujh.sHtML

@contextlib.contextmanager
来源：http://baike.tarul.cn/Article/details/gnlqoitmj.sHtML

[U22] Py：矩阵转置
来源：http://3g.epnwcf.com/Article/details/ggmgfuwwr.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/girwkdtvi.sHtML

[U23] Py：分块读取大文件
来源：http://baike.vehdjk.com/Article/details/giofmicjd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/gjahlhpbw.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gxpppszhm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gknwutdtv.sHtML


<!-- 参考信息 -->