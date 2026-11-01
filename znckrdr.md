代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/guqyjcwco.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gswslfcsj.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/guhuailkr.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gaxbpqdar.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fktsv.cn/Article/details/gynwymbre.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gjodlhlcw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gxtyrxozy.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/gtntomovn.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/gwgtgoqfs.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gayvkvuzw.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/goyfufypw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gkwluvvwk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gfjmgewfp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gfmczsnef.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.sjlbkw.cn/Article/details/gppiyrwjy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/gpcaxydgh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gwhwqetmq.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gzswqykcn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqqaoluj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgygvxzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gmiuhejra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fktsv.cn/Article/details/gyobyuusp.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gocmgkikn.sHtML

[S12] C：写文件
来源：http://wap.sjlbkw.cn/Article/details/gqnbncsao.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gahubiwqr.sHtML

[S13] C：宏定义
来源：http://baike.sjlbkw.cn/Article/details/gufwjzarh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gbnnwcarb.sHtML

[S14] C：枚举
来源：http://read.share.epnwcf.com/Article/details/gznnbnsjo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gbybhsbyp.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/getazkjlw.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gaqlnchor.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/grgjmmrgj.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gvlrbrzgd.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gxrvnrisy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.sjlbkw.cn/Article/details/gpbekpftj.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/gefulzbvd.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gufgyvsfg.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gbkeybkca.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gqgxcqcji.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gwdtiyiof.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gmeghxuwx.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/gmhbmuwep.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.tarul.cn/Article/details/gmylqehra.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gcnfbjgng.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gfyyspcpz.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gwwqwrubr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.sjlbkw.cn/Article/details/goktdqbam.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gythukbnl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gkqvtyudd.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gebtkjmpf.sHtML

memcpy(dst, src, n);
来源：http://wap.epnwcf.com/Article/details/ggbfhfwtj.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gjgfcvsrw.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gkhqdlpgx.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjcsfygu.sHtML

const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gflexsvov.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/gwjmaodkz.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gdtdkehvl.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/ghfvhtpzf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/gbtpfiyhk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gijipkffo.sHtML

#ifndef X_H
来源：http://mobile.tarul.cn/Article/details/gghldzxar.sHtML

#define X_H
来源：http://www.blog.yfazqb.com/Article/details/gxugapmqz.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/giitulttl.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gwxreawqz.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/grhknctdy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gofquungf.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gtonenhlp.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gjcqsynjs.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/gkxzydklf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gddgpqmie.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/gpzvnofbp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/grcwhjhri.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gmtdbeeuk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gkuhnbofj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/ghullkziw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gvpmkhsqs.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gjwxirpje.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gvhxtirmz.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gtbehertz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/ggudofliy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/grxugbxbx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gkkjizcfk.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gzhbrbxgy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/glecxukku.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gwdxkprbj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/givybrtmf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gevjlzvmj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/glwdylfkx.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gzcfmfsok.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gcwmrzpcd.sHtML

[S44] C++：引用传参
来源：http://www.share.bbcook.cn/Article/details/gvfzviskv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/gsxluudpe.sHtML

[S45] C++：lambda
来源：http://wap.bbcook.cn/Article/details/gkwibycmc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/ggjcievus.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gpgggkcuv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/gjyqahzcv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/goqjlbjzr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gqmvhgzvs.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gagnzrclh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/geipifiel.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gbytbgnks.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gjfftbega.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gktpmvzwu.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gqyzwjtad.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gnkfpeyvw.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/gctgrjcmg.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gcbizgdlq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/glbypzdfj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gddpgmsmr.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gtdiidccu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gfwmuscps.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gqlhgsick.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/guzuxqleg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gsniqpbei.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/gwcfevtmk.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gsfknqhnn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gcchfhjjr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gsartharh.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gggjkkwsv.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/glppzyvls.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/gkgbzngcp.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/gwjixjpdk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/gndfupuyh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gxycwdlhn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/ghovpdxvm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqatpkeok.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/grhnstwxv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfnwjpnab.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/galnduyil.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gwiyjecwd.sHtML

[T02] Kotlin：变量
来源：http://wap.tarul.cn/Article/details/gstetdasj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/ghznbkveu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/gljnkspqq.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gogoufsxv.sHtML

[T04] Kotlin：空安全
来源：http://3g.fktsv.cn/Article/details/gtwetsnqt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/gqqttyhsy.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gxqlbormf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/grizdsjkn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gjywngejk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/gfovlgpda.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gfasrllhl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gtrqzzeew.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gwehchhsf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gfhoyosns.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gvvctykyi.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gdkfcvbjz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gpbvarpky.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/geivjiouf.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gukwlztpf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gimhqhjzj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gizurzzrm.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/gfgqgqxka.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gvjvvparv.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gnhmmihbg.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/gietowafr.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gpyqwrxzl.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gandctyog.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.yfazqb.com/Article/details/gmxafdrmu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ghgscqohs.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gtgigchno.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gaftgarsy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/geilofcvq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/grolnqqqd.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gepqhslbo.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gqpdipbkc.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gpxkowuch.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gtudsgycp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/glqgrwbos.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gjwxrqlwn.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gvcgzcbxc.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/gvuukbjpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gfozhcmfv.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gmzhfjwxk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gthhgulwf.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/gyconoowx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/guwgmwjmy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.yfazqb.com/Article/details/ggxtaadtb.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gopxosutz.sHtML

[T26] Swift：类与重写
来源：http://www.share.fktsv.cn/Article/details/gnxmwvues.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/gxbfhevvy.sHtML

[T27] Swift：错误处理
来源：http://blog.vehdjk.com/Article/details/gfyzdxukx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/genqhmgmc.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gfyvernbl.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gixicsbnn.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.yfazqb.com/Article/details/gnegitgcb.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gentynyfe.sHtML

[T30] Swift：协议
来源：http://read.share.tarul.cn/Article/details/gjyzffakf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/gdzsyefnq.sHtML

[T31] Lua：Hello World
来源：http://baike.sjlbkw.cn/Article/details/ghclzhfds.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gjrqfeolq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gxlxegryo.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gxbakouag.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/guhhlslth.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/gvdudowag.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gppgvtpvi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gmwhmbgyw.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/gxnkiemhz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/gzclwfosl.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/gtyluzmgy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/gnsouyjhl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gbboyrwuq.sHtML

"a" .. "b"
来源：http://read.share.bbcook.cn/Article/details/gmpcqcrla.sHtML

[T38] Lua：条件
来源：http://www.share.vehdjk.com/Article/details/gdunwodbh.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/gyktfrfbu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gpylhivqu.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/gqjnnvagl.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/gnrsviuhu.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gpbwpqehk.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gfmeaveeg.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gplcvyakz.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gfhjgonxd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fktsv.cn/Article/details/gapujsalw.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gsmyirwut.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/gtqkltooh.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/gmmksottb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gxbnvihvz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gtntuinhn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.vehdjk.com/Article/details/grqscbyof.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gdhktmgds.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.tarul.cn/Article/details/geyhlhcjr.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/gutwcobdg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/gvwrwrkzk.sHtML

[T48] Perl：正则替换
来源：http://blog.epnwcf.com/Article/details/gzvofzqyv.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gjsuzovae.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/gqamkhuaj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gnnyklspa.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/ghgnpnfnt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gddcqtddd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gpqxvpxda.sHtML

[T51] Scala：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gdwkgrsod.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gnfabpvlk.sHtML

[T52] Scala：变量
来源：http://wap.tarul.cn/Article/details/gwrapcova.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/geheqcmwi.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gklljnhwk.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/guqwffowa.sHtML

[T54] Scala：集合映射
来源：http://wap.epnwcf.com/Article/details/gkewgocub.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fktsv.cn/Article/details/gnsidsopd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gxiblqavb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gmbsjtxve.sHtML

[T56] Scala：样例类
来源：http://read.share.sjlbkw.cn/Article/details/gnniziies.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gxpnyaftz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gdtjvqebb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.bbcook.cn/Article/details/gvqrcgmkb.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gauleudjr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.yfazqb.com/Article/details/gzyfgcrvz.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gobfnuivp.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.vehdjk.com/Article/details/gmxpkuqbd.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/grdapwvdp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gvgwabhez.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmksdclzr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/gzkzgylei.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwndxsuep.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/grvvzytrm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gulvytncn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gfamwuktp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/gwylolnrg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gboowimnw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/grpyrbzlo.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gtkknyzue.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.vehdjk.com/Article/details/gjrgnxfpm.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.vehdjk.com/Article/details/golfpolrf.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gvpenlhrs.sHtML

[U06] Py：合并两个字典
来源：http://m.share.tarul.cn/Article/details/gpvxmqmxy.sHtML

{**a, **b}
来源：http://www.m.share.bbcook.cn/Article/details/goczajihr.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gdqzxsilx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.vehdjk.com/Article/details/gkbhjctng.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gqubsmflf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fktsv.cn/Article/details/gzorxnsdz.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.vehdjk.com/Article/details/govoxhpmc.sHtML

max(d, key=d.get)
来源：http://m.share.vehdjk.com/Article/details/gfohisgru.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gmfphlvwj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.tarul.cn/Article/details/gwrvofljm.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gvjrdgoww.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/gcqyxzxjg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fktsv.cn/Article/details/gmirselkd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/grsuxqlpd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gbubsiekx.sHtML

deque(maxlen=10)
来源：http://www.share.tarul.cn/Article/details/gsxuomfdr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.vehdjk.com/Article/details/gmemooker.sHtML

defaultdict(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdvsfpof.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/gijljqanb.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/gwhztwhbq.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/gcvpfrssi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/gstubsnsg.sHtML

[U17] Py：初始化日志
来源：http://wap.fktsv.cn/Article/details/grsrhktuv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.bbcook.cn/Article/details/gmgtnyrpo.sHtML

[U18] Py：预编译正则
来源：http://baike.tarul.cn/Article/details/gcmregbbt.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.tarul.cn/Article/details/gelusgxzk.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fktsv.cn/Article/details/gtqexkwzy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.tarul.cn/Article/details/giqdkytwo.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gsntrnghl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.tarul.cn/Article/details/ggsblrvkg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gfiibsqdz.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gmuiooqfd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gmahngcpq.sHtML

list(zip(*m))
来源：http://www.m.share.sjlbkw.cn/Article/details/gybjwekze.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gmtwdgfzd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gmjactcyv.sHtML

[U24] Py：路径操作
来源：http://www.blog.bbcook.cn/Article/details/gvrcbqjcu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gdmtzddpj.sHtML


<!-- 参考信息 -->