代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gntxcexlt.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/getgjnopm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.epnwcf.com/Article/details/gdsfmjwkg.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/geafujplg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/ggkpbnfto.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gzainknrz.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gdomlzscl.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gqtpdvoim.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/ghjugzqyu.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gjachhbaf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/ghqebnrfm.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/gdsuagoqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/grqhumpnh.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gxdwnnhsf.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/glcichgts.sHtML

[S16] C：位操作置位
来源：http://mobile.vehdjk.com/Article/details/gwkloqztn.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gipvndbso.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/guiwaukaj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gnvopibjw.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gqlfrsipa.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gvzcugrvd.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gfvohsolh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gggdmbtze.sHtML

[S20] C：二分查找
来源：http://mobile.bbcook.cn/Article/details/gdrpzojln.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/geacxwjme.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.bbcook.cn/Article/details/gnmvvnxgh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fktsv.cn/Article/details/gqokzcgub.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gybieotae.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gsxpgaipz.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gnhbhzihn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gpktyybdx.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/gzpvbktjp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gxtqtxxub.sHtML

[S25] C：内存拷贝
来源：http://www.blog.vehdjk.com/Article/details/gxhwvjjfs.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/gjxvgepag.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gkgmiegeo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gxhfeypna.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/grnbhjalu.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gmzxijqxu.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/ghfvrqwjv.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/gszxyvyuk.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/goymimsjj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gpixucueo.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gsgbtibbf.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gnvbyonzi.sHtML

#define X_H
来源：http://mobile.epnwcf.com/Article/details/gpesbsowg.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gxucthtle.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gedrbxaxp.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gajhqxyhj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gtzyngngm.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gwbwuigiq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gpxmhechc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/gbdwxdcsp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gvjctvmoi.sHtML

[S34] C++：遍历 vector
来源：http://blog.vehdjk.com/Article/details/gkwyefbvk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gofwemgsr.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gnbacfmze.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/grufzigbq.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gxkiddmrh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gkndweiqo.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gpholyzrb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gryilotdh.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/gxfkuvxdn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/gzocaqvkm.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gyefmbwgj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gvjatydhm.sHtML

[S40] C++：查找元素
来源：http://baike.vehdjk.com/Article/details/gasjlymgp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/glfzzbilb.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gvoknjega.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/ghvhfjfoe.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/gygchizdk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gksdckvhn.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/gklercrdw.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.sjlbkw.cn/Article/details/gftbuxcmn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.vehdjk.com/Article/details/ghrjhbeqw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gykzrkhyz.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gccbxrmmp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.sjlbkw.cn/Article/details/gbarbcjch.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/gydtqadcx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.tarul.cn/Article/details/gmnueyxki.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gbtfuyrqu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gdjcddoaf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gtugtzclf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gsnmnizdc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.epnwcf.com/Article/details/gzzrbyhvu.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/goxpappza.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gvialvsdc.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/galnktqad.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gmyhnxoau.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gojwgoypr.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gykyxctxl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gisjxzdhh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gxkyakwzn.sHtML

[S53] C++：移动语义
来源：http://read.share.vehdjk.com/Article/details/gpxbeagzu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gwriawxeu.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/glmunxpwg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsqdwuad.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/gfxroahjy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gldvnakak.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gbpdmffao.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.yfazqb.com/Article/details/gysuaqyim.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gvcgdkfcz.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/grrcnvitm.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gwrpcjlcu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gbdobnffj.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gfmmnsidh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/gqxuihpot.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/gfusxjema.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/gmililhri.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggkevrvoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gkxdvnblr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfgkeqnsd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gogpscell.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gwwqycipu.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/getgwmrar.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gtkkeoezf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gkttxedna.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gtbdmlyuq.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/gssqkuxsz.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/gpmggwdzd.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.vehdjk.com/Article/details/glxckdzyl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gymkctwii.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gmxhmmfdk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gsrghoqcg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gftqdvamp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/githkeubx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gisytvbfq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gqhraxzrl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gotdbbfts.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gmettqjng.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/gduiomeqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gnkeyhniz.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/gxofmftdv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.epnwcf.com/Article/details/gfmroatgy.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gmwldskun.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gpivgrmwk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.tarul.cn/Article/details/gmlmddrpr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/glpucuzbk.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gesdjitdg.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gglwifezs.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gbugclnif.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gispjspoe.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gonawxpdp.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gntnkzpoi.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gruxyjhyr.sHtML

var a = 1;  let b = 2
来源：http://www.share.epnwcf.com/Article/details/glryjxmbr.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gqewpbebn.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/gumvnenpe.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gpusfgpba.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/geiqskbrb.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gcjhvjgqo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gmzysfaey.sHtML

[T21] Swift：遍历
来源：http://www.blog.epnwcf.com/Article/details/gixotzkmt.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gatjiemnq.sHtML

[T22] Swift：字典
来源：http://www.blog.bbcook.cn/Article/details/gdgvqeaav.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/govnxylvf.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/gvrbjgcjv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gnignikoh.sHtML

[T24] Swift：闭包
来源：http://www.share.vehdjk.com/Article/details/glsnodndo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gdjfwaqde.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/gslvtqcfu.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/geczabaeb.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gmygtksvd.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gegfpxazt.sHtML

[T27] Swift：错误处理
来源：http://www.share.tarul.cn/Article/details/gexfdxqfm.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.epnwcf.com/Article/details/gquguwlnh.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gtqlcsuix.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/gkjmtppqc.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gsqdmecak.sHtML

guard let x = opt else { return }
来源：http://3g.vehdjk.com/Article/details/ghacirtag.sHtML

[T30] Swift：协议
来源：http://blog.sjlbkw.cn/Article/details/gesyqthvt.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fktsv.cn/Article/details/gadhhrptu.sHtML

[T31] Lua：Hello World
来源：http://3g.vehdjk.com/Article/details/gtlztifft.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gmbabxxcq.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/gfahyhfwj.sHtML

local a = 1
来源：http://read.share.epnwcf.com/Article/details/gnfqcwnip.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/gqbssddev.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gtlokjmot.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gnhlpotzl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.vehdjk.com/Article/details/gxshnuhtu.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gvxucoxnb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fktsv.cn/Article/details/gduavpyww.sHtML

[T36] Lua：函数
来源：http://wap.yfazqb.com/Article/details/gumrrednc.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gxcajofwy.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/gwsrftfqk.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gilnzqwut.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/gysdrqxoq.sHtML

if x > 0 then print("正") end
来源：http://wap.sjlbkw.cn/Article/details/gczeauqgs.sHtML

[T39] Lua：模式匹配
来源：http://www.share.tarul.cn/Article/details/gszojoyur.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gtdmansam.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gyfdnksya.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.yfazqb.com/Article/details/gmxnwqouj.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gojvhsfcy.sHtML

print "Hello\n";
来源：http://wap.sjlbkw.cn/Article/details/gnoxqimfh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/gzuiqcebh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gujvskyuy.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/grctugmzv.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gnrwdqccj.sHtML

[T44] Perl：条件
来源：http://blog.epnwcf.com/Article/details/gbrhxlrtj.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.vehdjk.com/Article/details/gpjtvitdy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.tarul.cn/Article/details/gdfudncww.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/gvedojnwl.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gdbrnjekx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/gtjuxkatf.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/gizxztbbe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gknagfnsm.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gdzfukzvc.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/gwqbvfghz.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gwamdbutj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gdlkkykdz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gvwtbbdzm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gusirkzee.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/guullrirr.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyomhpbg.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gckwimqqy.sHtML

[T52] Scala：变量
来源：http://www.blog.yfazqb.com/Article/details/grdyswfmx.sHtML

val a = 1;  var b = 2
来源：http://wap.sjlbkw.cn/Article/details/guwwfivzx.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gvvhpmuoj.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gtsmffmey.sHtML

[T54] Scala：集合映射
来源：http://www.share.vehdjk.com/Article/details/grislxnit.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.tarul.cn/Article/details/ggiukxkau.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gtkapelza.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.vehdjk.com/Article/details/gajpopdeg.sHtML

[T56] Scala：样例类
来源：http://baike.vehdjk.com/Article/details/gytyiefds.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fktsv.cn/Article/details/gklwigpjh.sHtML

[T57] Scala：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gejakfriu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gagxxlyio.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/gtndyncbs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.bbcook.cn/Article/details/gltbfigvi.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gktrmorsm.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gtdobuyqo.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/gwakswnvh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/gdchiqkoq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcrvrymux.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gxuxklfyj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxilyszub.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/glvzbjias.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.sjlbkw.cn/Article/details/gkelriolf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/gyyzowmhk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gbfjtpara.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gpzvyhuvt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/gxnrlshxg.sHtML

[U04] Py：变量调试打印
来源：http://baike.fktsv.cn/Article/details/gmbqkfqpb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.epnwcf.com/Article/details/gyrdcjtxc.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gyuaggree.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gydhphepv.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/gitaxbsux.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gspokiwds.sHtML

[U07] Py：反转字典键值
来源：http://3g.yfazqb.com/Article/details/gyrxlzbcc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.yfazqb.com/Article/details/gcmomoorc.sHtML

[U08] Py：展平二维列表
来源：http://m.share.bbcook.cn/Article/details/giqcogwko.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/gvszqqret.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.epnwcf.com/Article/details/gwnhtorwj.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gapmvdbmu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.tarul.cn/Article/details/gdtlgvhqo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.bbcook.cn/Article/details/gljcpgbdk.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gbanqajfy.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.tarul.cn/Article/details/gilvrpwhj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fktsv.cn/Article/details/gnkliikcg.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gtyuarnlr.sHtML

[U13] Py：固定长度队列
来源：http://blog.epnwcf.com/Article/details/guvjrhzbs.sHtML

deque(maxlen=10)
来源：http://www.m.share.bbcook.cn/Article/details/gqsnawegt.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gyxnaxnek.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gyihowzqn.sHtML

[U15] Py：高精度计时
来源：http://www.share.vehdjk.com/Article/details/gzumhfnvc.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/gzacircur.sHtML

[U16] Py：命令行参数解析
来源：http://blog.bbcook.cn/Article/details/gyeqdligs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/gbwufjexd.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/gcuiwaizl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/gnzzhxali.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.yfazqb.com/Article/details/gslypumjw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.yfazqb.com/Article/details/gcijalxzv.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.vehdjk.com/Article/details/ganogstsr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/gtrvcdcqv.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/griyseyeh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gqqbdxqet.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.yfazqb.com/Article/details/gixapddbw.sHtML

@contextlib.contextmanager
来源：http://www.blog.vehdjk.com/Article/details/ggfuqewuq.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/geicqebfo.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/gbkcmjukp.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/grhworbwh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gnwujyvcn.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/ggmcmxifg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/gdmbnoofg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/gsgnafxhy.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/ggofzqkrc.sHtML

[U26] Py：并发下载
来源：http://www.share.bbcook.cn/Article/details/gqirsybub.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gncjroxhz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/gruarffhe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/gkjmvgwsn.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gfdtyplhg.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/grucowehm.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/glkjisobz.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gzssfbzot.sHtML

[U30] Py：数据类
来源：http://www.share.fktsv.cn/Article/details/gvhenvvmq.sHtML

@dataclass(slots=True)
来源：http://www.m.share.bbcook.cn/Article/details/gyyjklavc.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/ginktwkcn.sHtML

python -m pytest -q
来源：http://www.share.epnwcf.com/Article/details/gajemtahs.sHtML

[U32] Py：代码格式化
来源：http://www.blog.tarul.cn/Article/details/glifhujqn.sHtML

ruff format . && ruff check --fix .
来源：http://3g.yfazqb.com/Article/details/gxuczagob.sHtML


<!-- 参考信息 -->