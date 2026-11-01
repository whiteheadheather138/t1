代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.sjlbkw.cn/Article/details/gqnvdqgde.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/ghwyzftwp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gpkkxyfac.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fktsv.cn/Article/details/gszcthfpn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/grscfkqiq.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/gqjatrgnn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gdjfmhcjy.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gacycgfbw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/gtdemumcv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/ggyrsomvg.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gbgsvbniv.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gonoaayyb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gayaitzwd.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/girmqunih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/goqjxkktr.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gqxozwihy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gnldwpdog.sHtML

[S15] C：类型转换
来源：http://wap.fktsv.cn/Article/details/gpvgcqbir.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gbknvckel.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gfcqijrxk.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gtjjeckkz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gqirafkwq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gwgbgrirg.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/ginoelhoh.sHtML

int main(int argc, char **argv)
来源：http://wap.yfazqb.com/Article/details/gtvueaxjg.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gjldstoaw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/giaphzbhm.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gtntbtyfj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gikyiubfj.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/grzbsdhql.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/gvvemzwrm.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gbglngazl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/geihbuijz.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gxxoogwbt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaakqgxq.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gustlsvbf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gmvsdwghd.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/genigrmig.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gjnmxvqdj.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/gtvnxtrmy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/grssedfja.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gjhsnsgss.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gsmmxomxh.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gyrdmvrwg.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/glcrcmsgy.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/gcaevrysj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/ginemqjuz.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/ggxxbktwm.sHtML

#ifndef X_H
来源：http://read.share.epnwcf.com/Article/details/gperzyrby.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gcupbfygr.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gqobldqzq.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gxtwdkjxw.sHtML

#include <iostream>
来源：http://blog.vehdjk.com/Article/details/gplrfbhhh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/gyedmnkwi.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gxjuihspv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/givciezme.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/gpganruud.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/gjlziqdzl.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gnkmlvamt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gstjmblaq.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/ginsvzgcu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/geprewqdk.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gusphfnzk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gqbkxwdau.sHtML

[S37] C++：set
来源：http://baike.vehdjk.com/Article/details/gnbspdudo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gpojctivg.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/gtjdukvze.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gecposfbf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gznammvth.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gpnihgqxn.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/geillgnho.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/ghoiquvfj.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gjcwatrrj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/gdljtghhc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gnijryvkd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gdfotfysm.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gsqhbezef.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/gctqasgqn.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/ghkdvjqjo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gozlrroyv.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gsiurllha.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/ggogzumwk.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gdszdljhe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/gszneznxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/gmhmofumf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gtcnyhvnn.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gyfevdoqs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gntfkmwhu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gnxbwbket.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/gnokqqvfh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gbzgmtvkv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gdusmtvus.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gljanzsqn.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/geionwdul.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gwwwcdbjv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.bbcook.cn/Article/details/gagyyyhhq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/gibbtayrh.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/gfecspvps.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gyjrpdzoe.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gilrcagiy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.yfazqb.com/Article/details/grcncanea.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gdgfdpixm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gzinumgzt.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gqvsrpfpd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/ghgazuxpe.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gqqogatbp.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gtbpqiqtk.sHtML

[S58] C++：命名空间
来源：http://read.share.yfazqb.com/Article/details/gzymvootr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/glbyarhxw.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gakpxzcxa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gyihmykoa.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/gixiqsgdo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gongjamlr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gguhzlynx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gzukdayxn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqjbbvkmd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gpdnaoquk.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gahrsbvpn.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/gvcppvodo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/glsousiml.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/ghmhkdjwj.sHtML

"值: $b"
来源：http://blog.bbcook.cn/Article/details/gnjyhpjzy.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gkeofuntw.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gqbnnhgpa.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gcvhvgmdv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/ghrjdjfus.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gtcumjfoh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gazydykzc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/geostbfdq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/graoagqrb.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gzpzdktmh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.yfazqb.com/Article/details/ghypaiyje.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gyuyavsye.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gfefwndoo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gqizromzy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/ggfvrlfmd.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gwjqykwqp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gdlhchzpu.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gowgfaqhc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gmtblkocu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gnxkeyzlj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gpygzayzh.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/ggouoimmy.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gqfntafip.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/gusilvdgq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gsdbgkely.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gxjtwkqbz.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gxusgzung.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/gtkrexwse.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/gyjwnfgqx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gizgpeqay.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gsrxhpbli.sHtML

[T19] Swift：可选绑定
来源：http://mobile.epnwcf.com/Article/details/gjnzkfpoh.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/glwyddgoh.sHtML

[T20] Swift：数组操作
来源：http://baike.yfazqb.com/Article/details/gavqrlqav.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gibpzpmfk.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gpjdhlfsr.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gabvdesge.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gowxqhluj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gkdpcmukk.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/gndrdioyw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/ggcbsigqb.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/glvrmbhfz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/ghoyhsjwg.sHtML

[T25] Swift：结构体
来源：http://www.share.fktsv.cn/Article/details/gsnclhvmn.sHtML

struct P { var x: Int }
来源：http://mobile.fktsv.cn/Article/details/gedabrdeu.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gzcamncic.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/guyzmombb.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gqorcvoer.sHtML

do { try f() } catch { print(error) }
来源：http://baike.bbcook.cn/Article/details/gyuaccwsu.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/geoovlnoj.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gdgphbosl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/guhlcoaip.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gwhpuoobn.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gnlhgtpst.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.epnwcf.com/Article/details/gkbyrnfzm.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gtwwosmks.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gpxjmrbql.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gogfgwigy.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/gywqwodsy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.yfazqb.com/Article/details/grlyskust.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fktsv.cn/Article/details/gdckeadsh.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gifryyahf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/ghcsdqmbb.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gnajmuyyk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.bbcook.cn/Article/details/gdfyfybzo.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/ghcvsjnvo.sHtML

function add(a, b) return a + b end
来源：http://mobile.sjlbkw.cn/Article/details/gzjznumlz.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gosvygiyj.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/glqozlkvh.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gsngwgagc.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gvkgxkuzc.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/ggoyjkuxq.sHtML

string.find(s, "%d+")
来源：http://m.share.yfazqb.com/Article/details/gkpityhsv.sHtML

[T40] Lua：元表
来源：http://www.share.epnwcf.com/Article/details/ghdjhyxgc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gqbrmyxkq.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/ghytqlwfj.sHtML

print "Hello\n";
来源：http://mobile.bbcook.cn/Article/details/glipmgffe.sHtML

[T42] Perl：变量类型
来源：http://read.share.yfazqb.com/Article/details/gvimsyxdq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gmhhouziu.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gphywirmh.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gfccxiesh.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/ggvevdhnj.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.yfazqb.com/Article/details/gqyfchets.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/grxuqliln.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.epnwcf.com/Article/details/gqwjsveig.sHtML

[T46] Perl：哈希操作
来源：http://www.share.bbcook.cn/Article/details/gsuwnqsut.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gzgezvzrv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/gpgiznqvh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.tarul.cn/Article/details/grrqwytdk.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/gkqmwxypo.sHtML

$s =~ s/old/new/g;
来源：http://blog.epnwcf.com/Article/details/goxxhgmmp.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gqcfqpams.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gnlktmwwb.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gfozpaezf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gjtiuedse.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fktsv.cn/Article/details/gkjfusvyx.sHtML

[T51] Scala：Hello World
来源：http://baike.tarul.cn/Article/details/gghvenzkq.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gibeyirpa.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gfbjpybpy.sHtML

val a = 1;  var b = 2
来源：http://3g.tarul.cn/Article/details/ggqqyjbca.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gdgotjrpi.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/gjqcgsulh.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/ggbbsbtge.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.tarul.cn/Article/details/gnmwzmkqp.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gdajfxjhm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gwwkgpsna.sHtML

[T56] Scala：样例类
来源：http://wap.bbcook.cn/Article/details/gywpapnkp.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gptykixeq.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/ghgedidil.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.bbcook.cn/Article/details/gepiqhilh.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/gtllwqdyu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gryyennsv.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gghbvunph.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.tarul.cn/Article/details/guvowtjms.sHtML

[T60] Scala：折叠
来源：http://blog.vehdjk.com/Article/details/gjzjsxmsg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gieziqnru.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghayyhrfr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/ghtsdjzfx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glqgyaguy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/griuraseb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gcdrujdfp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/gtlgaaaqz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.sjlbkw.cn/Article/details/ggivanbsn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/ghxmsdiol.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/gmrqzklmk.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/guepjgiil.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/glessgrpi.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gxondiled.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gfysvfxvs.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gyzvjqkbv.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gwwglucyv.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.epnwcf.com/Article/details/gioobqfls.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/gwffzqqqu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/gxoretibx.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/grbriewum.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.yfazqb.com/Article/details/glkoumihf.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqdmtrgb.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gstwmaelz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gzupzbqgv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/gzwdtmdgi.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/guavepwrt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/gvucwhlfh.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/gzupsadlz.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gbcvnhlhz.sHtML

deque(maxlen=10)
来源：http://read.share.epnwcf.com/Article/details/ghgqbjuxr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.tarul.cn/Article/details/gedqdmcix.sHtML

defaultdict(list)
来源：http://wap.bbcook.cn/Article/details/gpymwfndi.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gknpdkhsd.sHtML

t = time.perf_counter()
来源：http://read.share.bbcook.cn/Article/details/gnkghhoyx.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gomlvojya.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/grzvvhzqg.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gyqilneuy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.sjlbkw.cn/Article/details/gbdupfjpw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gqsfesfqe.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/goifhsaml.sHtML

[U19] Py：正则替换带回调
来源：http://blog.epnwcf.com/Article/details/getvhdzjk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/gbxrgzqnt.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gkigxmkvj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gbwkcybxo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.vehdjk.com/Article/details/gygwvhxkd.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gbrhzckfd.sHtML

[U22] Py：矩阵转置
来源：http://blog.vehdjk.com/Article/details/gifbhxvmf.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/glllwsepe.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gayapjytk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.epnwcf.com/Article/details/grasksinu.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/goeipiaal.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gmoshjrkz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fktsv.cn/Article/details/gefrnpdqa.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/gfdgvwzrz.sHtML

[U26] Py：并发下载
来源：http://blog.fktsv.cn/Article/details/gbfatzjzo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.epnwcf.com/Article/details/gfahmybeh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/ggzmdiljh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fktsv.cn/Article/details/gxjhgqorb.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/gjgtsekea.sHtML

UserId = int
来源：http://m.share.vehdjk.com/Article/details/gzbgvdxfs.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/gvnowwugu.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gnyaziglp.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/gbkjriryv.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gvntunzgy.sHtML


<!-- 参考信息 -->