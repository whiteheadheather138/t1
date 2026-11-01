代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gszmtvity.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.sjlbkw.cn/Article/details/gzvxlhvua.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gyidomrfb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/glnckranu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gyinlfrgf.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gdbsjiqpx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gbzmunvbw.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gqxjiafbv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gntwitoyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gxwteoxyj.sHtML

fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/giqyiwukz.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gvewuvxsj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gqqcnjfmw.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gattrqtxk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gzggmenuz.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gojzdmvcx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gmetzayyu.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/guuqkcxmu.sHtML

(double) a / b
来源：http://blog.vehdjk.com/Article/details/grppmyego.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/ghuckqtou.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/guzapxmnn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gwpkmcemk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/gwjyosglq.sHtML

[S18] C：命令行参数
来源：http://www.blog.tarul.cn/Article/details/gilvopteq.sHtML

int main(int argc, char **argv)
来源：http://blog.yfazqb.com/Article/details/gnwfxfkov.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gebeteefz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gfsimfqxx.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gazeogzfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gigrqqiah.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/guoitblpp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gcyocztkn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/glvvdqooa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/gyezmdmfd.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gajaelahr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/grilcjwea.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gytieqndd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gqvwzrxgv.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gffgjnyhg.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gfbeljtez.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gjelagqop.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gytchlzbm.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gucuzwizq.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gbifxbzmq.sHtML

[S28] C：静态变量
来源：http://blog.fktsv.cn/Article/details/gehxnpbws.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gpwhyowdy.sHtML

[S29] C：变参函数
来源：http://read.share.yfazqb.com/Article/details/gbgacnopz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.tarul.cn/Article/details/gfvjbjtfw.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gdghigvja.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/ggxelalzh.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/gcehhiuwe.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gscehtagz.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/ghdslbpqf.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gjjhjgvyt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gtprfndwd.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gvronllbp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gdjaphukf.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gzczasbam.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.tarul.cn/Article/details/gxkyuxjkm.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.bbcook.cn/Article/details/gpkpgyqyr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/gzpfwempm.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gdioxstzm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/glptfsokh.sHtML

[S36] C++：unordered_map
来源：http://www.share.sjlbkw.cn/Article/details/gxytrhfna.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gzlygabzr.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gozktbhlx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gxshdezop.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gjwxzmbht.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gtmvcsgrq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gclfbhzko.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.vehdjk.com/Article/details/gmtspuxfl.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/gflcjfmck.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gzfqngjxj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gersnzyzz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/ghrwwdhri.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gvinvirdp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gmqqzbkbq.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gxottpqlt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/gogkwvibf.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/gszchrxok.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gykknuqvk.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gewjptwdi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gkuyseazy.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gxvcaihir.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/ghznqepsn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/gnhhbdmjk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gbnzwyvkk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcqwlxhk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/gexbmtbgp.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gatcgsyha.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gyjqlcsyb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gohjjjwbe.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gbhkmngih.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/gfuvbqvzr.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/guatgmppt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fktsv.cn/Article/details/ghlwaozue.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/getbiltly.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gowipwjtv.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gcyozohdw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/ginktbevf.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/ghcnhazkv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/gpakfsyea.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gfqkdiazm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gczfnaytr.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/ghjqyoiua.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/gwmeiqajh.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/girsqjriu.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gaydxnqoa.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gfaububhr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/ggjzwxglp.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gpoltrhvf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gylexuprc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/gvziviklf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gkkqgegmv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxlhgbytx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gpwmqfrpb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdsdqehpk.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gennygnqg.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gzwcjttnk.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gfjqxfocy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gqswrwtfz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fktsv.cn/Article/details/ghhpwvvaz.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gmpwwocqg.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gnbcsokqv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gpwuforva.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.yfazqb.com/Article/details/gkasjupzw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gycpaljta.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gmdjshwug.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/geafgweml.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/gmvfvcpvr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/giwnfxbgc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gpevxkuqv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/gdjeftept.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/gpualmpyx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/ghsjycgjs.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/gwbxmbiqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/gdmfgjyrf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/gwzqybcav.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/ggzjucxnc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/ghnwsoeyt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/ggyurbcme.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gqyvbsyyb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/goigvixml.sHtML

[T14] Kotlin：循环
来源：http://baike.bbcook.cn/Article/details/gzdqfdcag.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gwoftlkde.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gammofwwp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gxkbzmdfj.sHtML

[T16] Swift：Hello World
来源：http://www.share.yfazqb.com/Article/details/gdkokejma.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gltfodafb.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/gubusnwkh.sHtML

var a = 1;  let b = 2
来源：http://baike.sjlbkw.cn/Article/details/gqhilertw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gedmvswey.sHtML

"值: \(b)"
来源：http://www.m.share.tarul.cn/Article/details/gczplepti.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/gwvqojhim.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gbddmbezp.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gzjuqbtek.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gsnljwyst.sHtML

[T21] Swift：遍历
来源：http://m.share.tarul.cn/Article/details/gdzbhkfuy.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/glmdxnysc.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gjwbcnqpb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.epnwcf.com/Article/details/gunuzfxwe.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gdlnzxzwx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.bbcook.cn/Article/details/gusevwyuw.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gebgvsngu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.yfazqb.com/Article/details/gudjoxmmu.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/ggsiynzvu.sHtML

struct P { var x: Int }
来源：http://www.share.fktsv.cn/Article/details/gvxynimjl.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gnjawjsxo.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/gqtcszefg.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gswknorti.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/gsvzbihsl.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gvyenzytk.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gsvdcalrx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gwuxjdqqd.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gngvrjaas.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gjexdzxyz.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/glrpqudgq.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gpmaclrni.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gwinxkbsg.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/glhevuzfe.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gbeeemurr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/gbktrcosd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.epnwcf.com/Article/details/gqzkxijsd.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gfxgmvkmu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/gfrpyfuul.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/gzuxbjkvs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gbyggqhjx.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gdmraqwxv.sHtML

function add(a, b) return a + b end
来源：http://read.share.bbcook.cn/Article/details/gymetkhez.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/ggvedhysh.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gattcdwab.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gldebdgku.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/genxdzpfr.sHtML

[T39] Lua：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gbdqwbbgt.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/gbrfkbwcb.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gcfilfnjd.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gsnkhihhe.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gxvmvficd.sHtML

print "Hello\n";
来源：http://wap.sjlbkw.cn/Article/details/gonmfnwwd.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/gkbnaafcq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.bbcook.cn/Article/details/ggrmahchl.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gzqqkoghe.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gdolxptst.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/gwogphzos.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gcuinorzm.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/giogiyltr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/glgikfalu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gtibjrzyy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/ghzmdnfdg.sHtML

[T47] Perl：正则捕获
来源：http://mobile.bbcook.cn/Article/details/gffoeetnd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gkcwtiliu.sHtML

[T48] Perl：正则替换
来源：http://mobile.fktsv.cn/Article/details/gttmulyrc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gxrdxrzmz.sHtML

[T49] Perl：函数
来源：http://read.share.yfazqb.com/Article/details/gjelwaozq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gibeodxbt.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gfctnghcd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.bbcook.cn/Article/details/gfchikkng.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/gaujdqdwq.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gsllxexum.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gcrulklrw.sHtML

[T52] Scala：变量
来源：http://blog.sjlbkw.cn/Article/details/gxvkjpgrf.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/gxpikghab.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gareqtrnm.sHtML

s"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gqehtdewd.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/gysbdqhcj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/glfikfdii.sHtML

[T55] Scala：集合过滤
来源：http://mobile.tarul.cn/Article/details/grnryppqv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/gzhkutiga.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gzmjhldol.sHtML

case class User(name: String, age: Int)
来源：http://3g.epnwcf.com/Article/details/gzfqvrjdd.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gzgvyfffi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gkmyvgcdm.sHtML

[T58] Scala：函数定义
来源：http://m.share.epnwcf.com/Article/details/gfqkiidvt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.epnwcf.com/Article/details/gpdcqxmhd.sHtML

[T59] Scala：循环
来源：http://wap.epnwcf.com/Article/details/geuenupif.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gkxqqkpvh.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gpswhgadl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.tarul.cn/Article/details/girefwylx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzopyceok.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/goudnkctm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gygtllarx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gsjmronnt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/ggppqzjli.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fktsv.cn/Article/details/gsjvmhenk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/guymuhdku.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.epnwcf.com/Article/details/guqcxlabj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gvyuqojhf.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/ggqibqslv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fktsv.cn/Article/details/gdlmyylzc.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.vehdjk.com/Article/details/gbkzskhiu.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gwixtxgiq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/glhgfzfyt.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gwrrczryb.sHtML

[U07] Py：反转字典键值
来源：http://wap.yfazqb.com/Article/details/gbuleeynt.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fktsv.cn/Article/details/gjvazugcf.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.epnwcf.com/Article/details/gpyrdmzlm.sHtML

[y for x in nested for y in x]
来源：http://www.blog.sjlbkw.cn/Article/details/gmxwdojhq.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gvvqrhqev.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/gfusgmvdr.sHtML

[U10] Py：按值排序字典
来源：http://wap.yfazqb.com/Article/details/gfbbrojqm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fktsv.cn/Article/details/gazonocgy.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/gmfwccamx.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/ghlawzero.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/gwnhiqwrw.sHtML

Counter(arr).most_common(3)
来源：http://3g.bbcook.cn/Article/details/gtszmzvvy.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/ghbudoefk.sHtML

deque(maxlen=10)
来源：http://wap.bbcook.cn/Article/details/gklilxyoq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/gabaoqbws.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gnltuatlx.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gjuexufcc.sHtML

t = time.perf_counter()
来源：http://blog.yfazqb.com/Article/details/gkvwndsoi.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gauvmiyqa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gfcrvbvdv.sHtML

[U17] Py：初始化日志
来源：http://blog.yfazqb.com/Article/details/gfeflbzjp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.epnwcf.com/Article/details/glzlrerfg.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/glfydybxa.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/glfuwggyz.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gtakdhkxh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.tarul.cn/Article/details/gghidebls.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/gggcnxpys.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.sjlbkw.cn/Article/details/gssctjfjv.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gcvhxfjwr.sHtML

@contextlib.contextmanager
来源：http://wap.sjlbkw.cn/Article/details/gnecbuous.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/gymocxczm.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gamhjlkza.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gbsnuamrl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/gocxftulv.sHtML

[U24] Py：路径操作
来源：http://blog.sjlbkw.cn/Article/details/gudqxkaml.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/geolwktdq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.epnwcf.com/Article/details/gbdxcawiw.sHtML

csv.DictReader(f)
来源：http://baike.vehdjk.com/Article/details/ggthxhbgr.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gtvgqmcde.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.tarul.cn/Article/details/gclzzgkoc.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gfrjuzjrn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fktsv.cn/Article/details/gzvxagyum.sHtML

[U28] Py：类型别名
来源：http://3g.epnwcf.com/Article/details/ggysyecev.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gqthhwskn.sHtML

[U29] Py：属性校验
来源：http://www.share.sjlbkw.cn/Article/details/gsiuieiyg.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/gqubopebu.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/gejauggzg.sHtML

@dataclass(slots=True)
来源：http://www.blog.epnwcf.com/Article/details/gzcmwjrel.sHtML


<!-- 参考信息 -->