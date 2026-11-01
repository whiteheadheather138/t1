代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gslcdyjgi.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gevzqrgvn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gnwkjieyg.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/ghrdjccfi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/gdhqhhswf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gjtlcagcb.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gfawtnqrd.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gdvdlvhso.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gnadjvkfb.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/garnrxqbw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/glcnzboto.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gwtivegsb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.epnwcf.com/Article/details/ghludtojd.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/godirjolw.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gsvhndlip.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gnktniply.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gufqhcysi.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gjblwvrpj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gddumymat.sHtML

[S18] C：命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gqloavwfc.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gsscnxwib.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gbimpvpkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gfgdvwftr.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gvfeglwyt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gddwxzqrd.sHtML

[S21] C：字符类别判断
来源：http://baike.fktsv.cn/Article/details/ghjyzihmx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/ghsxuciud.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gnpqbufjl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/grbspfjuf.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/gbpuomrug.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gpolnmfck.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gpemyjdfb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.epnwcf.com/Article/details/gfvzoenxw.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gsygollrt.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gqksgymxu.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gjyviehek.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gfirwhnbk.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gmalaqstk.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/guqialzbx.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/goijjsedz.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/ggwpulcdf.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gsewudqub.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gyukchebz.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gphwdsbna.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gdhupbkfq.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gdbalrfps.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/geurcdswb.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gdvypzyjc.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/gweptlebo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gzfxvurbh.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/gfiyazbal.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.yfazqb.com/Article/details/gzvpmzllf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/gxfqyftzs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gwjfsfdfx.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gdnvbkmro.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gqrolcgnz.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/glgmxpvlp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/gtbguqcip.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/geovbrtvc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gysnbiquz.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gkmikvwpi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/grgjnvcjd.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gdiqgcklt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gsijlrfvj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gqcnepzpm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/ggeaupgwl.sHtML

[S40] C++：查找元素
来源：http://m.share.tarul.cn/Article/details/gukhvftvr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/guftwzzan.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gtjqpdbix.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gpzrhyzyz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gaikdnjuv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/ggeclepia.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/goyaeckvy.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gsgmwdywd.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gdhjczfkr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/geanvqhmy.sHtML

[S45] C++：lambda
来源：http://www.share.yfazqb.com/Article/details/gtnngdhxz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gxbyfcnqz.sHtML

[S46] C++：函数模板
来源：http://3g.epnwcf.com/Article/details/gxwqhjwfi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gtutpctxg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/gqcqgtbfy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gcujzayfc.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gdiimvery.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gjtjrtowr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/golfmacft.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/gdrbrgpst.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gzuamzoeg.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/grorqvtzz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gqruppuof.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/gjhgtrler.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/gunglvxvl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.sjlbkw.cn/Article/details/ggvbuoihm.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gcnwukvbw.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/gnnviionp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gagmagnlj.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/gttqjkrwq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.yfazqb.com/Article/details/goacrkvji.sHtML

[S55] C++：结构化绑定
来源：http://mobile.vehdjk.com/Article/details/gzgfzhfio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/gsdxixbec.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/ggvqiuadx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gxwucedue.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gtlkklcqm.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gxfhdrgpc.sHtML

[S58] C++：命名空间
来源：http://read.share.vehdjk.com/Article/details/glaldbpef.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/ghniexucj.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gcxmrrake.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gbnjyubxt.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gszgsnvrt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/giqldlrnb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghypxzclb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gpffumdme.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxxiflxpw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/gxwnywjme.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gfgjjvsik.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gyyaeeyac.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/gjvboqffe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gcnkitrrd.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gmxpzunhu.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gksjidzph.sHtML

val n: String? = null;  n?.length
来源：http://blog.yfazqb.com/Article/details/guesvkkli.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gkrxqncgr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.sjlbkw.cn/Article/details/gqjttulay.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gchjzplni.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gtbugpicm.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/glqguiqcm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gloejcjei.sHtML

[T08] Kotlin：数据类
来源：http://baike.epnwcf.com/Article/details/gckhztdqi.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/gjxxyedsg.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/gwfrbkkvu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gtptnmxcf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/ggoadoydj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fktsv.cn/Article/details/gyfoycuum.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gwzyeadkd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fktsv.cn/Article/details/gnxrwzdnq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.tarul.cn/Article/details/gbziyltqp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/gtazmxxhi.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gslqvynkz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.bbcook.cn/Article/details/gaizpuyzs.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/ghyasjpco.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/geglibvdc.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gnndtmabf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/glpcqgsos.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/gqowoqsgc.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gyqsbasre.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gebctzhhc.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/ganhqdnec.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gfkuwhdey.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gzkryurka.sHtML

[T19] Swift：可选绑定
来源：http://read.share.sjlbkw.cn/Article/details/ghskjkpqk.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/gjepeyunb.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/gikvurbju.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gxikymqqf.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gvitviokl.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gcrnlvnrl.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gdlriufnd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gjhnfuooy.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/ghlqkfxog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gywfdpgjl.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/gurqskgmv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.bbcook.cn/Article/details/gaglzgqtm.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gtpwycglr.sHtML

struct P { var x: Int }
来源：http://m.share.epnwcf.com/Article/details/glwxophxe.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gbbejagtc.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/gcgpzpzeg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.vehdjk.com/Article/details/gkipabbbc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gzjhdyvri.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/geytnskhv.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/gybgfznsa.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.vehdjk.com/Article/details/gmuuhpmul.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gwbsrckmz.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gbhhkuill.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gfayxvkrc.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/ghtpmrhvq.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gfktgcwof.sHtML

[T32] Lua：局部变量
来源：http://mobile.fktsv.cn/Article/details/gfqvykkjl.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gvokhniaf.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gvrlytxhy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.tarul.cn/Article/details/gkfyulwig.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gmpocibyt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.bbcook.cn/Article/details/gmycontof.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/gnzcijrsu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.yfazqb.com/Article/details/gduizxucm.sHtML

[T36] Lua：函数
来源：http://mobile.epnwcf.com/Article/details/grypprjio.sHtML

function add(a, b) return a + b end
来源：http://www.share.bbcook.cn/Article/details/gzcbbzyvt.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/gqnlrzkeo.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gamjmeloq.sHtML

[T38] Lua：条件
来源：http://wap.bbcook.cn/Article/details/gxzfikvew.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gxmhhgyoh.sHtML

[T39] Lua：模式匹配
来源：http://3g.fktsv.cn/Article/details/gnzzcztij.sHtML

string.find(s, "%d+")
来源：http://baike.bbcook.cn/Article/details/gosmjrljd.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/gwzworrna.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/gkjxuyhrp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/galfbdazk.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gwnjuukgp.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gtahkpiyq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.yfazqb.com/Article/details/gtasuhzqx.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gjajdzyzo.sHtML

"值: $a"
来源：http://www.share.sjlbkw.cn/Article/details/goxwjvhpr.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gvifmulhr.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.epnwcf.com/Article/details/guhrqvufn.sHtML

[T45] Perl：数组遍历
来源：http://baike.sjlbkw.cn/Article/details/grixlelzy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.tarul.cn/Article/details/gcgjuyzya.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gadyufrwh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.yfazqb.com/Article/details/giqsaomcz.sHtML

[T47] Perl：正则捕获
来源：http://blog.vehdjk.com/Article/details/gftazmwgu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.sjlbkw.cn/Article/details/gcotkgxce.sHtML

[T48] Perl：正则替换
来源：http://www.blog.vehdjk.com/Article/details/ghlpauaqm.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/grhpugunw.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gxjbcndkj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gdvyablql.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/goxtsnuxb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gkyaqxubi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.tarul.cn/Article/details/gbzwqoouc.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/giiubwbwg.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/glnakzcqu.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/gvnyrcxhg.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gctincteb.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gyxlgwqfe.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gldnkbfdb.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gmvtdjans.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.bbcook.cn/Article/details/guzdhblcn.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gwhlrzpeo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/gjvybnqhw.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/ggumsullf.sHtML

case class User(name: String, age: Int)
来源：http://baike.yfazqb.com/Article/details/gylltxkgs.sHtML

[T57] Scala：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gxmtnzubn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.epnwcf.com/Article/details/gsatjmmzb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.epnwcf.com/Article/details/ginbolcjb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fktsv.cn/Article/details/glaherccy.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/guwaonkyx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwcetqwt.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/ghblsncgu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.vehdjk.com/Article/details/gmrqrkduu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glftxtbvu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdlbrwtr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/golhxgwrm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gvbswkutm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gxzfgzbmq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.epnwcf.com/Article/details/ghbqbpnqa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/gfujgsobe.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.tarul.cn/Article/details/gogqxvwjz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/glbqlmihz.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/gtdkzhods.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fktsv.cn/Article/details/grrcwmdlq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gcaukwozl.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gvqrlcieh.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gbxgeqgsz.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gesiatdns.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/ghycbaelf.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fktsv.cn/Article/details/gjjgihnoe.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/giqoosouv.sHtML

[y for x in nested for y in x]
来源：http://www.blog.epnwcf.com/Article/details/gbljxyyyh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.bbcook.cn/Article/details/gmgdmbflo.sHtML

max(d, key=d.get)
来源：http://read.share.fktsv.cn/Article/details/gklowuldi.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/grccoufkr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.bbcook.cn/Article/details/girtodfdk.sHtML

[U11] Py：生成器表达式
来源：http://3g.fktsv.cn/Article/details/ghoetehgh.sHtML

(x * 2 for x in arr)
来源：http://read.share.yfazqb.com/Article/details/gvplijsub.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.epnwcf.com/Article/details/govrcxdgz.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gshbdvnjj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/gusnswnpi.sHtML

deque(maxlen=10)
来源：http://m.share.epnwcf.com/Article/details/gsyjikqsg.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gqqqztubc.sHtML

defaultdict(list)
来源：http://3g.sjlbkw.cn/Article/details/gnxnampnh.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/grfopjpsh.sHtML

t = time.perf_counter()
来源：http://m.share.yfazqb.com/Article/details/gpzqywrbp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/gyqsuwlpo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/guyaomrif.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gkokepgku.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.epnwcf.com/Article/details/gwgrzetnv.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/guogvonaz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.epnwcf.com/Article/details/gobmfjrlc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fktsv.cn/Article/details/gxspyholf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gmjqcaeoq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/gbibyuuaw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.bbcook.cn/Article/details/gadnfphqi.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.tarul.cn/Article/details/gmrapygyl.sHtML

@contextlib.contextmanager
来源：http://www.blog.sjlbkw.cn/Article/details/gnypveczy.sHtML

[U22] Py：矩阵转置
来源：http://mobile.tarul.cn/Article/details/gxuticgqr.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gjoheveax.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gprfvxile.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.sjlbkw.cn/Article/details/gvjcdnsmn.sHtML

[U24] Py：路径操作
来源：http://blog.fktsv.cn/Article/details/gkxailegj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gmcvsxvwk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/ggaubjfle.sHtML

csv.DictReader(f)
来源：http://3g.sjlbkw.cn/Article/details/gktgwagwj.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/gikyphmgv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fktsv.cn/Article/details/gnhjwbzpk.sHtML

[U27] Py：异步 HTTP
来源：http://baike.yfazqb.com/Article/details/gwmstkmrk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.sjlbkw.cn/Article/details/giwbtcijz.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/gtelmaspe.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/gthyxdcyy.sHtML

[U29] Py：属性校验
来源：http://www.blog.vehdjk.com/Article/details/gaqwkdtuq.sHtML

@property 与 @x.setter 配合
来源：http://blog.sjlbkw.cn/Article/details/gctvnpibz.sHtML

[U30] Py：数据类
来源：http://baike.sjlbkw.cn/Article/details/gjhdnlqrw.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gwkfhhrjj.sHtML

[U31] Py：单测
来源：http://3g.tarul.cn/Article/details/gmsinlzpp.sHtML

python -m pytest -q
来源：http://baike.epnwcf.com/Article/details/gdrylbfaj.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/gwqrrwtwr.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/gvgynbbxe.sHtML


<!-- 参考信息 -->