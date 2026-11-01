代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.tarul.cn/Article/details/glqseaibe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gmrzcuouq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/ggfazspqy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gzwhinkmi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gfxkuyalk.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gmezqvasd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gpsgdqbhx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gqkbdcgof.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/guxdkoraq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gktmldepi.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gkaqbyykd.sHtML

[S12] C：写文件
来源：http://baike.yfazqb.com/Article/details/gwldnoxyc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gojgtoqqw.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gliitotsf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gydizhfjh.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gdijjmzaz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/ghmquiqso.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gurwfnrvk.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/gyxqcluua.sHtML

[S16] C：位操作置位
来源：http://www.share.fktsv.cn/Article/details/gfqjtfnqt.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/geprpxdvb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/ganzanlfn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gwpkdijxg.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/gvsrbjbnv.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gkaqpykqi.sHtML

[S19] C：快速排序
来源：http://m.share.fktsv.cn/Article/details/gsaxuxowf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gouhqmidh.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gikroznck.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gziapdtti.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gzeecykig.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gupklolbe.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gvghkwter.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/glkphdths.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gwoveohog.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gvzhqwmqr.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gyblzeuzz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/garjfqqjq.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gguzqhcxj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gbpgpucdu.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/gjiwierro.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/gtwuhlrbc.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/ghrnbzxdp.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gsjntqwhe.sHtML

[S28] C：静态变量
来源：http://www.share.fktsv.cn/Article/details/ggupwivnw.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gywibylei.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gqxbczldo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/gnjbxbbiw.sHtML

[S30] C：头文件保护
来源：http://read.share.vehdjk.com/Article/details/gtlelgmtu.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gwgtresku.sHtML

#define X_H
来源：http://mobile.epnwcf.com/Article/details/gbnduoazv.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gsowsiulz.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gmkndaoga.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gxxexrgpt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gabfkqcrv.sHtML

[S32] C++：字符串
来源：http://mobile.fktsv.cn/Article/details/gtzsshkxq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gebmrnivv.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/glnekivcd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/gjxxkbipv.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gubkdquud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/gucawcodo.sHtML

[S35] C++：map
来源：http://baike.tarul.cn/Article/details/grouivbqv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gvjeueint.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gtwategew.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gxjpqtfik.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gqbsmhlvg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/gicpwbjzg.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gszgtqtjz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/guyeodlmn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.vehdjk.com/Article/details/gsvmgozth.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gajduqjsv.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gzbnryjhp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/gsdmftenp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gbkhpxxqv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gtomhbnjw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gjsilxmkj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gzxqirmnr.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/guxtiumwl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gpvthsihm.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gewnicqml.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gxgjvciof.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gbxglqixp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/grqropllk.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gcwqyojuo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gwoclffne.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/gcijaxvjm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gjwsjnzzc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gtapaxgzz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gdxrfjwjl.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghejjlfxk.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gzfxylird.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gicyhkilh.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/grpcptcio.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/guhyxjfqy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/grptuonxa.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gxudnujjz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/ggbqcoucs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gbbnlcrio.sHtML

[S53] C++：移动语义
来源：http://3g.fktsv.cn/Article/details/gojejfpon.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gvygydjon.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gwbmbggoa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.sjlbkw.cn/Article/details/gekavycit.sHtML

[S55] C++：结构化绑定
来源：http://blog.yfazqb.com/Article/details/gqobznxee.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gkkjyxdjx.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gvqegywlg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/gtfqodvml.sHtML

[S57] C++：编译期常量
来源：http://baike.tarul.cn/Article/details/gjicjtdwa.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gogfzgien.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gljvlhnph.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gvsvwpjde.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gudmjpqid.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gtyrqmbnl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/gxebzkdkf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.bbcook.cn/Article/details/gnhmywqem.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grjizgiwu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gewbigmbg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvtfxfroo.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gpuflrpmf.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/ghxcrkhhf.sHtML

[T02] Kotlin：变量
来源：http://read.share.sjlbkw.cn/Article/details/gthplgdjt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gbdfjnxhf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gzlcuzvzc.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gqvixggsc.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gdaoumpuo.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/gmvavilul.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/gzsagreev.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gonrnavhs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/ghuwswpxb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gvbyrznhx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/glbfrwvts.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gsfvugdcm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.bbcook.cn/Article/details/gmegeuqua.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gsadpicca.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/grwndttjy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/guzayzqwp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gnbyiwqci.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gwdtvrypa.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gvxtqgpoo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gspuhjsii.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.vehdjk.com/Article/details/glnmsiftk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gevkwfihv.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.tarul.cn/Article/details/gahucgztf.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/gehuiapad.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gnitjeczj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.epnwcf.com/Article/details/guijbspqk.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gniibezqs.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gggdipatl.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/ghtomioiw.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gnygllnnl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gdxmwfgye.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/geqdqqlzn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gsfzmszpf.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/ghcwzvtpm.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gyzxjurmh.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gkrqmwcmf.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gnzmswknz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gmjebxznm.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gymxaxxxt.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/gvwbshxdu.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/gsavutlrz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/gylqzvhaf.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/gvleycvpt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.epnwcf.com/Article/details/giastqaoy.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gfazcbold.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gztuwceas.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/guswnutcg.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/grqleukyf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/gahtxnjvz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gibzvjsef.sHtML

[T27] Swift：错误处理
来源：http://www.blog.yfazqb.com/Article/details/glestvnpi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gjpksikvp.sHtML

[T28] Swift：枚举
来源：http://read.share.vehdjk.com/Article/details/ggltqxlfj.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/geoolocds.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/gutnpbmpt.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gkbtqvjau.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gfzjmdzji.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/ghuzltppz.sHtML

[T31] Lua：Hello World
来源：http://wap.yfazqb.com/Article/details/gcjvatmmh.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gjrumwvyi.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gijkjbxrz.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/ggohvpsmm.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/gtbejtzmv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gvmjpivbx.sHtML

[T34] Lua：遍历表
来源：http://www.share.epnwcf.com/Article/details/gyqqjcrpo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.vehdjk.com/Article/details/gpmesszyv.sHtML

[T35] Lua：字典表
来源：http://blog.yfazqb.com/Article/details/gdbghlbui.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gqmwrcwfn.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gmhjfogqn.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/geayjlddx.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gugzhkuml.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/gmgwfxfqt.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/glrwrulce.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gbgcncfih.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gyaepczbf.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gfbgdwumj.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gkorbctfc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/gmiivyoud.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gyuzprmuc.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gbufsouvd.sHtML

[T42] Perl：变量类型
来源：http://www.share.epnwcf.com/Article/details/gayrrtfjg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.bbcook.cn/Article/details/gvlpjffoq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gynjzbtvh.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gpvbuyupi.sHtML

[T44] Perl：条件
来源：http://read.share.vehdjk.com/Article/details/giqhuoqip.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.epnwcf.com/Article/details/gincounuj.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gnvbzmtma.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/ggilrqbaq.sHtML

[T46] Perl：哈希操作
来源：http://3g.sjlbkw.cn/Article/details/gqeocjklp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gnudlbncf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gjflatpnm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmfupdbt.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gpatzlbdj.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/grlsaitla.sHtML

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/ghyeutopy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gcjrsvdgf.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gfxbusiur.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gqokzmwmu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gymfmviva.sHtML

[T51] Scala：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/geyzpfevs.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gyryoyird.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/glmdzezbo.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gkmpfazfi.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gadbvmmzt.sHtML

s"值: $b"
来源：http://3g.yfazqb.com/Article/details/gvrjcloth.sHtML

[T54] Scala：集合映射
来源：http://blog.epnwcf.com/Article/details/goebbisqc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fktsv.cn/Article/details/gsbxfdorx.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/gooobfogl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gjevooypt.sHtML

[T56] Scala：样例类
来源：http://mobile.epnwcf.com/Article/details/gpqlhpfub.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fktsv.cn/Article/details/gayzwxibm.sHtML

[T57] Scala：模式匹配
来源：http://3g.vehdjk.com/Article/details/glfzffzlq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.tarul.cn/Article/details/ggrdfeitz.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/gdigwxitb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.bbcook.cn/Article/details/gayiirdzs.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/gtokhltet.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gdwssrmqp.sHtML

[T60] Scala：折叠
来源：http://baike.tarul.cn/Article/details/givgtcxrb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fktsv.cn/Article/details/glwyrdoee.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmraegiiu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/gjfdptjnp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggfxdavot.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.sjlbkw.cn/Article/details/gygpwxbfy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gclwssdbs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/gcliylumh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fktsv.cn/Article/details/gufkpuhll.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.yfazqb.com/Article/details/gheglsbta.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.epnwcf.com/Article/details/gwmzbwiye.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gjljxznrt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fktsv.cn/Article/details/gpzdauvle.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gsbbkucdo.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gpnxagucv.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gpgflcoql.sHtML

{**a, **b}
来源：http://3g.bbcook.cn/Article/details/gydmqxkng.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.tarul.cn/Article/details/gwoljjqkv.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.bbcook.cn/Article/details/gllhwvktk.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.bbcook.cn/Article/details/gwowkbjcq.sHtML

[y for x in nested for y in x]
来源：http://blog.fktsv.cn/Article/details/gmexvyghi.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.yfazqb.com/Article/details/gdavrddnz.sHtML

max(d, key=d.get)
来源：http://read.share.sjlbkw.cn/Article/details/gvplkiyqn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gbiybcqno.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.vehdjk.com/Article/details/grbyuzkxi.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gfpwohqcx.sHtML

(x * 2 for x in arr)
来源：http://read.share.tarul.cn/Article/details/gqrrigdtp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gwejeroio.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gjobxpqrr.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgsbixgm.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/gxpjxjlmo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/gltgecvlx.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/ggdlpdopn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.sjlbkw.cn/Article/details/gyuuuklqh.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gicjsvldo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/gudqhkedl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.vehdjk.com/Article/details/gbkfnggkq.sHtML

[U17] Py：初始化日志
来源：http://m.share.vehdjk.com/Article/details/gsfolvnix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gbcafmysx.sHtML

[U18] Py：预编译正则
来源：http://www.share.yfazqb.com/Article/details/gaftnfbot.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/gixrbpauj.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.sjlbkw.cn/Article/details/gwzckhffi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/ggrnajvzo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gnrlzbzlw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gztlfeagu.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.bbcook.cn/Article/details/gpzkjxgcz.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/gikziuxek.sHtML

[U22] Py：矩阵转置
来源：http://m.share.sjlbkw.cn/Article/details/gbwvepvoy.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gtctjjsbj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/gdlyvxukl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgewzsfe.sHtML

[U24] Py：路径操作
来源：http://m.share.bbcook.cn/Article/details/gvvbjpgau.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gixsatmms.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fktsv.cn/Article/details/gltforwjx.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gannfnlsc.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/giuhosyhu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/gzxdxugwg.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.bbcook.cn/Article/details/gspmjfcly.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/ghxtqjsup.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/gtbycqrxe.sHtML

UserId = int
来源：http://read.share.sjlbkw.cn/Article/details/gozpkrvno.sHtML

[U29] Py：属性校验
来源：http://www.m.share.yfazqb.com/Article/details/gndufgclf.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fktsv.cn/Article/details/gjnkarphp.sHtML

[U30] Py：数据类
来源：http://www.blog.fktsv.cn/Article/details/gqkhdutkl.sHtML

@dataclass(slots=True)
来源：http://www.share.sjlbkw.cn/Article/details/gcxlodwzx.sHtML


<!-- 参考信息 -->