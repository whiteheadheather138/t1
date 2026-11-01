代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fktsv.cn/Article/details/gerkipdmi.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/grklmbxls.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/guphcccfp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gbkgrgite.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gkqukqbom.sHtML

[S10] C：指针与解引用
来源：http://www.blog.bbcook.cn/Article/details/gmopimvlc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/ganewrzrq.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gwjpddqho.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gvueheufi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gywmsbveb.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gstwlopjj.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/guqbgtzho.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gepppxpzc.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gwqfjpwbt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gsxfcyblo.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/grjpjyruk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/grcepotvx.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/gtuoemxwa.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/gfjfprfya.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gdapypasm.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/grderijyw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gkyftjgvt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/gmytunblx.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gvtdrcrvd.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/ghqurjdqx.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gtpmontna.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gfzrxrxgf.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gqwksqaph.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/ghfwkexqg.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gdfhvikmv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/grmzvegww.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/grrhkjyft.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/grrivikaa.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gxlwspgsi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gywauorhq.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/gohsmlteq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/ghsovyejv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gaszrdjrc.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/getxapper.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gjslreqkl.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gtvfvfzid.sHtML

[S27] C：定义常量
来源：http://www.share.tarul.cn/Article/details/gsgjlmeoz.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gergpuina.sHtML

[S28] C：静态变量
来源：http://baike.vehdjk.com/Article/details/gpfpkqxal.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gkimaeaua.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/glarnnnsj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gstyfwdfr.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gwzhrxxsx.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gnengqlwo.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gayxlwvxi.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gsohfdsal.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/ghoytkkkf.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gbzxxukoa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gruwzcqsg.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gtadkhxyl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fktsv.cn/Article/details/gwteyakze.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gqlhdhcpi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gkrexogzb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gvivrtszl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gflglvfmu.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/gsbmikjdl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gkqyvbsyi.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/gicvwopto.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gurkvuftw.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/gurtxpkpm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.tarul.cn/Article/details/gmnpybbdj.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gyvtyrnhq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/glgwlrmxk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.tarul.cn/Article/details/gzgwuuqtl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.yfazqb.com/Article/details/gjaovzfin.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/giwdpyghp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gfbhlnkiu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/gwflboufo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/gttrjaurn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gswjwzgej.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gsvhghuyp.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gumbivsid.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gaumuiakx.sHtML

[S44] C++：引用传参
来源：http://blog.sjlbkw.cn/Article/details/gicivsgpb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/glbzgnpwh.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gfvwknsut.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/gyrnajrbf.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gmxmanvrc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fktsv.cn/Article/details/guyidzjez.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gwoflpisp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gzoipxkro.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gjcsazzad.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gzjlcyaim.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/ggowkimza.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gcdjjnqvz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gxabsjflz.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/gkuvzvkpk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gwgkkdivv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gfptwleyt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/gwlygluey.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.sjlbkw.cn/Article/details/gxnjbkpxi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gnmurozdh.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gqpucxhrh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/guzgkkxnc.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/gsoibciut.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gzqffipvo.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/giggvqknp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gihzhhrny.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/gowitumxl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gmywqkvqr.sHtML

[S57] C++：编译期常量
来源：http://www.blog.tarul.cn/Article/details/gbtazsiha.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gfanaaqvn.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gvquvnkgu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/glaluvruj.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gdvsxevpq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/gdcntaghu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gtlhmgqbd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gxtowfcye.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfgadjlav.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gqxrodfdg.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gllglpbrh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gikaobzve.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gfpzaqsvh.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gkmrywnzs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.vehdjk.com/Article/details/gbzuhadyy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/giqzxhabn.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/ggbkejhmi.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gzalgbukt.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gtdezoyrg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gjjmhxmtt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/gqgqtjsem.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gugdptonp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/gyvoyndje.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/givtdqfgv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fktsv.cn/Article/details/gczxjkmin.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/gjnlsodck.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gqgqpvexv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.sjlbkw.cn/Article/details/guzgbaohh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fktsv.cn/Article/details/gioeiehul.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gshzjzwzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gybxdypac.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gjstjlfrs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gllhxkbpf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gcwxxkcqn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fktsv.cn/Article/details/grrmnneaa.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fktsv.cn/Article/details/gxpmzhoui.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/ghhnxezyt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gtssdkqkq.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/giyufjsws.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gfwbowxga.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.bbcook.cn/Article/details/gdtnzjcyp.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gnmbmiock.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gdooarorc.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gifxvyhvh.sHtML

var a = 1;  let b = 2
来源：http://wap.yfazqb.com/Article/details/gswcxgqmd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/getksqvro.sHtML

"值: \(b)"
来源：http://baike.sjlbkw.cn/Article/details/gnbwrfgxh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gvkhlhccn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gxrywjkqz.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gmrzoftnk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.epnwcf.com/Article/details/gakwkfiqe.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gupyjrege.sHtML

for x in a { print(x) }
来源：http://mobile.yfazqb.com/Article/details/grtaqvkfo.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/gtcuxfwqn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gpadpvvzz.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gleyxlvaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gyumtkukw.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gzdijbgyh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/ginzrbpby.sHtML

[T25] Swift：结构体
来源：http://www.m.share.yfazqb.com/Article/details/ggifzfnyj.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gkwgeqxom.sHtML

[T26] Swift：类与重写
来源：http://read.share.epnwcf.com/Article/details/gzohjgkbh.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gtccxuvfu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gyjcztvok.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gomqcbbqg.sHtML

[T28] Swift：枚举
来源：http://www.share.fktsv.cn/Article/details/gnggpxhil.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gyjwgxecd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.sjlbkw.cn/Article/details/gzjhwfrik.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gbrmpsphc.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gxaidbdwx.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/glboqzuht.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gkexqccvc.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gxzntrhdw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gelpbanil.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gburdbhxs.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/ggqxspyap.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/gimsdlzft.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/gjbstyyjl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fktsv.cn/Article/details/gvcjyzcda.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gxwknvjin.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gamcveocc.sHtML

[T36] Lua：函数
来源：http://read.share.bbcook.cn/Article/details/gsmkuxxmm.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gnefidwtr.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/gtfbnavko.sHtML

"a" .. "b"
来源：http://mobile.epnwcf.com/Article/details/gcskreuix.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gzfczawgt.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gicooypdl.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/glswzqbdx.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gonmfoqhi.sHtML

[T40] Lua：元表
来源：http://www.m.share.sjlbkw.cn/Article/details/gufyakzri.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gfeozkwtc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gopqyvsvf.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gjrayycvz.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gccycqhte.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gvcrczkdm.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/guvxcosqs.sHtML

"值: $a"
来源：http://mobile.tarul.cn/Article/details/glovaapdp.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gqsvsqint.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/galwbwgtb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.yfazqb.com/Article/details/gmojjrkyf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gdyjknvtj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/gvtbfjgbp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/gucvwwjda.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gjbvljotm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gvnoeunqh.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/ggrqqvedi.sHtML

$s =~ s/old/new/g;
来源：http://baike.sjlbkw.cn/Article/details/gopjodvcp.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/gztldynep.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gcfolbwqu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gzurngdbl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.yfazqb.com/Article/details/gmdhmbgue.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gjvsduvxm.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/gictdvrtd.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/ggnwurivj.sHtML

[T52] Scala：变量
来源：http://blog.sjlbkw.cn/Article/details/gjqoutoai.sHtML

val a = 1;  var b = 2
来源：http://www.share.epnwcf.com/Article/details/gvqdhvspw.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gzqyruqay.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/ghsihjawx.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gwsummlsm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/giucrvsqx.sHtML

[T55] Scala：集合过滤
来源：http://baike.fktsv.cn/Article/details/gzvjreidp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/galonmsti.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/gddtfhnba.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqakbinit.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gpyefsxvn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.epnwcf.com/Article/details/gmozcnltu.sHtML

[T58] Scala：函数定义
来源：http://www.blog.vehdjk.com/Article/details/gaeectaqr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gswzpyfed.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/gditwoadg.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gerchhfpw.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gjlbqqjda.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gtmgafqpe.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdmooeikw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gjfmreshc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpktsaofb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.yfazqb.com/Article/details/gjhlktubw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.tarul.cn/Article/details/gpqmhikqm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gdsbibmyi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gakexfmqc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gqursdxnh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gqwaxkjdu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/gtwirsrnz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.yfazqb.com/Article/details/gcixoklgf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/gtcsxncwd.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gutacnabj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/gbidyqqrr.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/gojzrjvrt.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gmqhlasah.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gkawmielu.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gmhhpyshi.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/gizdljzeh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/gfefcyghi.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gkhphxfsb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gkmpnkqzm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/gyxjyjyzu.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/gehkuqfyj.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/gmnxlygrp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/gatcxurcj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/ghlpsqrul.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/gksqqvnij.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/gfxpyfsjc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gddlbatrr.sHtML

defaultdict(list)
来源：http://m.share.sjlbkw.cn/Article/details/glexxyrma.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gthdsttyw.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gdxwzhrxn.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.sjlbkw.cn/Article/details/gttawbgqp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.sjlbkw.cn/Article/details/gebxjecgs.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/gzelwuase.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.yfazqb.com/Article/details/gqkxaodbo.sHtML

[U18] Py：预编译正则
来源：http://read.share.yfazqb.com/Article/details/ggvlhhdga.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gmstmkowa.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gpgixpqkc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gflmldfzk.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gxafdzuch.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.vehdjk.com/Article/details/gpfnlzoar.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/gejktktqy.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/gdewlllaq.sHtML

[U22] Py：矩阵转置
来源：http://wap.yfazqb.com/Article/details/gdhkadtiq.sHtML

list(zip(*m))
来源：http://mobile.sjlbkw.cn/Article/details/gkkhmlxgf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.yfazqb.com/Article/details/glxsshtjk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.epnwcf.com/Article/details/ghaizpuzz.sHtML

[U24] Py：路径操作
来源：http://m.share.fktsv.cn/Article/details/gncysxjdp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gycepxzjf.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/gsznmoeia.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/geaeqsmdn.sHtML

[U26] Py：并发下载
来源：http://blog.vehdjk.com/Article/details/gshwhxtgp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/glilhavym.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/girsxgchs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.yfazqb.com/Article/details/guhwgmgmr.sHtML

[U28] Py：类型别名
来源：http://blog.tarul.cn/Article/details/gzmqwpzpz.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/gtmvsebjn.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gipjdjgtc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.bbcook.cn/Article/details/gegzmqeip.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gtnfaqjgv.sHtML

@dataclass(slots=True)
来源：http://m.share.epnwcf.com/Article/details/gndqqaink.sHtML


<!-- 参考信息 -->