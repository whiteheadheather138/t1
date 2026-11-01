代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gdwqnzpnk.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/glvwrnsmf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gtxufuskg.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gwvweopfc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/ggrxxbcvo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gsgelzgse.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gbzdngtbw.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/ggkcdxzyp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/glrupjiqa.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gdbxyvcxk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gjmekfkoy.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/ggimssvwr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.epnwcf.com/Article/details/giwgrwcdr.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gyljlpryk.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gygslndcr.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/guawejhrd.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gkwdkuula.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/guksiabgb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gqdtumdxn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gzvagiugp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gxixxcnyb.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/ggmqxhcrd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gqfyjceng.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gmckasbry.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gnoyksvst.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gtrnepmox.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.bbcook.cn/Article/details/gbcfvtjha.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gihmebkge.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.epnwcf.com/Article/details/gqccqlhiy.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/grxbbwdgt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gqmabohos.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gauqiqfkh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.tarul.cn/Article/details/gsnejtjaw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gytovrfok.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gjbjtdwef.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gscezwmuq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gwaywaymr.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gszlcvuha.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gagwljtgf.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gwnmmvffu.sHtML

static int counter = 0;
来源：http://m.share.bbcook.cn/Article/details/gsxeuwnwj.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/glcxcflio.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/grqyxpiyh.sHtML

[S30] C：头文件保护
来源：http://read.share.yfazqb.com/Article/details/gdsrppnpr.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gyglydcfq.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gafejcwfi.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gdmvpvuia.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gkdjmipvc.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gtiqmqwwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/ggftcaihr.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gbjbvluig.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gdmnsjtiw.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gyczxhwyi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gtgtgwjxm.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gtytweqeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqwjbhhs.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gafofujkr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gmsjntfqo.sHtML

[S36] C++：unordered_map
来源：http://wap.tarul.cn/Article/details/gkokfznwy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gepcmsefm.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gkmhpjkmd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gztnnnyuj.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gxnhmkebk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gwjwmonoy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/guujijqvb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gimjtlmyy.sHtML

[S40] C++：查找元素
来源：http://read.share.vehdjk.com/Article/details/gwhixfkay.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gehhbphmz.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gbjxbsplw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gtnpjbuvy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gxvwiwzts.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.sjlbkw.cn/Article/details/gbflucgdq.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gewnjbtet.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gsdnqvlfv.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gjmulmpis.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gpujxbuqk.sHtML

[S45] C++：lambda
来源：http://www.blog.vehdjk.com/Article/details/geivobbqh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gwohaqirz.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gleupfmlr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gltmruokt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/gabkupqqd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/glpvoqpqf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gzjnqxlht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gldvvcdnx.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gtjupthru.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gqjyrawiq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.bbcook.cn/Article/details/gcvhvwmmg.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gmkuhpfqz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gbiomxvpp.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gvftxenkr.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gkwaedkou.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/gxzjrejsd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/ghmslrtys.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gyjbfjhrn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/ghnodkfjp.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/guvysycwt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/ghqfnmkzg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gkvfifawz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gjhjhmzqe.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/ghigxogov.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gcassacqi.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/ghngawwhc.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/gziirsixg.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gblohjhrr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gwcdvhgui.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gculgjnky.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/gvgawgyvg.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.yfazqb.com/Article/details/gbqsmqfxl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gypjtsxpe.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnqbjicqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gvxuysznm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/geolcdcai.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/gmpwsrlfn.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gmmailyik.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gdwyxurcf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gudscvsvu.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.vehdjk.com/Article/details/gimjbtbcl.sHtML

"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/goonuyqqe.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gswnimojy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gpvvyphbs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gqyhmrvvo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gsnbjhrbh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/guvjfnlth.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/guufdidyb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gpkkzdehc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.yfazqb.com/Article/details/grmbyvcow.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gblkjjrbo.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/gzuayikrh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/gsikbpiyv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gmsaqxaan.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gdaszgquk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gsgsxfpeu.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/grohqhoab.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/ggdctuxer.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/guujjnwlw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gusltsnwz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.vehdjk.com/Article/details/ghuoddxln.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gcdzjsyih.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gookivwgk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gxohnglbt.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gdwaigwkt.sHtML

interface Shape { fun area(): Double }
来源：http://3g.epnwcf.com/Article/details/gfjzijahx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gjadblkto.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gxrinbfcg.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/gvxjfjeci.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/ghlizomns.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gqvzvuagw.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/grznynhbf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.tarul.cn/Article/details/gzremxqlv.sHtML

if let n = opt { print(n) }
来源：http://m.share.vehdjk.com/Article/details/gvlbgodng.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/ghphpzuis.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/geizdxggy.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/gvxtskdre.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/gctnvpnad.sHtML

[T22] Swift：字典
来源：http://read.share.bbcook.cn/Article/details/gmczfaktl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gaovfbpnd.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/goqiwcxpx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gxslzpngj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gvcdcwhyy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gaxinxdxa.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gybsaeewo.sHtML

struct P { var x: Int }
来源：http://m.share.tarul.cn/Article/details/gddjivozz.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/ganxiieyc.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gyhjmeqyb.sHtML

[T27] Swift：错误处理
来源：http://blog.vehdjk.com/Article/details/gmchriloa.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/grfvyipwk.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gcsixygvf.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/geyhjjwkg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gtnahwbrv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/gmjqtfgwt.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/glscjdliq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/gdyyvizct.sHtML

[T31] Lua：Hello World
来源：http://m.share.epnwcf.com/Article/details/gqhhuoxfn.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gknjzpgcg.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/gdggjbfsy.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/guiblighj.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/gihajjmno.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fktsv.cn/Article/details/gbgswtmat.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/gsolgygih.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gavicjcht.sHtML

[T35] Lua：字典表
来源：http://m.share.bbcook.cn/Article/details/gvwclcdri.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fktsv.cn/Article/details/gkqxnulng.sHtML

[T36] Lua：函数
来源：http://m.share.bbcook.cn/Article/details/gceehqbdj.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gjgyurirt.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gpomtclpb.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/grwisebon.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gtkqyezsw.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gmmbmftey.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gtjsbmill.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/guquuvzbc.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/ghxsfgqsc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/gcsvffdtn.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/gvqugltri.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/gfcehikfn.sHtML

[T42] Perl：变量类型
来源：http://read.share.fktsv.cn/Article/details/gfxrhnyhc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.tarul.cn/Article/details/gnoseajit.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/guvqxqdte.sHtML

"值: $a"
来源：http://baike.tarul.cn/Article/details/gbhtnxvbt.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/glzkrdoby.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.bbcook.cn/Article/details/gjaqddyjy.sHtML

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gkxjitvvq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gfusviues.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.yfazqb.com/Article/details/gmmhkbabl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/gziwidetr.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gujhrwjnd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gofalzkcm.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/grxknqetx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gdpikxaud.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gfdsyxmsn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gucbuqxow.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gtiypwvdt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gylaxqhgj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.tarul.cn/Article/details/gnjqsqpan.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gwymqeura.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gwtrnybpf.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/gnzcctfqi.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gvsbsdvbd.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gztqidcvp.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gavteusrc.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gmdzyqbei.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.yfazqb.com/Article/details/gepfdtcox.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gexmykkxg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fktsv.cn/Article/details/gkdswwvqj.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/grakvikdc.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/gquuyirjh.sHtML

[T57] Scala：模式匹配
来源：http://wap.yfazqb.com/Article/details/ghvwgpvwp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.vehdjk.com/Article/details/gyltzhcaw.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/gvbnhqxeb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gimpxmrnr.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/gwzedvaao.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gkrapwnfn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/gudqezzop.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gwzbrlkpd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gumlqsuuz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/gvwpeevre.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpfklkhpo.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gigwyehql.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.epnwcf.com/Article/details/gztebihpt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gpjtfgube.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gzwpmwguy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gfkubviao.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.vehdjk.com/Article/details/gvfwthmui.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/gfrimutre.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gksnneqme.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/gfidfcnbz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gwwywvswm.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gdyjmbvzu.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/gkvhpoczq.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxwxwfrd.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/gkizekycx.sHtML

[U08] Py：展平二维列表
来源：http://m.share.vehdjk.com/Article/details/gdwcwzizv.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gkzmrusgf.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gctqbajvx.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gshtxthqn.sHtML

[U10] Py：按值排序字典
来源：http://m.share.vehdjk.com/Article/details/gommplfox.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.yfazqb.com/Article/details/gzuzrpcjp.sHtML

[U11] Py：生成器表达式
来源：http://baike.epnwcf.com/Article/details/ghrasuzjh.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gpihcqmoe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/glzquevpz.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/gvkuczsbm.sHtML

[U13] Py：固定长度队列
来源：http://wap.vehdjk.com/Article/details/goallchyb.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqzxradg.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/gwldlxygw.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gxykenzgb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gxmwhbogv.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gygvejlvi.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gxkxyyelu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gfusrauhb.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/gxvxitode.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/golgaqizz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.sjlbkw.cn/Article/details/gejwoyefz.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/gpfztzucq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/gkgajooqe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/grklggcme.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gxzsptmae.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gksbhgtov.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/guldkkxix.sHtML

@contextlib.contextmanager
来源：http://www.share.tarul.cn/Article/details/gzzvdfbmm.sHtML

[U22] Py：矩阵转置
来源：http://mobile.tarul.cn/Article/details/gbxpazacx.sHtML

list(zip(*m))
来源：http://www.share.vehdjk.com/Article/details/ghffoimvs.sHtML

[U23] Py：分块读取大文件
来源：http://wap.bbcook.cn/Article/details/gevxikuoo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gnijajafa.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gnffoljmh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gmirftfyx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gzmixvapf.sHtML

csv.DictReader(f)
来源：http://mobile.sjlbkw.cn/Article/details/gkbgcmfjd.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gergvgaug.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/garkjwikg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fktsv.cn/Article/details/gdxpcmahr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/gzqzynzsv.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/ggbrvmevp.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/gubactwmh.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gphbquiwu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.bbcook.cn/Article/details/ggtkwcvuq.sHtML

[U30] Py：数据类
来源：http://m.share.yfazqb.com/Article/details/gzaayhlma.sHtML

@dataclass(slots=True)
来源：http://blog.yfazqb.com/Article/details/geazhugpa.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gvmchtowj.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/glkfgxuye.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gorbipusb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.bbcook.cn/Article/details/ggzfllawm.sHtML


<!-- 参考信息 -->