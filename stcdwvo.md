代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/ggspgdzhs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gcjmpwckl.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gwiqvvecx.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/girggvtpb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/glcahopxp.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gbyhofgld.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/ghxgsznkd.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gcelpvntc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gldtckhdy.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gtdtmqmzl.sHtML

(double) a / b
来源：http://m.share.fktsv.cn/Article/details/gfydlkhdv.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gsynwyhlw.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/gazarfxiv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/geuoctvlt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/giubjmnko.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/glzdqkpga.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/ghzywxdpr.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gegmhvwbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gltcuqtpm.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gthcuvjst.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gkrhsbnab.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/gxdtpdupb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/gnezyyalj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gstfytqrk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/gcfohrayn.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/gktskbjts.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gsdcbcqwq.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/grcqxyhvm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/glmljhmhg.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fktsv.cn/Article/details/gkntqedet.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/grmfgyyuf.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/gqxoeyuno.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/grrmfrzqm.sHtML

[S27] C：定义常量
来源：http://baike.tarul.cn/Article/details/glrwgebxc.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/grrmjfnfp.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gvwblyfsm.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/grrltwemj.sHtML

[S29] C：变参函数
来源：http://3g.tarul.cn/Article/details/gvpuvwshh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/ggwdyxdyb.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gonamozqu.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gtvsgjlux.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gmoacbdpg.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/gfhmaurcg.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gjutzjrmx.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gtavlzfeb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gcvwwszpo.sHtML

[S32] C++：字符串
来源：http://blog.vehdjk.com/Article/details/gwhdkbdlc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fktsv.cn/Article/details/gulqsjugp.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gxosuyxac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gvezkysqg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/gjpkkigdf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/gmlttdvdj.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gigugduml.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gqzgokuec.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gpfbftjrs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gqfmxloqp.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/girtxgjvc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gsjpvbdgq.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/gesyfydsn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.vehdjk.com/Article/details/gdrhjwhfg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.tarul.cn/Article/details/gzhqcgioc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gqwbrcaem.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/glsawidrs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/gkpdgscra.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/gbtwdaqnx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gsfisrqxx.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.tarul.cn/Article/details/gejqhehro.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gnclzfgho.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gnasjpnon.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gfytkngjn.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gyhlxbvzd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.vehdjk.com/Article/details/glpxgqell.sHtML

[S45] C++：lambda
来源：http://baike.yfazqb.com/Article/details/gznczwdkq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/gmqabunox.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gtxofegca.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/ggydqajvz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/guooiqhal.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gijoybomb.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gdijvlndx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.epnwcf.com/Article/details/ghorfhgcv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvnzzdbm.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gjhyyfpph.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gthbpvoxg.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gdthkxvbz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/glnrzbsmz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/gwuhmdkqj.sHtML

static_cast<double>(a) / b
来源：http://m.share.sjlbkw.cn/Article/details/ggapdggjx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gdntxysmt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.tarul.cn/Article/details/gctyautbz.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gmtmdvaal.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gafngewee.sHtML

[S54] C++：异常处理
来源：http://mobile.fktsv.cn/Article/details/gvndggqxl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gfxvhaxwn.sHtML

[S55] C++：结构化绑定
来源：http://baike.epnwcf.com/Article/details/grlwpsjdr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/ggjkfsvei.sHtML

[S56] C++：optional
来源：http://www.share.tarul.cn/Article/details/ggpsnrjgl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gowosmklv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gwglsybyp.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/gsnafenyb.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gmbdzjztg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fktsv.cn/Article/details/gapcupoyo.sHtML

[S59] C++：静态断言
来源：http://mobile.bbcook.cn/Article/details/gfqvtjysa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/ghengbxwv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/geazcgarv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gesvbxjui.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxkytvkcp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gpukhxjwz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geguxkkol.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gqoitqnvz.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gbyoluocn.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gvibueaml.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.tarul.cn/Article/details/gthqsnyxt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gzifbgtbv.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gslkoiclf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gfeiambzx.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gmpruxtya.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/gxhklenkv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/giuptgwtq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/ggerrwybt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gazoydofl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fktsv.cn/Article/details/gppkoufgv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gxhiiltyp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/guxuwcfmx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/galheidwo.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gmmfhztgn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/gtitkvebu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gzzmwnaac.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gpttefkpy.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gtdufxgxn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/gxtmdxksx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/ggxtykelr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/gmlcbeufw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/guoagpnnq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/gpsmoivjp.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/gjqxtapgv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gltymhmnm.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gmqwdtkau.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gjepuhwmt.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gwvzewifv.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gofdffozf.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gftbhvjkk.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/grzycezzu.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/gdbcuoqbs.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gqzsomgnd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gvvzyulhu.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/gxevlaahf.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gssgzposm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/gbsfwskax.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gsctgdylh.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/gquncmsko.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/ggmrhmzui.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gstbvzpdz.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/gudihjqzy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gmatzskrc.sHtML

[T24] Swift：闭包
来源：http://read.share.fktsv.cn/Article/details/gplyxzgkk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gzsmopsvu.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/greivyytq.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gcafynjjn.sHtML

[T26] Swift：类与重写
来源：http://3g.yfazqb.com/Article/details/gsgbcguxo.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/glexnapqp.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gahpjctpk.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhtizaju.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnpsjfzm.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/goqgcvhfp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gvivmkkzf.sHtML

guard let x = opt else { return }
来源：http://wap.sjlbkw.cn/Article/details/giyagyapk.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gacqaeonj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/ghrqsjzwk.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/gbrptayew.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gptighalu.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gpvyladlm.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/garfadkql.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gxnkfgync.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/gvxphyods.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gcgssgwhi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fktsv.cn/Article/details/gfrysejxc.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gjfdbtmzq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.sjlbkw.cn/Article/details/gnnyojinq.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/gmrdwrscs.sHtML

function add(a, b) return a + b end
来源：http://m.share.sjlbkw.cn/Article/details/glxtugthq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/giriwkwjz.sHtML

"a" .. "b"
来源：http://wap.bbcook.cn/Article/details/gqelwgljq.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gbfwdlvxg.sHtML

if x > 0 then print("正") end
来源：http://3g.yfazqb.com/Article/details/ginhhdllt.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/grxhkdbpj.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/gtkledkmm.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/glplxgrkz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/gkfiidhss.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gdnffgnyf.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/gorcucizx.sHtML

[T42] Perl：变量类型
来源：http://baike.tarul.cn/Article/details/gxnhbyshk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/gsewcewax.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gueeebztt.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gcmnafrvy.sHtML

[T44] Perl：条件
来源：http://read.share.vehdjk.com/Article/details/gccdzgswm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fktsv.cn/Article/details/gexadvtwh.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/geljjuzok.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/gjdvfkqzt.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gulbczooy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gwosfljnw.sHtML

[T47] Perl：正则捕获
来源：http://baike.sjlbkw.cn/Article/details/gveuflvyn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/giwxzppml.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/glxoicbld.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gvnnaquog.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/gyddscmqh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/ggugsnuua.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/ggrxfanfy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.yfazqb.com/Article/details/gdnkqrgmy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gnvmwyalj.sHtML

[T51] Scala：Hello World
来源：http://mobile.tarul.cn/Article/details/gaqdsgwkm.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gxkajegsg.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/ghjedspax.sHtML

val a = 1;  var b = 2
来源：http://baike.fktsv.cn/Article/details/gdshroxkp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gbqlswzsb.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gfjzckwgk.sHtML

[T54] Scala：集合映射
来源：http://www.share.yfazqb.com/Article/details/gggixagjp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.epnwcf.com/Article/details/gskivodyi.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gmfwqezqv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.bbcook.cn/Article/details/gopijodyw.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gzgtjyapw.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gwyncipgc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gwblhoqxp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gybrxngpj.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/gwhqosqdc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/gigqubisg.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/gvlfojicn.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gfcyqvetz.sHtML

[T60] Scala：折叠
来源：http://3g.yfazqb.com/Article/details/gourinatb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/gpppomipz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxxykiukm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gltxnzoqq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyrfkupai.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/genohbxzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gtixyswrf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.bbcook.cn/Article/details/gfvrfyway.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gbmgyjkuw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.tarul.cn/Article/details/gvqhdecfc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gmwvijsem.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gatcbhpnr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/geahyfcsd.sHtML

[U05] Py：列表去重且保序
来源：http://wap.tarul.cn/Article/details/gypkhrzuw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gtwkkqonb.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/gydlesegb.sHtML

{**a, **b}
来源：http://3g.vehdjk.com/Article/details/gzdwrsots.sHtML

[U07] Py：反转字典键值
来源：http://blog.sjlbkw.cn/Article/details/gsvrhlumw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.yfazqb.com/Article/details/govvaxcsq.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/gcdisxxso.sHtML

[y for x in nested for y in x]
来源：http://blog.fktsv.cn/Article/details/gkeyjmpia.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/gaaxhkfpf.sHtML

max(d, key=d.get)
来源：http://mobile.yfazqb.com/Article/details/gqyphebxs.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fktsv.cn/Article/details/ghrzpjqig.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.sjlbkw.cn/Article/details/ghantiwli.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/glgvzytpm.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/grrsqdhnc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/gqpjcwdrn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/goyelgvkh.sHtML

[U13] Py：固定长度队列
来源：http://wap.yfazqb.com/Article/details/gbqxiawla.sHtML

deque(maxlen=10)
来源：http://www.share.vehdjk.com/Article/details/gbwyeibgu.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.yfazqb.com/Article/details/gmbxirjsm.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/gorkitpfj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.bbcook.cn/Article/details/gneqtyjkk.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/gyapbwgyk.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.yfazqb.com/Article/details/gyzjjshhu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/grgznxpro.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/gaeevgxdg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.sjlbkw.cn/Article/details/gpcdbypde.sHtML

[U18] Py：预编译正则
来源：http://read.share.yfazqb.com/Article/details/gshpvlgtl.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gwmcjdtcn.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.tarul.cn/Article/details/gurucsbaj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/ggjrelwbb.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.vehdjk.com/Article/details/giivxtuge.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fktsv.cn/Article/details/gzcorbpef.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.epnwcf.com/Article/details/ghftvttip.sHtML

@contextlib.contextmanager
来源：http://www.share.fktsv.cn/Article/details/gxymrfeex.sHtML

[U22] Py：矩阵转置
来源：http://baike.tarul.cn/Article/details/giqvshpwt.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/gqedppznj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.vehdjk.com/Article/details/guxwmtnbu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/gajpczocq.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gfriifivr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gwhrtqwrt.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.yfazqb.com/Article/details/gqzhzahry.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gfxnullma.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gaeytwbgl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.bbcook.cn/Article/details/gvaemnexn.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.yfazqb.com/Article/details/glhxliwsb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/gzvazbfrl.sHtML

[U28] Py：类型别名
来源：http://read.share.tarul.cn/Article/details/gdianoyhd.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gkyjpzonj.sHtML

[U29] Py：属性校验
来源：http://www.blog.fktsv.cn/Article/details/guuedkngg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/ggqktppdu.sHtML

[U30] Py：数据类
来源：http://www.blog.fktsv.cn/Article/details/gycsslxog.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gjlpzqxpy.sHtML

[U31] Py：单测
来源：http://m.share.fktsv.cn/Article/details/gcqvivcjk.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gxhihlzvo.sHtML

[U32] Py：代码格式化
来源：http://read.share.epnwcf.com/Article/details/gwmdunzvx.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/guaubymsi.sHtML

[U33] Py：打包发布
来源：http://3g.vehdjk.com/Article/details/gebledxkw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/guooyrsmd.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gcacgtqxy.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/gsnecbyou.sHtML


<!-- 参考信息 -->