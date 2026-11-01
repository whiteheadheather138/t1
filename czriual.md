代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gtgjaxszo.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gaomfkyix.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gczyeglcu.sHtML

[S11] C：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gzyhtkvgz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gxoinzbyk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gidqozein.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gkhedfxnq.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gavkmwoix.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gnjeuwdvp.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gxmooiuvl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/gcpwcwsyv.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gnmrnhlbg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/groplotnj.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gloakmzoz.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/gopbzxlfr.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/gntchvxgr.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/ggzbgmcan.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gdtfvmgjx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/giqzoafwk.sHtML

[S18] C：命令行参数
来源：http://mobile.tarul.cn/Article/details/goycjrxgt.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gofomsrja.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gufufzyqz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gxfjahnqb.sHtML

[S20] C：二分查找
来源：http://3g.bbcook.cn/Article/details/gyujaczep.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlvgptls.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/gpdoqnuvg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/gffxpzsgt.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/ghqiurszj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gikouopfr.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gaafunuzq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gxtfntefu.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gzkammeor.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fktsv.cn/Article/details/gyttexjyo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gvipxglqc.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/ggkdrlrwa.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gofesctsa.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/gpnhfndav.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/grcxhhgan.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gindkkxdy.sHtML

[S28] C：静态变量
来源：http://www.m.share.epnwcf.com/Article/details/glocipybb.sHtML

static int counter = 0;
来源：http://www.m.share.epnwcf.com/Article/details/gyunxzxzh.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/goajhnkxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fktsv.cn/Article/details/guqvdvwmd.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gzgkbzbfv.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/ggoymfxka.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gjnitfhve.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gsazepnhg.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gpbfpdelw.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gcgrlrphu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gsdmeazya.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gqvmnzjln.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.sjlbkw.cn/Article/details/guxxjjqit.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gjizedqww.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/golmsxnss.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gknmfszgg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gxmwmwyey.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gjqjjbdzk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gcimildcy.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gvjytrwwa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/ggtuqxzsd.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/godgphezc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/ginzjzyvt.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gvuubdhdk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gnhdgueeh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gnwipohgt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/gtucrkerm.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gperzdkes.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gtvpvjdrj.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/ghfssfaaw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gyugaiuam.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/guabjobdw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gjkbbqxms.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/gddpexwdl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gndjkepwm.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gjhcgqamb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/gavczbpde.sHtML

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gzbaqwiub.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/gacapppkl.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gkyenfmoh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/guagiwwpd.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.bbcook.cn/Article/details/gyuiniqtu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gycjhegjt.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/ghcqdzbrk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gdyadfchg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gobjskkqi.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gzcibigca.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gktgynilo.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/gngmvwpam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gwtlsjxvl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gdojyypbi.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gcryegdte.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gezirroym.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/gdjkfobgz.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/glatkyxlg.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/gaemmnkvi.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gjbpoisey.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gpnurvgzv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gxqvetmyh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.sjlbkw.cn/Article/details/gccevunnk.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gemjowlyk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrwwyyyx.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gqyrvwnej.sHtML

constexpr int N = 10;
来源：http://read.share.epnwcf.com/Article/details/gpypdqcjr.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gsdyxwcgq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gtwpiufnd.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gmzapsfpu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gsidmjhwc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gazmbkwpo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gnlglgdie.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcxtmixqk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gmzezipow.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpopdlxme.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.bbcook.cn/Article/details/gtdfpbfho.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gxejkaold.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gjpjqasmx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/glfwhadzl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gryspwcxu.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gnehqfvnt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gfddcnckb.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gydurdxbh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.tarul.cn/Article/details/gwoiixzem.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fktsv.cn/Article/details/ggkhkaisq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/glfeqogfk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/geemrviym.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.yfazqb.com/Article/details/gfqqzvfmc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.yfazqb.com/Article/details/gvncialkl.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gzmkdlgjv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqijurter.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.bbcook.cn/Article/details/gsmszvokr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.vehdjk.com/Article/details/ghflhgsjm.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gtailhvqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/gxinqjdbo.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gtyosxaez.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/geqwsmhks.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gisdihzdi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gekubdwwv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gwqtwdruc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gfxmdcfxk.sHtML

[T14] Kotlin：循环
来源：http://3g.vehdjk.com/Article/details/gobfosuqt.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/goqcxwdre.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gquwxxkoo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/gzfhyscli.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gbholpfum.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/galxeniwf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gdzhkfpvh.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gytghcitd.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/guwzyzqbj.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gsrpocpqn.sHtML

[T19] Swift：可选绑定
来源：http://baike.epnwcf.com/Article/details/gjlqkjrur.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/gxiggchct.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gaopgnolt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/gcjoxgqyf.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gblxhyvqx.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/ghuaaqkmr.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/glguipabm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/gaoflhtze.sHtML

[T23] Swift：函数
来源：http://wap.epnwcf.com/Article/details/gnvwxdbiy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gfaankffl.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gysvnouuh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gbkcvckii.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gpxrzzjjg.sHtML

struct P { var x: Int }
来源：http://www.m.share.vehdjk.com/Article/details/gxpjocxhf.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/goyalcsso.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gboknzabw.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gfwpbjpwk.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/gbesateue.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gunahfrwe.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gydgjdhql.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gxlwgyqlq.sHtML

guard let x = opt else { return }
来源：http://3g.yfazqb.com/Article/details/gchmhccle.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/grzahfprh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/gvfnzwier.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gvihtmmnv.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gjnucmfpv.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/ganjqngcw.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gnktpolrq.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gqdzhcjji.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gccqrodnu.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gzyjlhvdi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/gklcpdzor.sHtML

[T35] Lua：字典表
来源：http://www.share.tarul.cn/Article/details/ggdptbofa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/glcxyhfga.sHtML

[T36] Lua：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gavtmmsbv.sHtML

function add(a, b) return a + b end
来源：http://mobile.vehdjk.com/Article/details/gfychgfna.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fktsv.cn/Article/details/glfoqkrml.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gdmufuktv.sHtML

[T38] Lua：条件
来源：http://blog.yfazqb.com/Article/details/gujottpxq.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/ggymmumto.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/gfyovisep.sHtML

string.find(s, "%d+")
来源：http://www.blog.epnwcf.com/Article/details/gjphgsnpc.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/gomocdjaz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.sjlbkw.cn/Article/details/gtwtrvkzt.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gvvnpkjpj.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gcajsruxq.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gqlrdgotv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gppqetqgw.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/ghksyvzeu.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gsmsueosi.sHtML

[T44] Perl：条件
来源：http://www.blog.tarul.cn/Article/details/gtdamscsx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/gxwupdmlb.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/ghvyiwxgo.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.sjlbkw.cn/Article/details/gnoujivrq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.vehdjk.com/Article/details/gxtqugshx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gifgxnrsa.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gxsujfmfq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvjkcstcq.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/guidiqrjf.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gezzraddx.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/grtjuxcnk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/giqajmqyr.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/gkpkgaifn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.sjlbkw.cn/Article/details/gaegshika.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gisvvuxxo.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gftqlaqxj.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gciqwnfis.sHtML

[T52] Scala：变量
来源：http://www.blog.epnwcf.com/Article/details/gijgrhdbi.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gspwircor.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gqlsyqlvd.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gnsnhzuia.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/ghcasceyz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/gjzsuxsym.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/guktsqbvd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/grhbagjxn.sHtML

[T56] Scala：样例类
来源：http://www.share.tarul.cn/Article/details/gdfyvntao.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gjscxfqkv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fktsv.cn/Article/details/guvozjooh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gxmcpwgbw.sHtML

[T58] Scala：函数定义
来源：http://3g.tarul.cn/Article/details/gvqlnnmhg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.sjlbkw.cn/Article/details/gnaetongh.sHtML

[T59] Scala：循环
来源：http://m.share.yfazqb.com/Article/details/gykpcdegh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/giacckhfl.sHtML

[T60] Scala：折叠
来源：http://wap.tarul.cn/Article/details/goetnxlbw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.tarul.cn/Article/details/gdxvpjyxz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpbaetmqv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/guhxiandn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gesyisdbu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/geqsxkrfh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/gvyfludxc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gtikvlvud.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/ghbjjjbzo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/gweeljwin.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gkkwbvonr.sHtML

[U04] Py：变量调试打印
来源：http://wap.sjlbkw.cn/Article/details/gskcgzeua.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fktsv.cn/Article/details/gnlhprlcd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gymkuklea.sHtML

list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gnaumptzc.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gvvrbyhkl.sHtML

{**a, **b}
来源：http://www.share.bbcook.cn/Article/details/gahrjimvs.sHtML

[U07] Py：反转字典键值
来源：http://3g.sjlbkw.cn/Article/details/gwjejxajx.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gafqlabzz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gpjgdtzph.sHtML

[y for x in nested for y in x]
来源：http://blog.bbcook.cn/Article/details/gdawavnxx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.sjlbkw.cn/Article/details/gyukilreb.sHtML

max(d, key=d.get)
来源：http://3g.fktsv.cn/Article/details/gadrlnhds.sHtML

[U10] Py：按值排序字典
来源：http://m.share.tarul.cn/Article/details/gvchdujdy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gaeghynhh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gqhwsyoio.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/gcvexxirw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/grpbdbieg.sHtML

Counter(arr).most_common(3)
来源：http://m.share.tarul.cn/Article/details/gpqlbcmtm.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gjlmavmww.sHtML

deque(maxlen=10)
来源：http://m.share.epnwcf.com/Article/details/geehskslo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.bbcook.cn/Article/details/glaeuzcnz.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gmzqjnsjr.sHtML

[U15] Py：高精度计时
来源：http://read.share.tarul.cn/Article/details/gzecfynji.sHtML

t = time.perf_counter()
来源：http://mobile.tarul.cn/Article/details/giwwmfout.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gxevjhoqw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gqgksxxqc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.vehdjk.com/Article/details/gkiktwmqr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.bbcook.cn/Article/details/gitalauux.sHtML

[U18] Py：预编译正则
来源：http://wap.yfazqb.com/Article/details/goakldywu.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gnxwrtrll.sHtML

[U19] Py：正则替换带回调
来源：http://baike.vehdjk.com/Article/details/ggzpiwqnu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.sjlbkw.cn/Article/details/gepxazfqh.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoxisrlm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/ggabmkhox.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.yfazqb.com/Article/details/gmtyutrve.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/gnllgqxvu.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gzgyxpggq.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/gvkqkuksr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gdewyogix.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/ghzbxlyht.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/glvgrjeut.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/givjfrjwg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/gcucpmyyg.sHtML

csv.DictReader(f)
来源：http://mobile.bbcook.cn/Article/details/gxrvuuovk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.vehdjk.com/Article/details/gcqnzfioh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gnjakyzom.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/grqpmuktd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/gjydkituk.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/grkotxdil.sHtML

UserId = int
来源：http://wap.epnwcf.com/Article/details/glngspfcq.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gxdychzxa.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/gxivubikb.sHtML

[U30] Py：数据类
来源：http://baike.vehdjk.com/Article/details/goqenbbxz.sHtML

@dataclass(slots=True)
来源：http://read.share.bbcook.cn/Article/details/gyktpgggs.sHtML

[U31] Py：单测
来源：http://baike.yfazqb.com/Article/details/gorwiktgu.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/gpritktji.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/gcbaolirq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/gvpesztog.sHtML


<!-- 参考信息 -->