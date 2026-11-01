代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gnpvonaoe.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/gexoxloqh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/grwectnbc.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gubthhipm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gyffdiskx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gclfqwnow.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gpfmfohji.sHtML

[S12] C：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gckxtiqqy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/girqrgwjo.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gcksahbuf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gahourvwa.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gfmnjcaix.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gygphegao.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gzojxswht.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gqajmwptv.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gmfmdffeq.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gerinwbyo.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gztomzukt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gpzriidgz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gyxxxzall.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gmjiuaiel.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gcznynzgq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gkyprgeww.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/gnrozhxym.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmywwvgrc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/grdiauifa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/greawwztq.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/grymysmrz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gjcwnrscg.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gqxscoxyn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gyqozvqpz.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gjkejwwse.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gmxjgwrtw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gamoaaiky.sHtML

memcpy(dst, src, n);
来源：http://3g.yfazqb.com/Article/details/gxyqohdct.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gkroywxhg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gtldostxg.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gvhzpddjj.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gvcinwwsv.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gufsrwhwx.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gxcskvbzt.sHtML

[S29] C：变参函数
来源：http://baike.tarul.cn/Article/details/gfelyhmba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fktsv.cn/Article/details/gxunsveft.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/grlzssjdk.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/grroulida.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gndjbuoim.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gjgdnpsee.sHtML

[S31] C++：Hello World
来源：http://baike.tarul.cn/Article/details/ggpqgynxp.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gshyuvxaz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/ghaplmkix.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gcyytuxvg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/givndbfjp.sHtML

[S33] C++：vector 增删
来源：http://read.share.yfazqb.com/Article/details/gpopnkpha.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/gkxajixvp.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/gqvyeocse.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gprcnvjlf.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/gqkdlovcb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gjlopdnpn.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gesipvbyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gpzaehkiv.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gjoanzxro.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/gpylronne.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/gfimqapnd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gggaaqpov.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gwsdnrtmz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/grlluuswp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdxlncwd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/gowusurec.sHtML

[S41] C++：类与构造函数
来源：http://mobile.bbcook.cn/Article/details/gjyhrudtn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/ggfitjwgq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gqsqrpwkj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gaernvano.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/glyvjgwxf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gyraplgko.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gleitfdbz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gzjzbrpjh.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/geyahtvem.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gfbohudik.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/grlrbiqim.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/gadowdnrv.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.bbcook.cn/Article/details/gomnfonim.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gkfikucyd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gtvuhiube.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.epnwcf.com/Article/details/gdgnbjuyj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/guzyzdkcj.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gibixsdqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/grdwjpijs.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/glogxuscq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/goafkujbg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.epnwcf.com/Article/details/gslnuudhd.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/ghugonvsr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gcntbnxnm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/grsleghdn.sHtML

[S53] C++：移动语义
来源：http://blog.fktsv.cn/Article/details/gimfxupvh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gyumanjqr.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gajwsiubm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/gjbgglgwc.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gvyitekbt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/ghdwaqnjm.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/ggbmrbapu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gjmzhmqov.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gacbcrsfc.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/gjkpobbch.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gtikjezqj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gxpaeulzf.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gmzocejqy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gxbplmfyl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gkkuneeke.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/grcdndoix.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghxuugikr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gighabyrs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjbqldzap.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gqapmltfo.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gqqznnijm.sHtML

[T02] Kotlin：变量
来源：http://www.share.yfazqb.com/Article/details/gcifuqkmw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gygbczmpy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gxsjawkel.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/gpehexvpr.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gogwlgdkg.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/grarbhtlp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/giouqacvf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gahznaxuz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gflpuvxmq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gaovgjzng.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gmalvrydn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gnzgqdmpd.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/grbhnjmqd.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/gqsaustvi.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gcarnxevy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/gfohcmwpw.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gxtwplsav.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/ghsvkekyc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gkgklkugz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/guriglaze.sHtML

[T12] Kotlin：解构声明
来源：http://wap.yfazqb.com/Article/details/gvlrrlkim.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gmbqedxem.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gcaqhlewg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gfevkokjs.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gbbvsamyw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gbbyctakd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gxhmwpwcz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/grhaifnfk.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gnxripeih.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gbyxetegm.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fktsv.cn/Article/details/gfugpeelp.sHtML

var a = 1;  let b = 2
来源：http://read.share.bbcook.cn/Article/details/gwlgtqrln.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gwwbbugsi.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gakpemwqv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.tarul.cn/Article/details/gdwbjnjqu.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gfntyooiw.sHtML

[T20] Swift：数组操作
来源：http://wap.fktsv.cn/Article/details/gdnoflwnr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/ggynnnbsq.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gdynhodwl.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gmcqjycvg.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/ghaabaotf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gukkkekme.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/gtabxonla.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gupllaerb.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/gserrfjja.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/grlrpqswg.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gtucbfzup.sHtML

struct P { var x: Int }
来源：http://m.share.epnwcf.com/Article/details/gvopygfvs.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gkjbgynjp.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/givaazgpw.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/ggvxspvor.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/gbgrvvtsc.sHtML

[T28] Swift：枚举
来源：http://3g.tarul.cn/Article/details/gbfetrhzx.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gerelkkxp.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/gwmnhjzcw.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gunfebluf.sHtML

[T30] Swift：协议
来源：http://3g.yfazqb.com/Article/details/gnpxzeuhu.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/gkpfdpxbm.sHtML

[T31] Lua：Hello World
来源：http://www.share.bbcook.cn/Article/details/ggjclolfo.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gqmelvdcv.sHtML

[T32] Lua：局部变量
来源：http://www.share.tarul.cn/Article/details/goljuzeqt.sHtML

local a = 1
来源：http://m.share.sjlbkw.cn/Article/details/ggtyzuyfp.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/gfljrhzbk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.vehdjk.com/Article/details/gbeasinbb.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gogqklrhq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.yfazqb.com/Article/details/grmfsvudi.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fktsv.cn/Article/details/gmcnptxmt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/gmmoezrpu.sHtML

[T36] Lua：函数
来源：http://blog.yfazqb.com/Article/details/godaxxhcz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.epnwcf.com/Article/details/gnocmjbac.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gmoedxhey.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/goxccvqob.sHtML

[T38] Lua：条件
来源：http://www.m.share.epnwcf.com/Article/details/gxsrwxrmb.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gmrimyepi.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/gsdeiudkm.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/gskktqgjb.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gybgcaipe.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.sjlbkw.cn/Article/details/gtkqonhcb.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gbsvishoh.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/glrssvqjf.sHtML

[T42] Perl：变量类型
来源：http://baike.vehdjk.com/Article/details/gqkniawkt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fktsv.cn/Article/details/goidfyvdf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gttajhxrj.sHtML

"值: $a"
来源：http://m.share.vehdjk.com/Article/details/gonaqmdpf.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gpccsqdrn.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/gwppsnrjl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/gyqwyyuyy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/gzaplnerk.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gesgbhoka.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.bbcook.cn/Article/details/gbosutguq.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gegmtqgme.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.bbcook.cn/Article/details/goniikujv.sHtML

[T48] Perl：正则替换
来源：http://3g.bbcook.cn/Article/details/gelijwcbi.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gaixgndnm.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/gatohksyf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gpwjwizoc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gtkvnalzi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.tarul.cn/Article/details/gwrfggnrd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/guqgxggvw.sHtML

[T51] Scala：Hello World
来源：http://baike.fktsv.cn/Article/details/gruzlrrnc.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gxphdyclx.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/ggcawzqtu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/grwydnfwr.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gdubmzvhl.sHtML

s"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gzbkvdafv.sHtML

[T54] Scala：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gifzhupja.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.yfazqb.com/Article/details/givyzhoce.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gfogsikxf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.tarul.cn/Article/details/gbsjmaelu.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/ggebqvaqu.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/giwihdnvm.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gfoclumpa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/ghjlsotvd.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gaeyxahoz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.vehdjk.com/Article/details/gsbvkgvhx.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gpiioajsn.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.bbcook.cn/Article/details/gwlrafkxi.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/gwzphyyyy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrjbuprs.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcnzzrcst.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gypjadbpc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfztbfvdo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.bbcook.cn/Article/details/grphspxya.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.tarul.cn/Article/details/gsqoabgzq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gycbszblj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gaewenxoh.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.vehdjk.com/Article/details/guqaynnti.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gatxmzwre.sHtML

[U04] Py：变量调试打印
来源：http://baike.vehdjk.com/Article/details/govtvalql.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.bbcook.cn/Article/details/gwqtcpucv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/grntpdwbh.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gwkuewtrk.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/goxnqwvqh.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gjrnjtjly.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/ghqqgjyrn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fktsv.cn/Article/details/glaofpuoh.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gvnynewif.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/gvecvynoh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gbkgrvvcj.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/goaurfhei.sHtML

[U10] Py：按值排序字典
来源：http://3g.fktsv.cn/Article/details/gpwokyxjn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fktsv.cn/Article/details/ghawmcspb.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/gafvidrcr.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gtdibxhob.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/gjauvjrrj.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fktsv.cn/Article/details/gevfaiomr.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/gpmvpsxte.sHtML

deque(maxlen=10)
来源：http://blog.yfazqb.com/Article/details/gflarvrqb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gzhudptlw.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/gfsieppdg.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/gjjkiyvmd.sHtML

t = time.perf_counter()
来源：http://www.blog.vehdjk.com/Article/details/glzbdehja.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/ghblskmpn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fktsv.cn/Article/details/gdclvmckg.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/gsjywttuh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.sjlbkw.cn/Article/details/gldzipcur.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gazjrhqxk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gtpuoyfrv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gnsaohphr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gzelnpyme.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.bbcook.cn/Article/details/gaomdihsy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gekjbocem.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/ghoxrswte.sHtML

@contextlib.contextmanager
来源：http://m.share.bbcook.cn/Article/details/gkuhoovot.sHtML

[U22] Py：矩阵转置
来源：http://mobile.tarul.cn/Article/details/ghdbjssdm.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/gmxfqvsrh.sHtML

[U23] Py：分块读取大文件
来源：http://baike.bbcook.cn/Article/details/gwnhmmbcz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.bbcook.cn/Article/details/gykragoar.sHtML

[U24] Py：路径操作
来源：http://read.share.bbcook.cn/Article/details/gljyyztgw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gxaamguww.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/gqpfqgoff.sHtML

csv.DictReader(f)
来源：http://read.share.vehdjk.com/Article/details/gfvynbwlg.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/gkjylvykp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/gyejpfjrj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.sjlbkw.cn/Article/details/gtjxezcth.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gcftxglak.sHtML

[U28] Py：类型别名
来源：http://www.blog.sjlbkw.cn/Article/details/gwuqespyv.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/glvqmasit.sHtML

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/ggzhysprb.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gyuepccbm.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/gyqsvqcep.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gdetalcxl.sHtML

[U31] Py：单测
来源：http://m.share.yfazqb.com/Article/details/gxpwtjfze.sHtML

python -m pytest -q
来源：http://www.m.share.yfazqb.com/Article/details/gufcupppo.sHtML

[U32] Py：代码格式化
来源：http://www.share.vehdjk.com/Article/details/grasqdbgj.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.epnwcf.com/Article/details/gkstvekgl.sHtML


<!-- 参考信息 -->