代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gdqfgteta.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gjrrfudaw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gtuukwmcz.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gibltflru.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gkmggqbgt.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gztpvwymx.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/grailbmzw.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gteqyvxxl.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gyzgphfuc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.bbcook.cn/Article/details/gjyvdjgjz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/gjqdahsib.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gjkntstoa.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/ghhlldzuz.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gsyvdsqwy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gpmrdxlyi.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gzjhdkgir.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gtazcvked.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/goxklecnh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gpfliutml.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/glyjxqimi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gifrhabdc.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gsjwfbwvl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gqfywmpcm.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/gnhhgtfev.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/glfnaljtx.sHtML

[S25] C：内存拷贝
来源：http://wap.tarul.cn/Article/details/grbkbqhca.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/geuobrvfx.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/ggnidnaoy.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.epnwcf.com/Article/details/glsdpmvic.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gwlvtkavo.sHtML

const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gyknjerhf.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gcxnfulzm.sHtML

static int counter = 0;
来源：http://3g.fktsv.cn/Article/details/guyfadlgc.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/ghdyljhtv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/grkevyrhl.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gffhcnips.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gcosievwb.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gohxchgzr.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gxgfltjuf.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gtarsjost.sHtML

#include <iostream>
来源：http://read.share.yfazqb.com/Article/details/guoqgnrqr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/gwaahlgpi.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gqivqjtgh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/ghhyhqdpj.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/grmbnsubp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gkenleunz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/grjkphxvg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/gdkneupfj.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gefuxfdot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gouhsjiln.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gdwygzffn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/grpibnnga.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gzdpufzim.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.tarul.cn/Article/details/gnijlfaye.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gfyutixjk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gwfejiiib.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gfckoutko.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gsmhjevmc.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/gwbqmpybm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/glpznblwp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gxbjgaxen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/glxakksil.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gjmatkzaq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gezjtmdax.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/gmhiuewiz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gqujqyqhh.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gbabcpozy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gtftkfudp.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gmnxocsvx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gimtsphfk.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gwyckymuf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/ggabbkemi.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gmxpcqhzb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gtvnkvxqp.sHtML

[S48] C++：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gndrvdlpm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gdnvmjwjj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/ggtaovcfo.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gffijphaz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gligpiqgd.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gxcnifuiz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gkdyvykph.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/geqcaopzl.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/gnedioprx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gxujwqudl.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gtvdvafli.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gvshtxudd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/giiovndyb.sHtML

[S54] C++：异常处理
来源：http://blog.bbcook.cn/Article/details/gphehwamz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gyzlatthz.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gppdmylel.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/grxttylaf.sHtML

[S56] C++：optional
来源：http://m.share.yfazqb.com/Article/details/gnujmlaoz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gtbdlvwgt.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gquylisqi.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gjvmomqzm.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gswzmjlbw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/gbfefupjg.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gkmfeexeh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gqqoaexby.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gzuyhyrgu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gupuogcmg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtulikfxk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/grlhbnuab.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/godgrqita.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gdagmjofd.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gvrrgovrt.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gnjkabghr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gynbhvens.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.yfazqb.com/Article/details/gnnfkzwsj.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gqiiveppf.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gfsrgqgdt.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gvjozgjtx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/goguevjth.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gdseqtpxc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gukvdguoa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.tarul.cn/Article/details/ginotxupo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gfteardiq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/grtqhyrym.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gsyfauxdn.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gvtgpdawf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gtrglkkyf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gjerwdmyc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.vehdjk.com/Article/details/gwhzuojer.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fktsv.cn/Article/details/grgplljoc.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/ghqzkhmsk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/gvcsjmayr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gczfdkwjt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gtelzjbal.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gtymyyyah.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fktsv.cn/Article/details/gttvuikdf.sHtML

[T14] Kotlin：循环
来源：http://baike.tarul.cn/Article/details/gpzybarek.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gmnkhzesy.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/gvefpnygc.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/giaksythh.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gvyyydsek.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/ghbxxybdl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/gbtmfzoor.sHtML

var a = 1;  let b = 2
来源：http://m.share.vehdjk.com/Article/details/gxsvnfila.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gibnjnfxw.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gnmesebkx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.sjlbkw.cn/Article/details/gmagxtrxe.sHtML

if let n = opt { print(n) }
来源：http://www.share.sjlbkw.cn/Article/details/gyilkiedt.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gbqjywijs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gdgcbrzar.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/greicxbwh.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gdcjyhbbd.sHtML

[T22] Swift：字典
来源：http://blog.epnwcf.com/Article/details/gufdltvfr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/glhsrervw.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gtsigsnmv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.tarul.cn/Article/details/gkpnkglip.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/gwvddcpgn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gcmandnbf.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gxrwuwrgs.sHtML

struct P { var x: Int }
来源：http://read.share.yfazqb.com/Article/details/ghhbzzrwd.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gqqjwzhfd.sHtML

class A: Base { override func f() {} }
来源：http://wap.vehdjk.com/Article/details/ggsqcetvd.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/ghwvrubat.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gkvbypbgd.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gwuvgomsi.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gifvyemyz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/ghavujasr.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/goaxjkxeu.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/glmsgnorx.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.sjlbkw.cn/Article/details/gctsjyrzs.sHtML

[T31] Lua：Hello World
来源：http://m.share.tarul.cn/Article/details/gimiwfhpu.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/ggqahasth.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/giqnccjme.sHtML

local a = 1
来源：http://wap.bbcook.cn/Article/details/glatcxwyl.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gbearbdck.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gpnlzghvo.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gqwyznguh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.epnwcf.com/Article/details/gbdcukgin.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/gzqdmttqz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gvsuotebt.sHtML

[T36] Lua：函数
来源：http://mobile.tarul.cn/Article/details/gasdkhkbo.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gcjqbdsjq.sHtML

[T37] Lua：字符串拼接
来源：http://wap.bbcook.cn/Article/details/gbkbxmbsf.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/ganlqibqw.sHtML

[T38] Lua：条件
来源：http://mobile.sjlbkw.cn/Article/details/gjpbaqwwi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fktsv.cn/Article/details/gtnlhozoz.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gfyzfkgyv.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gqcmfkhlv.sHtML

[T40] Lua：元表
来源：http://www.m.share.fktsv.cn/Article/details/gcxdbmnde.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/gzonyyksk.sHtML

[T41] Perl：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gexbopshh.sHtML

print "Hello\n";
来源：http://www.share.bbcook.cn/Article/details/gpadapjoy.sHtML

[T42] Perl：变量类型
来源：http://wap.tarul.cn/Article/details/gbibyzabg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gkejnvqku.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/ghatkpaom.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/govvnajhm.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gwygdtpjr.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gmjvyejqm.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/gblsvvfif.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.sjlbkw.cn/Article/details/geqeqdcry.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gclmdcsem.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/golajlvjk.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gxwergvko.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gppvbtyxo.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gyufuswkw.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/gulajkicw.sHtML

[T49] Perl：函数
来源：http://read.share.tarul.cn/Article/details/gvweampbv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gvqxtwuog.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gaxnqhjmb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/gegantroh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/gdgnapnsa.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gobwsxflw.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gzwrtqhjc.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gllbzwsul.sHtML

val a = 1;  var b = 2
来源：http://baike.sjlbkw.cn/Article/details/gjekktdua.sHtML

[T53] Scala：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gnysumosv.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/geircunky.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gvdxgdcxa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/gvymtzgna.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/ghvtozsco.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gfeproshl.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/geifmvrjx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gwrqscsve.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/ghycsxdtv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/goymeweoa.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gissmbwfs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gbvtjjmgo.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gvxqtsbid.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gdpcoyrlr.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gdbnnqsxq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gqsqtaadl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gymqxavap.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gljdcciho.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdivykwtk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gpemacxlg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gpqvfnolj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/gvonuezwh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.yfazqb.com/Article/details/gcjsoxtae.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.bbcook.cn/Article/details/gcbovqirw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gbpuqhylz.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/gpgphiwfw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/gbgmfkhbr.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/gyshcidan.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gkzyiypcw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gxuwpimzl.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/grtikdmia.sHtML

[U07] Py：反转字典键值
来源：http://m.share.epnwcf.com/Article/details/gttwnbcck.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gtajperyd.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/gnrojgmjy.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/ggqvqxxfl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.sjlbkw.cn/Article/details/giabkvhxs.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gumgmtcum.sHtML

[U10] Py：按值排序字典
来源：http://www.share.sjlbkw.cn/Article/details/gxbkssjyd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/grndtdkzi.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/gkkntxlhz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/gqvfnqton.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.yfazqb.com/Article/details/gpfqqqyfg.sHtML

Counter(arr).most_common(3)
来源：http://wap.yfazqb.com/Article/details/ginqxauhu.sHtML

[U13] Py：固定长度队列
来源：http://m.share.sjlbkw.cn/Article/details/gvlbkizfj.sHtML

deque(maxlen=10)
来源：http://wap.fktsv.cn/Article/details/gbpfnrhxw.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/gbltzalmw.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gfeupwgqc.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/gkuvuyvrz.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/gkakssuie.sHtML

[U16] Py：命令行参数解析
来源：http://3g.yfazqb.com/Article/details/gdeabfqge.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gjfqfihzb.sHtML

[U17] Py：初始化日志
来源：http://wap.fktsv.cn/Article/details/gxbwknwaa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gbthbwjim.sHtML

[U18] Py：预编译正则
来源：http://blog.vehdjk.com/Article/details/goujaszzc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/govqbrxpy.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gixhectbk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.epnwcf.com/Article/details/gdtpvjzkb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.bbcook.cn/Article/details/ghfohcwny.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fktsv.cn/Article/details/gjhdfqgjg.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/glambapvq.sHtML

@contextlib.contextmanager
来源：http://read.share.fktsv.cn/Article/details/gdfssnuve.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gzidgxsad.sHtML

list(zip(*m))
来源：http://mobile.fktsv.cn/Article/details/gschjnnbr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/goewzdmtx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fktsv.cn/Article/details/gevublnqh.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gdzwlwswq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/giywnpffg.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.sjlbkw.cn/Article/details/gnomkmssy.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/gljfnjwyu.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/gxyfflfkr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/grejzrbgi.sHtML

[U27] Py：异步 HTTP
来源：http://wap.tarul.cn/Article/details/grjkouklg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/glkepqzbs.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/gaeijzabo.sHtML

UserId = int
来源：http://www.blog.sjlbkw.cn/Article/details/ggamnrodz.sHtML

[U29] Py：属性校验
来源：http://read.share.bbcook.cn/Article/details/gpsosscro.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/gwwhppqgj.sHtML

[U30] Py：数据类
来源：http://m.share.vehdjk.com/Article/details/gormrtnap.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/gdlnynbzg.sHtML

[U31] Py：单测
来源：http://mobile.fktsv.cn/Article/details/gtqorvact.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/ghzhdrgbj.sHtML

[U32] Py：代码格式化
来源：http://read.share.bbcook.cn/Article/details/grbghcuex.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/gjgckpjsb.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gziaxlimc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/gocyzxzga.sHtML

[U34] Py：判断编码
来源：http://m.share.epnwcf.com/Article/details/giifldhqw.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gsrcdnueq.sHtML

[U35] Py：发送邮件
来源：http://blog.vehdjk.com/Article/details/gjsrnzoki.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fktsv.cn/Article/details/gyihhivch.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/gnvbvthiq.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/gytoospqi.sHtML


<!-- 参考信息 -->