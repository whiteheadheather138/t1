代发 wailian999

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gcadycvlf.sHtML

[S06] C：字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gjrfgmmrp.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gpkxurlzw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gnrxjmebb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gsssnpygb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.yfazqb.com/Article/details/gehafnapn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fktsv.cn/Article/details/gsktjdvyn.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.epnwcf.com/Article/details/giiliuzyp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gcvmpspjd.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gosceibqh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gvgjnbrxz.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gzqpuksme.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/gvadarphp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gdclomzhf.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gwxrrsgmm.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/gucvorjlw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gkjuxftnu.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/gbdnfnbcr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gzqxpuaty.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/ggdnaakzq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gsyictjsx.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/ghixmrnaw.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/goorwwxaq.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/gaijpiyop.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gnnehcthp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gzrflmizx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gziyhxvst.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gezejgtkv.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/ghtxbpgyr.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/grcwtttqz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gdibamzvo.sHtML

[S20] C：二分查找
来源：http://www.m.share.epnwcf.com/Article/details/geanqfgiy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gqkamuzra.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/gahmnnbap.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.bbcook.cn/Article/details/gsqstclki.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/ghryqrixo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.epnwcf.com/Article/details/grhbhtmbu.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/ghpdznkqj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gpevqsgqw.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gdhrypkun.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/gypusttxe.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gklzabdeg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.vehdjk.com/Article/details/ggjflfhhr.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gwyscfjzl.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gkvttwegh.sHtML

[S27] C：定义常量
来源：http://www.blog.bbcook.cn/Article/details/gucaphqow.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/ghxdaaqrk.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/gmnhoyedg.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gzcqxjwsb.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/gpdcoahsg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fktsv.cn/Article/details/gjoxsakxh.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/ggbaipuwu.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gsyexgpgh.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/grncgpgkl.sHtML

#endif
来源：http://www.m.share.epnwcf.com/Article/details/gwyapufft.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/geqslzpne.sHtML

#include <iostream>
来源：http://mobile.vehdjk.com/Article/details/gdozozirh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gntmxvcbw.sHtML

[S32] C++：字符串
来源：http://www.m.share.tarul.cn/Article/details/gzfqhjjvk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gsvubvxwk.sHtML

[S33] C++：vector 增删
来源：http://mobile.tarul.cn/Article/details/ghaxrxdic.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gieexnfmw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/gsoofxrhm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gkakclmgg.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gepmkeaxi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyergtox.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/gzyhjlonz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gqwzygzum.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gndsefflt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/goefdlhct.sHtML

[S38] C++：排序
来源：http://www.share.tarul.cn/Article/details/gqkpanysl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gjqtcqmjc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.tarul.cn/Article/details/gdquwggbe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gfxumxjed.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gkrdarikg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gxtbejgue.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gsxyurlny.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gpsrfkaag.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gwbzpewis.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gyjrfwhec.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/gxkzzlmib.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/glkqlznvu.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/gzckaqeen.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/gtilntrlj.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gkjpdndwi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gbiumfngz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/gzrrqjpso.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.bbcook.cn/Article/details/gjalzqaxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gidnvbdar.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gitlsdlzl.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gmnqdpcqo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gukmnrobn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gpwpcrebh.sHtML

[S49] C++：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gzkeuzgbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gwfremjbr.sHtML

[S50] C++：格式化数字
来源：http://baike.fktsv.cn/Article/details/gxfuxxwdx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fktsv.cn/Article/details/gudphyvqv.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gxxrnigld.sHtML

static_cast<double>(a) / b
来源：http://wap.epnwcf.com/Article/details/gkhhryxib.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gdsnrooed.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gfcccyiwo.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gfxfpccdq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gewyqmaxb.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/guvhofcfo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gpxzdgjua.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/gmnqwxxmv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/girdnlhvn.sHtML

[S56] C++：optional
来源：http://wap.sjlbkw.cn/Article/details/gohhdtchj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/grugkxzlv.sHtML

[S57] C++：编译期常量
来源：http://mobile.tarul.cn/Article/details/gmemdreaf.sHtML

constexpr int N = 10;
来源：http://wap.fktsv.cn/Article/details/gjczpoypy.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/govurtvzt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gcsydzjeo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.yfazqb.com/Article/details/gavqoynod.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gewexlhww.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gqjqmeisf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gogqfzrzd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gigmhthpe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/goerbmziq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxwsfsdfx.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gcnhrlviv.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gynofejmi.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/grceprhbp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/glpgdapoe.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/grukpcnkt.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/grzyrxiso.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gdmyfkful.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/gjbtmcjdo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/gwhpiokzb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.tarul.cn/Article/details/ghcuolwmk.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/glgswjwoj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gkarlbmwf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gbvqeysmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/guanehlsp.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/goiwoqcqw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/ghmcieenw.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.yfazqb.com/Article/details/gdyumtcrm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.epnwcf.com/Article/details/giputzolk.sHtML

[T10] Kotlin：默认参数
来源：http://3g.yfazqb.com/Article/details/geybanohs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/ggipwzkom.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gabxkbgxo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/giiuaaeug.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/giyhyonxh.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gpyqrvgww.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/ggcvhafzy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/gnypazucg.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/gcksdltle.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/gfuqdalbj.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gqgodabaj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.sjlbkw.cn/Article/details/gbvjsqvhn.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/ginafejry.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gvhltnngt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gfnuhwknz.sHtML

var a = 1;  let b = 2
来源：http://read.share.yfazqb.com/Article/details/gdihbbqbm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gajxrylyb.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/geecjvdhi.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.bbcook.cn/Article/details/gfuflchrd.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/gtxxltmsd.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/gzilngtqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/gjkhmjnsw.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/ggnrshsub.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gtmaiiiwy.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/grlcyqiju.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gjhqvxvce.sHtML

[T23] Swift：函数
来源：http://baike.bbcook.cn/Article/details/gsmnieckq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gzwatkndi.sHtML

[T24] Swift：闭包
来源：http://blog.vehdjk.com/Article/details/gryxdiogz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gibjawvqt.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/grifxslrc.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gkrxvjlau.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/guhzotjqi.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gslvfsajg.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gezjlmabf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fktsv.cn/Article/details/gdptgvxxf.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gwozmuvxk.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/garcdlogz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gwcaqqzfx.sHtML

guard let x = opt else { return }
来源：http://m.share.vehdjk.com/Article/details/gtcatmsen.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/ggjvmlait.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gjmfjvijb.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/ghkrxmieu.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/glajavdjr.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/gcfvwlckz.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/grnxmiuwb.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gxfvlbimy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.sjlbkw.cn/Article/details/gpthaxabv.sHtML

[T34] Lua：遍历表
来源：http://wap.epnwcf.com/Article/details/ggohxmvao.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuvwotht.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gfdtbcrng.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gkwnckath.sHtML

[T36] Lua：函数
来源：http://www.blog.tarul.cn/Article/details/gygolnqtf.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gsswqkkpa.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/gdhteoizd.sHtML

"a" .. "b"
来源：http://read.share.bbcook.cn/Article/details/gniaqscey.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gnchyjvpm.sHtML

if x > 0 then print("正") end
来源：http://m.share.vehdjk.com/Article/details/geydzhigi.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/glqvenach.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gzsijcnoc.sHtML

[T40] Lua：元表
来源：http://www.blog.fktsv.cn/Article/details/gexiebnpy.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.vehdjk.com/Article/details/gytebpwou.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gubskhaig.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gbwnbklzo.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gutdfkmyj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/ganuwowcr.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gxctijbwu.sHtML

"值: $a"
来源：http://wap.vehdjk.com/Article/details/gzsatwghz.sHtML

[T44] Perl：条件
来源：http://read.share.vehdjk.com/Article/details/gbzwavufz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gsxrpnnid.sHtML

[T45] Perl：数组遍历
来源：http://wap.bbcook.cn/Article/details/galgnrbcs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gxwqrbqpz.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/ghnhtewbx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/gqivpnydk.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/gnyweyaim.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/gtfuyohwu.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gcrifoyjr.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/ghsrfzhgp.sHtML

[T49] Perl：函数
来源：http://blog.tarul.cn/Article/details/gfxgpodxj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/guzzvxcau.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gatpyxdtb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.bbcook.cn/Article/details/gihclsscr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gyrwuxhlu.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gpuoyztou.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gtrksqyck.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gyfpsjwwi.sHtML

val a = 1;  var b = 2
来源：http://www.blog.yfazqb.com/Article/details/gwmjclkfw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/giyfonioy.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gcztxiedo.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gcwdbknrg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.vehdjk.com/Article/details/gvtwfakjl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gldbeigle.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fktsv.cn/Article/details/gegzeaidx.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/ggmjlxogu.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gyulcvtpj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gonsphdfm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/gqnoazsig.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/giworoufz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.tarul.cn/Article/details/ghpppvdrl.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gtgilooih.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gzvzstaee.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/glbxnlzli.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gzlntgfux.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqwtjbovv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/ggvrsgojj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gghodzbtq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.vehdjk.com/Article/details/gpfidryaa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/ggfgvkcor.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gnaaievpo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gdwnqmyob.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fktsv.cn/Article/details/greerkmqv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gwhrtitwh.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gumzwpqcf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.vehdjk.com/Article/details/girnyvpop.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gneydnkho.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gbacunoyq.sHtML

[U06] Py：合并两个字典
来源：http://3g.vehdjk.com/Article/details/grsayphck.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/gnebwhhjo.sHtML

[U07] Py：反转字典键值
来源：http://3g.sjlbkw.cn/Article/details/gvgxriqeg.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.sjlbkw.cn/Article/details/gfryimfdx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gvicxpfro.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/gixoyrzik.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.bbcook.cn/Article/details/gwrjftykz.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gznsjxjkl.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gsajxxmuk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/glqcuyfly.sHtML

[U11] Py：生成器表达式
来源：http://blog.bbcook.cn/Article/details/gbcunxycy.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gyqmeciep.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gerzayufv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gkxtjxykj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.tarul.cn/Article/details/gnsmroyai.sHtML

deque(maxlen=10)
来源：http://www.blog.yfazqb.com/Article/details/gcmyyiabx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gkfwgqzex.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/guedlfsye.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/gyqrpyuze.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/gufskogpn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.sjlbkw.cn/Article/details/gwksxjtwz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.tarul.cn/Article/details/gebaiwcnt.sHtML

[U17] Py：初始化日志
来源：http://m.share.fktsv.cn/Article/details/gfmjixljf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gaqwxzzvi.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/gpzlcwbka.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/goipdpvdw.sHtML

[U19] Py：正则替换带回调
来源：http://baike.epnwcf.com/Article/details/ghheetnlk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.tarul.cn/Article/details/goxobegui.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/gohajmtsl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.vehdjk.com/Article/details/gpuzxidbg.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/guimhfbea.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gvqslzfoq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/gplposqxa.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gwwdhvnnm.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/geycdtnbi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.tarul.cn/Article/details/gnremvxim.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/ghpeaogaj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gsmbefrmt.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/guufmwbbl.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/glbsdwqip.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/gkofusnjm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/gbbhoeqjr.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/gjfbpouky.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.tarul.cn/Article/details/gwjswsbns.sHtML

[U28] Py：类型别名
来源：http://baike.yfazqb.com/Article/details/gaspcjmuh.sHtML

UserId = int
来源：http://www.share.vehdjk.com/Article/details/gqxxqumog.sHtML


<!-- 参考信息 -->