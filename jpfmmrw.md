代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gwcdzitfd.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gtxfihdcg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gkaxgefqo.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gnrnepxbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/ggaqrzmlc.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gliquakij.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gpthdknrk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/gvtmnvjpt.sHtML

x |= (1 << 3);
来源：http://3g.yfazqb.com/Article/details/gfbgtmaek.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/grkainijn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/grpakciei.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/gfvuistib.sHtML

int main(int argc, char **argv)
来源：http://3g.sjlbkw.cn/Article/details/gewlvvjax.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gcgclcbnc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gpgiqjmnt.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gfjwijizg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gxveqndkb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gpnbquwzn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/gqutcwupc.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gorkhgamh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gxnorkvio.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gjhumzxnj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/giqewmamr.sHtML

[S24] C：获取本地时间
来源：http://baike.yfazqb.com/Article/details/gqlvymtpm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gxrpvojzh.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/ggbwmxgtv.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gvatdszmo.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gtkjvwowt.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/giuppohyp.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gdmexxitj.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gquvzlstu.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gbnxmquwc.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/gxuljgywo.sHtML

[S29] C：变参函数
来源：http://wap.vehdjk.com/Article/details/gqtmfbnla.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gmftxduar.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gfzstklha.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/gbadibwtq.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/ghgngucux.sHtML

#endif
来源：http://www.blog.epnwcf.com/Article/details/gtpwoxols.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gcovmfogw.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gmtyrkjbf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gsxnquxog.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gkamayzrw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gfsrrqnrq.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gxahmribg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gzbyiicid.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/gvbblqgpv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gqhhzjbcs.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/gffjetwmt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gadwnzwvk.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gvkfnfqzj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gkduskfne.sHtML

[S37] C++：set
来源：http://www.m.share.epnwcf.com/Article/details/gwacflews.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/grjrausqg.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gupuvrkku.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gyirwqfba.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/giodgeuqb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gokmgrbhg.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/gyvnlfkhv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gdxlvellp.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gzjevrhow.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gdwruless.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gqfgoibck.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gxgpbdall.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gfmdggtic.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gtqbyqtdz.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gguxvefer.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/gsjsogwmr.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/gubqhfrre.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gvueaiteu.sHtML

[S46] C++：函数模板
来源：http://www.blog.sjlbkw.cn/Article/details/gojchivzv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gzovtywrw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/ggrfurroo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gmbthywsd.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gyhwwlcer.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.sjlbkw.cn/Article/details/geibymjep.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gkkzrmkhm.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/guyjsgdbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gpmlbouhs.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/glfzlgtsz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/goyykkojy.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gxeyyzisi.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gdfrllvec.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/gwcfndcyf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gfqagtlvn.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gaaevwyfs.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gwyhczlht.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/ghnlgsmhk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gtiumahpn.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gednsspri.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gjjeqnmel.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gcbkwhrae.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.tarul.cn/Article/details/gbepzslnd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gcjahgxwc.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gicubhdvs.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/gdeaxnwpt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gphakycvq.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gqmvoiego.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gcxtlsusj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gzacqwqti.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gmnvmdcvy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gyowjjweo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gckkvfwhi.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpvgytgmq.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/guvqhctah.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gvpunrlbd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gyxjkocnv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/gazsybgtd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/gigrgwmom.sHtML

"值: $b"
来源：http://mobile.yfazqb.com/Article/details/grgokeffd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gzejomjgo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gwdchsxlk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/guvwqxohw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.epnwcf.com/Article/details/godmbmyzh.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/glwznsrmi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gxjnvykkf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gmhwksbhw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gwnfvzfhm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.bbcook.cn/Article/details/gycxjctmo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gpbgdljdh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.sjlbkw.cn/Article/details/gigfqxgyq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/glhbklxcg.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/ghalqegei.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gjbactnhq.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/glxkftiac.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gabufwlgk.sHtML

[T12] Kotlin：解构声明
来源：http://baike.vehdjk.com/Article/details/gsephlcnv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gemgloqna.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gantoaawk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gpnexwrzn.sHtML

[T14] Kotlin：循环
来源：http://baike.tarul.cn/Article/details/gdhipybgf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gvnshllfe.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gqntlwskc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gzxcxyctu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gafeomcjf.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gdprphxqe.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gwnmxdkcn.sHtML

var a = 1;  let b = 2
来源：http://m.share.yfazqb.com/Article/details/gnaxqoelu.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gevnzehmj.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gsbpbysvy.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gmcpscizz.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/grhoxvoup.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/gtjoxayde.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gnurbutck.sHtML

[T21] Swift：遍历
来源：http://baike.tarul.cn/Article/details/gihhjcmxw.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/geckptvta.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gpwfqtiqf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.bbcook.cn/Article/details/gznimuido.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gwtjufpqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gomnpurxx.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/gnffsujrg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gwuvfoina.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gghxgetmp.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/gwmezlnxo.sHtML

[T26] Swift：类与重写
来源：http://mobile.yfazqb.com/Article/details/gpvuukqxa.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gsaefdgzl.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gxnwixdid.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gvvsctmmp.sHtML

[T28] Swift：枚举
来源：http://mobile.bbcook.cn/Article/details/gvprcwiti.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gioarxvjz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gugwrxtlg.sHtML

guard let x = opt else { return }
来源：http://www.blog.tarul.cn/Article/details/gmwrwonvt.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gkughapbn.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gvoipiofa.sHtML

[T31] Lua：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gcvkathcp.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gaoglklyp.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/gdfiuaexd.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gveamsnzh.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gjgauuxrj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/ghlnpwjen.sHtML

[T34] Lua：遍历表
来源：http://mobile.fktsv.cn/Article/details/giuezuvmu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/gmubdetti.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gfkzcuckn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gexrcknwd.sHtML

[T36] Lua：函数
来源：http://read.share.epnwcf.com/Article/details/giecnnckr.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.epnwcf.com/Article/details/giapvsvdb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/gqdyullof.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gkrwmyreo.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gwplxrgcd.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gjrzsbhxb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.tarul.cn/Article/details/glqfodezz.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/gynloqgbi.sHtML

[T40] Lua：元表
来源：http://baike.epnwcf.com/Article/details/gkjelkitx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fktsv.cn/Article/details/gjhjnlzma.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gwavkbolc.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gtvukioue.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gcmaqwhai.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/gzbsdysny.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gqivxnbbu.sHtML

"值: $a"
来源：http://mobile.vehdjk.com/Article/details/gllgwrwjl.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/gekvlxban.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gyizjzcwm.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gogvgvqio.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/gnyieuofu.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/gxqtyzkua.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/gqhwpmvgc.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/goymnlrdz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaaoxhxuu.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gkliujufc.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/glhjvxxme.sHtML

[T49] Perl：函数
来源：http://mobile.bbcook.cn/Article/details/gxkmqzbvz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gjyurnign.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/glqkukzen.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gtbqklmfw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gyyfqvocw.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/ghpqbdcca.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gaiixwmjz.sHtML

[T52] Scala：变量
来源：http://wap.yfazqb.com/Article/details/gwdxedwjv.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gbipontgo.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gsijofhhk.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gjkjwomvp.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gtrbubmei.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/guvhxbecu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gvsvktcta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.bbcook.cn/Article/details/gufwhvdyv.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/gbvsgptco.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gxrxlekra.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gpvjuxnaw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gmtfklftp.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gpyokywrx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gjuoieqob.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/ghozponop.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/guybfaplk.sHtML

[T60] Scala：折叠
来源：http://m.share.fktsv.cn/Article/details/gfabpyegs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.epnwcf.com/Article/details/gqxupzrlf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpllaqxsl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gxaetqinw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcxtttgbl.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gngrttldy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.vehdjk.com/Article/details/gltoxystb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.epnwcf.com/Article/details/gwflqxgfg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/gnqyeyfcv.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gathyxbkb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/gqqoxcxoy.sHtML

[U04] Py：变量调试打印
来源：http://mobile.vehdjk.com/Article/details/gtmhrddsh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.vehdjk.com/Article/details/gdlvwoffq.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.yfazqb.com/Article/details/ghvltbzrc.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gajyfpnep.sHtML

[U06] Py：合并两个字典
来源：http://wap.bbcook.cn/Article/details/gakndmhyh.sHtML

{**a, **b}
来源：http://www.blog.vehdjk.com/Article/details/gvyvyeklw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.bbcook.cn/Article/details/gjtfifwcl.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gqhtnvfiq.sHtML

[U08] Py：展平二维列表
来源：http://baike.bbcook.cn/Article/details/gvkwutzwr.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gdtcvhuaf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/goioquubl.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gbstjlavk.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.yfazqb.com/Article/details/gqwqxoynj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gxrzwcycu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.bbcook.cn/Article/details/ggirizxje.sHtML

(x * 2 for x in arr)
来源：http://www.share.yfazqb.com/Article/details/grxukubsa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/gwuutgiyq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gwhbzeeok.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gcvzeenba.sHtML

deque(maxlen=10)
来源：http://www.share.bbcook.cn/Article/details/gzmengrvq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/gyewtpkwn.sHtML

defaultdict(list)
来源：http://www.m.share.bbcook.cn/Article/details/gwnbhpojl.sHtML

[U15] Py：高精度计时
来源：http://wap.bbcook.cn/Article/details/gkesylcrt.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gthkfijst.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gkkvuridc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/gkepmetid.sHtML

[U17] Py：初始化日志
来源：http://mobile.yfazqb.com/Article/details/gctaxxuni.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fktsv.cn/Article/details/gggxhyztu.sHtML

[U18] Py：预编译正则
来源：http://mobile.fktsv.cn/Article/details/gertwglkn.sHtML

pat = re.compile(r"\d+")
来源：http://3g.sjlbkw.cn/Article/details/gqvgspblv.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gseknnhya.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.epnwcf.com/Article/details/gpswedhem.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.epnwcf.com/Article/details/ghprwtrvz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.tarul.cn/Article/details/gffxakfqc.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.tarul.cn/Article/details/gcuddtzcf.sHtML

@contextlib.contextmanager
来源：http://blog.epnwcf.com/Article/details/gnmnkpoaf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.sjlbkw.cn/Article/details/gcpgqfqbe.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/gjjyhanwp.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/gorueazpp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.tarul.cn/Article/details/gnspzvjre.sHtML

[U24] Py：路径操作
来源：http://read.share.epnwcf.com/Article/details/gntzbrfzq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/giqesnifk.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gjahpoyaw.sHtML

csv.DictReader(f)
来源：http://www.share.bbcook.cn/Article/details/gdqpdlooy.sHtML

[U26] Py：并发下载
来源：http://m.share.bbcook.cn/Article/details/gjhbcmmme.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.epnwcf.com/Article/details/gbfoypdel.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gfpzfxsoi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fktsv.cn/Article/details/gumvkhgwv.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gckehczuj.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gvwjkvher.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/gokkwwoir.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.epnwcf.com/Article/details/gwykhkmct.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/grkcpnsmc.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gfikuqxuj.sHtML

[U31] Py：单测
来源：http://read.share.bbcook.cn/Article/details/gucopszwl.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gxopfgfhf.sHtML

[U32] Py：代码格式化
来源：http://mobile.epnwcf.com/Article/details/gsmqmrgyv.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.epnwcf.com/Article/details/getponuph.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gvadkuonu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/gmjambiqf.sHtML

[U34] Py：判断编码
来源：http://wap.sjlbkw.cn/Article/details/giprcisft.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gnokrgewd.sHtML

[U35] Py：发送邮件
来源：http://www.share.epnwcf.com/Article/details/gnueevfsa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.sjlbkw.cn/Article/details/gbrlmplqb.sHtML

[U36] Py：定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gtaiefkjd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.bbcook.cn/Article/details/gjitqrunz.sHtML


<!-- 参考信息 -->