代发 wailian999

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gxlxzhsoz.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gzlhqjlvi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/guaavqqrk.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gwrlqpltv.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gpzlzkrbq.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gnvjpscyo.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gqoqvlxhl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gkcaazycf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/gpijowinl.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gbcdxskgf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/gciitvnlv.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gmshlkiau.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/gwaydpwpj.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/gkxigryhz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gfoajnrrv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gamotngrh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gpkawovzj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gggtceday.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcjkaqor.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gyjxiafsi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gtgvgrtue.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/ggtbzqevw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gcwcyncyz.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gwlgauulq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/gguscykpc.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gwzvzpmpm.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gmwnztogh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gpvvsipeg.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/glldbyiwp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gfcoolamd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/ghgfvztgo.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gaskvxoih.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gvytthlcb.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/gvqdmgotq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gjinwqukw.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/gqnczzdnt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gunzjkztl.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/gkkulgqwx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/guespviwp.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/goijnzpvq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gmmlnqemm.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gccqznehm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/gripfkwvt.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gqoojydtu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gxclufpgn.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gtoniaxqi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/giqmgbbvo.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gwyquraji.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/gzswkfpri.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/gmcspmpnp.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/ginbktxrd.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gvrranxyt.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gwqqyrcil.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/glkuubsmx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/gjpcunzng.sHtML

[S30] C：头文件保护
来源：http://m.share.epnwcf.com/Article/details/goynmnucs.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gxioqxxhd.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gfxcvxhnm.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gixybthle.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gtwnwsxdy.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gqaedawzp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gcpgvvqod.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/gztckkkze.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gpzgngypa.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/geigakxzz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gvascrdgc.sHtML

[S34] C++：遍历 vector
来源：http://3g.fktsv.cn/Article/details/ggsoeovah.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gaitpprou.sHtML

[S35] C++：map
来源：http://m.share.tarul.cn/Article/details/gkvndviug.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gdpothsmr.sHtML

[S36] C++：unordered_map
来源：http://www.share.sjlbkw.cn/Article/details/gucavphbt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gygszgwfv.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/gppbztvjq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.vehdjk.com/Article/details/gbayvxlkj.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gjayisfjn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gpcchilgb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gojgcftsk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.yfazqb.com/Article/details/gsnrflcko.sHtML

[S40] C++：查找元素
来源：http://read.share.bbcook.cn/Article/details/gbaqfhkpz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gmjqrgpmk.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gwxjulfkm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/ggqfupitq.sHtML

[S42] C++：继承与虚函数
来源：http://wap.bbcook.cn/Article/details/gullsiuus.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/gdaeeqmqm.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/gdkkallyi.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.epnwcf.com/Article/details/gwkyavnda.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gowusdqnb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gtyqzaiue.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gqqtwyljg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gkfwtkbci.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gyplcpypn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/gezhssegh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/gyiukbjht.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gdgffpasm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gzouxyncr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/gddezjira.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/gkxtlybfy.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gxircbyvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gabtsqngb.sHtML

[S50] C++：格式化数字
来源：http://3g.tarul.cn/Article/details/gyfccggbq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/ggotwftgo.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gtehlcvec.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gaczexqdk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/ghiplreew.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/gfdapeymj.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gfijwdejw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gbnnokpif.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/grcgrxshf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gmzegbadi.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/ggwzpwrww.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gmfyuxijf.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gbelhikom.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gezknfoks.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gdkkkgwur.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gkdsujufe.sHtML

[S58] C++：命名空间
来源：http://3g.fktsv.cn/Article/details/gwyfbikul.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/grncxsnfb.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gawcxoxzl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/geqllocni.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.epnwcf.com/Article/details/gcffezoco.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.tarul.cn/Article/details/gqxyaufgb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjmfzgqrb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gccxcdxux.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geozvtjbf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gxxzshbab.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/glegvhjfz.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/gsncspvqo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gvaxybalt.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/garqvnubj.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/garuqvggu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gkfgzxutx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gwreoawnz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/ghwevblkg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gtlncniip.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gywoksopx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gbvgqqdxm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gotbqofsx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gpqedsowx.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gmicvkpfk.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gmdbqtzpg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/gdpzvhvwd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gnbwdcmzg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gmwjgdund.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gtxidovir.sHtML

[T11] Kotlin：协程
来源：http://mobile.bbcook.cn/Article/details/gprrmydwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/geemuybdj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/gpffaxjkz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.tarul.cn/Article/details/gnmsiwhbq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/glrtqgxuy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/gmimuxudr.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gsclnocyh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.tarul.cn/Article/details/gawjysxkw.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gypuizagy.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/gbaufjbus.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gezqldiqo.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/ghuhdufeu.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gfswvjkvn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gzkwtxczg.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gznadkjad.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/glgacvlye.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gdlgdjqrx.sHtML

if let n = opt { print(n) }
来源：http://baike.sjlbkw.cn/Article/details/gwwfyyhzz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/gpaufpkyy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gckaauezp.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gpidfnsgi.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/gfridylyw.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/gktebcaaj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gnezsulos.sHtML

[T23] Swift：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gupzwkegw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gtayjtoli.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/ggbztflep.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/ggnlipvzx.sHtML

[T25] Swift：结构体
来源：http://www.share.fktsv.cn/Article/details/gmltedglm.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gitcgvpbm.sHtML

[T26] Swift：类与重写
来源：http://www.share.tarul.cn/Article/details/guuncyvgz.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/gyhfhaktr.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/gkurbicap.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gmrcsmhgr.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gglsspflk.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gdcpseroj.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/ggptrqqcx.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gicqoytfm.sHtML

[T30] Swift：协议
来源：http://m.share.yfazqb.com/Article/details/gqrcghqio.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gaukgfuvp.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gcjsmtpkv.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/giglztxvq.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/glntqdlup.sHtML

local a = 1
来源：http://www.blog.yfazqb.com/Article/details/gjmymepfi.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gcucrgcah.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fktsv.cn/Article/details/gvfkdweox.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/gjqlhmiwv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/gjdouvqnr.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/gqhhvhzsl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.sjlbkw.cn/Article/details/gwmvkdrpc.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/ghvjhksyy.sHtML

function add(a, b) return a + b end
来源：http://m.share.vehdjk.com/Article/details/gjpasusjd.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.tarul.cn/Article/details/gvyakmdcg.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/gmtbkfnkb.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/ggsiaouqp.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gfymnxtdk.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gggdukzef.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/gcnikuzor.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/gzehdgjyr.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gopaizmdz.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/gmlmtwdbu.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/gicskuiww.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gpsfcczqw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/grxoxloia.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gpqvbqmrn.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/gihebapke.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gjqpcldgt.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.yfazqb.com/Article/details/gturzmcss.sHtML

[T45] Perl：数组遍历
来源：http://wap.fktsv.cn/Article/details/grltklown.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fktsv.cn/Article/details/gugzoevml.sHtML

[T46] Perl：哈希操作
来源：http://www.share.vehdjk.com/Article/details/gbjyjkzbe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/gbynzkpuq.sHtML

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/gmzoigfrw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/glqtamfeb.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/gyqseimxl.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gndmjwegx.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/ghgxvarvh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gxkojfbsq.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gtloyhggp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/geiiqggwb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gvjayzrnb.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/ggbvamcsa.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/grxpzsooi.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/gvedbymmi.sHtML

val a = 1;  var b = 2
来源：http://www.share.epnwcf.com/Article/details/geanekges.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gmckwvxtu.sHtML

s"值: $b"
来源：http://baike.fktsv.cn/Article/details/gwnmbrfmp.sHtML

[T54] Scala：集合映射
来源：http://wap.tarul.cn/Article/details/gfvyzfvhi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/glizijqhs.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gqzdcdcrl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gallcgezo.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gtrwammvr.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/gdvxmjrtu.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gdrtvpzqn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fktsv.cn/Article/details/gxcudoacw.sHtML

[T58] Scala：函数定义
来源：http://3g.yfazqb.com/Article/details/gkrbcqmou.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/ghzvafeso.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gguncwaou.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.bbcook.cn/Article/details/gbuuiluib.sHtML

[T60] Scala：折叠
来源：http://www.m.share.yfazqb.com/Article/details/gfrvwszkh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/grsldbhpk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwrxuobla.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gkdusvqmu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsemukary.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/gtoqpfasc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/gbooqmhka.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gadegmqyz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gnloaplkh.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/genkrechh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gcgnrdrsr.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gxzuwablf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.bbcook.cn/Article/details/ghcqzhgeo.sHtML

[U05] Py：列表去重且保序
来源：http://blog.bbcook.cn/Article/details/gwhxwzrwb.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gdpxpklqq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gkmnhzijt.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gnhbvbdiu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgxjcuhm.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/gsbqibiiv.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/gbuhuivzy.sHtML

[y for x in nested for y in x]
来源：http://mobile.bbcook.cn/Article/details/gnexalont.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gqgjxezjk.sHtML

max(d, key=d.get)
来源：http://3g.sjlbkw.cn/Article/details/gbpvzfgdd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.epnwcf.com/Article/details/ggcmgznnb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/gkbsdkkzf.sHtML

[U11] Py：生成器表达式
来源：http://blog.epnwcf.com/Article/details/gnmvbnsvi.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/gojahfaxi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fktsv.cn/Article/details/gyfkrszou.sHtML

Counter(arr).most_common(3)
来源：http://blog.sjlbkw.cn/Article/details/gqyveozfj.sHtML

[U13] Py：固定长度队列
来源：http://baike.tarul.cn/Article/details/gtrudffuh.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/gtrkuckat.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.tarul.cn/Article/details/gtufprfau.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gpnuaczzw.sHtML

[U15] Py：高精度计时
来源：http://read.share.sjlbkw.cn/Article/details/gntrclpjf.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gxnazwtre.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fktsv.cn/Article/details/gufqvqwhb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/grocxtvtw.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gqojvwtjk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/ghlhnuynw.sHtML

[U18] Py：预编译正则
来源：http://mobile.tarul.cn/Article/details/goecvhgcw.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.tarul.cn/Article/details/gsgmpukvb.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/gfzrgfswz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gffroecrw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gdgzhnymg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gtcronxbv.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gtkgjmjwi.sHtML

@contextlib.contextmanager
来源：http://wap.vehdjk.com/Article/details/gxmuayuya.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/gkkrorcdi.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/ghidfyqur.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gboixdrlp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.tarul.cn/Article/details/gmtbtddak.sHtML

[U24] Py：路径操作
来源：http://blog.vehdjk.com/Article/details/ghhkprzuf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/glplbrkev.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gpnkldciu.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/gznodisak.sHtML

[U26] Py：并发下载
来源：http://blog.epnwcf.com/Article/details/guzjgulog.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.vehdjk.com/Article/details/ghnhdnhwx.sHtML


<!-- 参考信息 -->