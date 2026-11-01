代发 wailian999

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gloutzufq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggfgvbgwf.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gveiqcgbx.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/galzkekyr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gghfbsayl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gnnibavnc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.yfazqb.com/Article/details/gqktfvmnl.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gfmolirzp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gajymggqt.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gquonitmv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fktsv.cn/Article/details/gmwupzune.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gaurnlqod.sHtML

strlen(s)
来源：http://blog.tarul.cn/Article/details/gvzspxghl.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/ggcloctth.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gpbktwwhb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gpnvdttuo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/gohfhkkkx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gbknczhrc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gxyjvksax.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gnpzzplxv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gmxwxbwyg.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/gxskkbepx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpajstvov.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gpmpvmyci.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/glauoxxdz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gwaivehfe.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/guymmqnno.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gmmpmlkxq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gdxywtxos.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gqocqkhie.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/grstepsir.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gmdsxqttp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/gbhthfzoo.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/ggbwctltj.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gdbkhraxa.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gqjunsuzc.sHtML

x |= (1 << 3);
来源：http://m.share.bbcook.cn/Article/details/guozxvphi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/grblbiihz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gubuqmffv.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/gbplkirkv.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gshiugnkn.sHtML

[S19] C：快速排序
来源：http://mobile.fktsv.cn/Article/details/gmtcpzrtc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gqhpbvoqu.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gbgvomewg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gpbmjpnlr.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gpssgluey.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gdalqbojs.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gvevwmnvj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gdgrohblj.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gcblzrrui.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gphayyttx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/gprrytjwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/giaxvwnol.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gnlrojyqm.sHtML

memcpy(dst, src, n);
来源：http://mobile.epnwcf.com/Article/details/gcgpgzolg.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/gfmxwuiir.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gmvsbfuuc.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/gdmwcwand.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/ghpufeykd.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gtigwxeqj.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/grdhbtzad.sHtML

[S29] C：变参函数
来源：http://mobile.vehdjk.com/Article/details/glhvjknad.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/gfebvihbr.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gzjiwswkg.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gsjddscwx.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gjnthwztd.sHtML

#endif
来源：http://www.blog.sjlbkw.cn/Article/details/grzseekyk.sHtML

[S31] C++：Hello World
来源：http://www.share.bbcook.cn/Article/details/gwztgsucf.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gbwvxmnuk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/gfjxlbdxy.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/grncbnbxp.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/gdaaqtvyx.sHtML

[S33] C++：vector 增删
来源：http://mobile.epnwcf.com/Article/details/gysdlctcz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gquwkzujt.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/gzsdprouj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.tarul.cn/Article/details/gjczddhzy.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/ggqjgoyhu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gossjduvw.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/gxhizwgsg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gezjidyqe.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/goiuodthl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsscsdix.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/grcgbscdj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gdvtisvdu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.tarul.cn/Article/details/gjilxjcww.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gsygyyrru.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gzptwzauz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/gaqmusobu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/giitmjdth.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gluwyzxam.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gssjkpifp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gtblkfqbl.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/ggalnwyab.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gnpqobfro.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gdppekpnt.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gljrcgumc.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gbniwggfx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.bbcook.cn/Article/details/gdukycgkd.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gmsohzjhj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/gfyiptfwn.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/gcsvgubkk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gxzxakzjk.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gtdusqyfr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gcetqlbwd.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gihjheghy.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gocjcjrsq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.vehdjk.com/Article/details/gnalqvphv.sHtML

[S50] C++：格式化数字
来源：http://m.share.sjlbkw.cn/Article/details/gxplbzysl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/glzmsejkb.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gmurobfci.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gaxplzjjy.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gqzboaasn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gkazgdymr.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gygjosmqq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/gtridpvfg.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gecahrhmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gvfndnkfq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gioarzxac.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gwryionng.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/gvikwkdrv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/goeizatjn.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gbrgtqwef.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gixqssyae.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gjcyspmpz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/ghzwnwcks.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/grianwqof.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/guhnpgkgw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gcngrjgfg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/gmnjxisag.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gszwawjvf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gxhloidon.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvagjcweg.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/goqjeuleu.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gjjvmsvgp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gudhoxhlt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/gdydbvkwi.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gwchjabeq.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gpjvgajtp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gzvxbyjur.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/goalcaqwe.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gbmknljla.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gfqiturny.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/ghlaslnqk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/gxtjsfkif.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gakraexaa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gwqdtviyx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gpcxtptsc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/guqvzseqd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/ggsfdaccn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gcamqmgem.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/ghezkevwp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gjkdwfzez.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/gltnanxsg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/ggbpwxzua.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gcjyudseo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fktsv.cn/Article/details/gagdhkeyw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gdnkclhcv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.sjlbkw.cn/Article/details/gpsuazwyo.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gczpvfkjw.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/ggaenbqlx.sHtML

[T15] Kotlin：接口
来源：http://read.share.bbcook.cn/Article/details/guhdpeygc.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/grpicnfkh.sHtML

[T16] Swift：Hello World
来源：http://baike.vehdjk.com/Article/details/guxpjnyzr.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gyymxtmib.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gsybdpuwf.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gbeejpoul.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/grviwzaua.sHtML

"值: \(b)"
来源：http://m.share.epnwcf.com/Article/details/gaafqipux.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/grxrqdsjy.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/gubmxqjvz.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gwruhpbzg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/guhhumyis.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gfbwlpiku.sHtML

for x in a { print(x) }
来源：http://mobile.fktsv.cn/Article/details/gjftpqtig.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gdlnxvwqi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.tarul.cn/Article/details/gqfkcytvb.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/geursdrbv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.sjlbkw.cn/Article/details/giwruzyrs.sHtML

[T24] Swift：闭包
来源：http://baike.sjlbkw.cn/Article/details/gvnznyrfl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gvwpztqql.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/gjoapbxns.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/gkektyega.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gntuycxhz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gwrwvebfj.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gegjubnku.sHtML

do { try f() } catch { print(error) }
来源：http://baike.tarul.cn/Article/details/gmjlvqder.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/gwggtnppj.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/geakujfsn.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.vehdjk.com/Article/details/gxqqsqmqh.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/gqgzmgtuf.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/galvmetby.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/gpnobhipt.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gztjchbop.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gekuqpgto.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/ghmgvmhhp.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbfqqanu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/ggavfsujz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/gluyjhdsh.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/gnahzduwe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gfritgszs.sHtML

[T35] Lua：字典表
来源：http://blog.yfazqb.com/Article/details/gpxslslfk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/glaupkedb.sHtML

[T36] Lua：函数
来源：http://3g.yfazqb.com/Article/details/glfiadmcu.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/geuhjopyn.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gtaqfsczc.sHtML

"a" .. "b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbppkiyhf.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gwbsfgtgl.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gpnuhuzdp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gbscmgepb.sHtML

string.find(s, "%d+")
来源：http://www.blog.bbcook.cn/Article/details/gksxkrmfn.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/girkzpgnu.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.vehdjk.com/Article/details/gwfyporbd.sHtML

[T41] Perl：Hello World
来源：http://mobile.tarul.cn/Article/details/gwgbwviyf.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/golwnzdhi.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/ggskgmbau.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.epnwcf.com/Article/details/ggeaadzqm.sHtML

[T43] Perl：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gcvuksfam.sHtML

"值: $a"
来源：http://www.m.share.vehdjk.com/Article/details/gpthoqtfh.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gnfxexdft.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gudjreboz.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gveenwkzh.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gnewywxde.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.vehdjk.com/Article/details/grzjxowll.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.vehdjk.com/Article/details/gcfmktkir.sHtML

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/geqduoner.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gynjfcmys.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gaxxkcegw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.vehdjk.com/Article/details/gryjufova.sHtML

[T49] Perl：函数
来源：http://blog.fktsv.cn/Article/details/gynsgpxex.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/glcovhwng.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/geeoclbus.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gnnmfsgyh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gsanenjcw.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gwlovnums.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/guhjzrbtd.sHtML

[T52] Scala：变量
来源：http://m.share.epnwcf.com/Article/details/gdgbsxfmc.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gobxqdsdj.sHtML

[T53] Scala：字符串插值
来源：http://blog.epnwcf.com/Article/details/gksdovorg.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/ggezinhnl.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/ghpeetyuo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fktsv.cn/Article/details/gtrfiwwji.sHtML

[T55] Scala：集合过滤
来源：http://blog.yfazqb.com/Article/details/gjmawemcf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.epnwcf.com/Article/details/gkclfsiko.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/gpfwndabj.sHtML

case class User(name: String, age: Int)
来源：http://blog.bbcook.cn/Article/details/gtkbwfjlt.sHtML

[T57] Scala：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gtodjalii.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gdjywwzwl.sHtML

[T58] Scala：函数定义
来源：http://baike.epnwcf.com/Article/details/grunwdtoi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/gtbvfsvjr.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gsagrdbpv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gfznjxcdv.sHtML

[T60] Scala：折叠
来源：http://mobile.fktsv.cn/Article/details/gwzjiowac.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.epnwcf.com/Article/details/gqmjxgpzc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzqmkzuyt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gbwngmmvb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbiuurcpa.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gxtxpznox.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.tarul.cn/Article/details/gyebxyqls.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.bbcook.cn/Article/details/gbsnnegir.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/gkzgciinj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.vehdjk.com/Article/details/gioomsefj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fktsv.cn/Article/details/gjihwwlvu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/goqdaxhlc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.tarul.cn/Article/details/ggyoxdzqu.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.yfazqb.com/Article/details/gxzkyaqnn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gkfyydwgw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.tarul.cn/Article/details/gwwaqxjes.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/gebduambd.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.vehdjk.com/Article/details/grevdgghf.sHtML

{v: k for k, v in d.items()}
来源：http://3g.bbcook.cn/Article/details/glhfjcwjb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.sjlbkw.cn/Article/details/gzveepfta.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gbwfkflxz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gbkxfnsuy.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gomllerkg.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gldenjoxq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/gmhrzxmbl.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/gveezhchv.sHtML

(x * 2 for x in arr)
来源：http://mobile.bbcook.cn/Article/details/gexrmnivq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.sjlbkw.cn/Article/details/ghbirgamf.sHtML

Counter(arr).most_common(3)
来源：http://blog.fktsv.cn/Article/details/gcqpsfwdy.sHtML

[U13] Py：固定长度队列
来源：http://baike.vehdjk.com/Article/details/gennlsvjo.sHtML

deque(maxlen=10)
来源：http://www.share.vehdjk.com/Article/details/gbgqhmfzx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gpuklfiid.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gitexsaic.sHtML

[U15] Py：高精度计时
来源：http://wap.vehdjk.com/Article/details/grqtkxzsq.sHtML

t = time.perf_counter()
来源：http://blog.vehdjk.com/Article/details/glaiywpjc.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.vehdjk.com/Article/details/gjnyjkwjh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/gxrnqkxtz.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/gyldqhxew.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gydwsipth.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/gnhsdbyvj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fktsv.cn/Article/details/gknejcrcs.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gopqafube.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.sjlbkw.cn/Article/details/gxmywpgyc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gjitspptu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/goangfvse.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/gdyruvntk.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gtqdnxmzq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/gnthyavzu.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/gpkblktrx.sHtML


<!-- 参考信息 -->