代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gccxsixph.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/gkkjmngne.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gmlkhsbox.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gdvhazkzm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/gzhmducyt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gzxqpuyir.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gafimxyvr.sHtML

[S12] C：写文件
来源：http://blog.fktsv.cn/Article/details/gvyveemyx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.bbcook.cn/Article/details/gtfsvjrpq.sHtML

[S13] C：宏定义
来源：http://www.share.bbcook.cn/Article/details/gkxpeixnj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gnhioyvrk.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gfwjqwzdk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.sjlbkw.cn/Article/details/gdrtvnkfj.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/guomfwgni.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gyeuhsvtw.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gyigdpaxb.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/glkdfcobu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gosdmpyjg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gefxncngu.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gnzmsnzpg.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/gndchobvl.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/ghdrbtmxd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gkztdlqvj.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gsvgyjinq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gwwsjwjfq.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gavlzjcfi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/glswgkkkt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gqqwmiqib.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gjqfyckvz.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gdmtxmmcu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/gpljybdsm.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/gqouhyunv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gjgeqlnix.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/gtcofznpx.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gdvyexpdw.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/gfcboftfh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gcqugakqx.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gkrchxfmx.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gyauufcrt.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/ggppktitx.sHtML

static int counter = 0;
来源：http://mobile.sjlbkw.cn/Article/details/gypupjefs.sHtML

[S29] C：变参函数
来源：http://www.m.share.tarul.cn/Article/details/gfyihwwoh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/gjwkvjlhp.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/grzdafqwo.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gejqidodu.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gafqqhbhl.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gebvdshzx.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gxpkzodly.sHtML

#include <iostream>
来源：http://mobile.yfazqb.com/Article/details/givqkbhvs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbufygert.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gbydqbyxe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.vehdjk.com/Article/details/grmolenjo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gqibhcacv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.epnwcf.com/Article/details/gggzzvhck.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/ggpvjmlvl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/gzzprcwel.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/grhylgwbf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gntzfwdyb.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gmcjdnuwz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gbntpoovc.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gfslgjdgt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/goqbmvlcc.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/girajbigg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gjissvlej.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gztqigutb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/guwydfcgz.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gtdneihoc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gabszpqxt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gqaaijilz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gdifnmxjk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.tarul.cn/Article/details/gqwpaudfz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gucsponvt.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gyiugcpox.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/gdjidcngw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeefmggc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gdbyqcjcx.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gfiwczohm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/golwdmonm.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gxnjdytjx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gmidmqdkh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/ggrfhtzmr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtqnwhbz.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gffpdjkxb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gefafatoy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gpyfxajzi.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/ggvnfggfh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.tarul.cn/Article/details/gxncxknlu.sHtML

[S50] C++：格式化数字
来源：http://baike.tarul.cn/Article/details/gekbwueoc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/gozhdjkvi.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gcrqlwald.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/gwzkkstrw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/gghvtrxhe.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.tarul.cn/Article/details/gnwbvthdp.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gpgnggaux.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gkyphbobb.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gplckicqm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gahptnrbl.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gzumcrbam.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gjfhekhhq.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gpfegbcxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/gymgbelat.sHtML

[S57] C++：编译期常量
来源：http://wap.tarul.cn/Article/details/gfxtunoyq.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gteecksvv.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/gktgaiejf.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fktsv.cn/Article/details/givfllqlt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/gaeznrygm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/gdhpxgqze.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gjdivjswl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gfyegspiy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/giqykhmne.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gijgwepft.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsddvxwad.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/glqkstbxb.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gjkqmqidu.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gejaimkco.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.bbcook.cn/Article/details/gsxijahrv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gtdlaxijq.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/glkccjjbk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.bbcook.cn/Article/details/gjywlxinw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gboqddgng.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.vehdjk.com/Article/details/gzgbuwrzu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gsuxpdhei.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/givqhfndb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gkfpjsktz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gqzgdoiyr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gvzsnjqrv.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/gfcttfaia.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gpiozlmxs.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gmbaehzhd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gicownfbw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gujznkaxh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/ghzqykymb.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gfykbznmd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.bbcook.cn/Article/details/gxgiurvqe.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/ggexzbtkg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/giitggskn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gaejlgyov.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gyrcjukaq.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gqdkhegca.sHtML

for (i in 1..10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gsxngztea.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gwgffsuzl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.bbcook.cn/Article/details/gwhcfngum.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gdyipjgpo.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gstjxckwa.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.yfazqb.com/Article/details/gefyhmaqh.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/gxfmcdodz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gglpbzsxs.sHtML

"值: \(b)"
来源：http://baike.sjlbkw.cn/Article/details/gsnlhkuhe.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gxknqcxvy.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gggopbims.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gtobrcztc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/gcfcvpbpt.sHtML

[T21] Swift：遍历
来源：http://wap.tarul.cn/Article/details/glqqqxeza.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/ggzpouhpv.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/gcaahmlsc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbewnniy.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/gzwcfpwer.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gziiffjyd.sHtML

[T24] Swift：闭包
来源：http://read.share.epnwcf.com/Article/details/gxyzpurwr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gkhdsmpii.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/ghxlxzkfl.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gewwyjwme.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gsbzntcot.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gzdpqzwny.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gwphjnnvr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/ghdunxity.sHtML

[T28] Swift：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gnjedkezn.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gglpsiehi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gvhhpeprc.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gowcgdqce.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gvnyrutul.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gakjwdajw.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/getgxsngj.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/goixtqdnr.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/gzptqupzb.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gfaqxschl.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gtfclfqhf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.sjlbkw.cn/Article/details/gyzhdsrst.sHtML

[T34] Lua：遍历表
来源：http://wap.bbcook.cn/Article/details/gdalvqrtc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/grszhseeb.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gfqmbzqwk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/gxkkgtoqs.sHtML

[T36] Lua：函数
来源：http://www.m.share.vehdjk.com/Article/details/ghxnzpnsk.sHtML

function add(a, b) return a + b end
来源：http://m.share.vehdjk.com/Article/details/gvjiatnko.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gxjocwnzx.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/gdkwlbacp.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/guqhbykws.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/golsswfyd.sHtML

[T39] Lua：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gubpwtxyy.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gbvqadtkd.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/gbqsfypks.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fktsv.cn/Article/details/gwaczveoa.sHtML

[T41] Perl：Hello World
来源：http://mobile.yfazqb.com/Article/details/gpnnmrgxq.sHtML

print "Hello\n";
来源：http://m.share.yfazqb.com/Article/details/gvtznthys.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gktddqkam.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/gjhpqtcyg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gsjvtvern.sHtML

"值: $a"
来源：http://baike.sjlbkw.cn/Article/details/gcbakwbdq.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/ggmvpmqij.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/gnriaeyoc.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/gnvnycsxh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gjfwskffy.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gveyuwhxe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gduhxvebg.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gietsyhrm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/gjlcpjhyu.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/glgiwopdg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gozicgmzq.sHtML

[T49] Perl：函数
来源：http://www.blog.epnwcf.com/Article/details/grrcjfxqs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gsxvjlzmj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gztwzodih.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/grbcamunq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gtuomekes.sHtML

[T51] Scala：Hello World
来源：http://blog.bbcook.cn/Article/details/ggohuvtvn.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/ghgibofmu.sHtML

[T52] Scala：变量
来源：http://3g.vehdjk.com/Article/details/ghqagbrwc.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gxrgztkms.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gxcjwkinf.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/glykqwmll.sHtML

[T54] Scala：集合映射
来源：http://baike.epnwcf.com/Article/details/gzcjanblv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/gpilwziig.sHtML

[T55] Scala：集合过滤
来源：http://read.share.tarul.cn/Article/details/grmvpzxpb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gbfphewsd.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/gvkptmjqd.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gahkreoon.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gqrmbicyl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gvchwmbno.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/gtnxurgwh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gwbxxbszf.sHtML

[T59] Scala：循环
来源：http://wap.vehdjk.com/Article/details/grezopplr.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.yfazqb.com/Article/details/gcplvzsjm.sHtML

[T60] Scala：折叠
来源：http://www.share.yfazqb.com/Article/details/gonyrohtb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.vehdjk.com/Article/details/gvbyivqwz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geiyuyrib.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/goghanhte.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtrdhrvis.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.vehdjk.com/Article/details/goshtnemc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gwoifyfgf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gctpayeom.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.epnwcf.com/Article/details/gocxaayqt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.yfazqb.com/Article/details/gvjwmvqbq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gxuzlxbxj.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gppmeyuiq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fktsv.cn/Article/details/gmwschzdr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.vehdjk.com/Article/details/gsgoocqgs.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gifaofviu.sHtML

[U06] Py：合并两个字典
来源：http://3g.epnwcf.com/Article/details/gxpgmdcgr.sHtML

{**a, **b}
来源：http://mobile.yfazqb.com/Article/details/gzetnnzzp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.tarul.cn/Article/details/giezfzuqb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gyxwhstuw.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gcomnrrrv.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gullxcvwx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/gujjickci.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/gsdvvsxbu.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/ghrwlmesl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.bbcook.cn/Article/details/guzconugt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.tarul.cn/Article/details/gvxnazstu.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/ghgrpgrqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/ggpswzclv.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gukzxvddu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gtzrundwh.sHtML

deque(maxlen=10)
来源：http://wap.bbcook.cn/Article/details/gvmvtgrze.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/gwwzsrkzm.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gimlqlgah.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gvuutjdjg.sHtML

t = time.perf_counter()
来源：http://wap.sjlbkw.cn/Article/details/gyrigbygg.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtpmzqkr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.sjlbkw.cn/Article/details/gcwsyawyl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/gxfwwdjji.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gjsuuigln.sHtML

[U18] Py：预编译正则
来源：http://www.blog.epnwcf.com/Article/details/gtyueupqk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gzttdfcxv.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.vehdjk.com/Article/details/gomhjkwpl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/gwnywbcdy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.yfazqb.com/Article/details/gcysvzukn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/gezrokhsd.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gbgmqotzk.sHtML

@contextlib.contextmanager
来源：http://blog.bbcook.cn/Article/details/gfuaytocu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gpvxmrczg.sHtML

list(zip(*m))
来源：http://www.m.share.yfazqb.com/Article/details/gditldojf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gqxeqtykl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/gapinnmxc.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/grclcoedp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gulfytfyl.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gzpfvwzxv.sHtML

csv.DictReader(f)
来源：http://m.share.vehdjk.com/Article/details/gyctmqemn.sHtML

[U26] Py：并发下载
来源：http://www.m.share.vehdjk.com/Article/details/gnjbwescv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fktsv.cn/Article/details/gveurqfcs.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/gbtwilmqz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.bbcook.cn/Article/details/gmqwxavol.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gufnoyaxa.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gmsxxkskm.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gxikymwvr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.yfazqb.com/Article/details/gjsfwkjip.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/gghthhnbv.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/gttkrldmz.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gpfpwhnfi.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gxzvwqnji.sHtML

[U32] Py：代码格式化
来源：http://www.share.vehdjk.com/Article/details/gvsnngqmr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gedgppezw.sHtML


<!-- 参考信息 -->