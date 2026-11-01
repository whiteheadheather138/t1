代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/gjuwvibxh.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gfmeudulm.sHtML

(double) a / b
来源：http://wap.yfazqb.com/Article/details/gigwyavxp.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/ghjwhlbjy.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gqyclnvvb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gzddbcmso.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/giveijsqu.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/ghblglqtu.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gqbugwvvb.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gmljmcdqd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gljavhvgx.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/gduydvvdu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gpwutxoor.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/ghefklfkt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gknduczsb.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gijcxjfig.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/gnhlshzzc.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/gwhzykubh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/glojvokhm.sHtML

[S24] C：获取本地时间
来源：http://3g.bbcook.cn/Article/details/gbgthioup.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gwzmaogzl.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gulmpatng.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/ggnlodrbd.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gejttntoq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/gbplsirym.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/glvarpynr.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gwygichfk.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gixsfzmzk.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gqlhsudeb.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/giadesgfn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/ghbuwdrbs.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gmxxrfety.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/gveiomtdf.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gqspymoci.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/ghllmkazl.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gomkyfvcc.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/ggqqrfxba.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/glfvujfep.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gmvxpsgrh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gdmbtzpxt.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gvydpcocx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gctpkhdcn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.vehdjk.com/Article/details/gnmptlytn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gbkglarxt.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/gltdmhmrl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gfixrkdgg.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gfbvfhthx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gnnpngejs.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gscoguxox.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgwdbvah.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gtyhugbow.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/ggiexgfaj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.vehdjk.com/Article/details/gsrhutjto.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gervfhbcb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/ghtunlycd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gejvjwhtv.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gaeywkdqw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/gdkcxpwzr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/glyynvwlv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/ggbxbwtyp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/ghuvgzeld.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gwlkjwliv.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/gpxagqfbd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/ggnggbsuz.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gmynwaidh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/gaeqidklc.sHtML

[S46] C++：函数模板
来源：http://read.share.sjlbkw.cn/Article/details/gwpqhpzyg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/gxjlahbtd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gtdgzdmnc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gcnkxgpmj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gqlibiczb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/gcohldxak.sHtML

while (std::getline(in, line)) { }
来源：http://3g.epnwcf.com/Article/details/giyagetth.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gujapksyk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gebppefrw.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gpplmuhlr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/glrxauehk.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gaawzmzem.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gzasgmgjf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fktsv.cn/Article/details/gbsvbhkex.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fktsv.cn/Article/details/gzvgsdmux.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/glyopqcps.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gsmjqyqrm.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gjkvqkadr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/giuulqpfr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/gofxbzvvc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gtqtraypr.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gexfmowrj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gylcsehif.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gmttwnaxx.sHtML

constexpr int N = 10;
来源：http://m.share.fktsv.cn/Article/details/gkqvylsqv.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gmfdyxetq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gtidgemxx.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/gvihlggtu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/grmkluvmc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gcfulflgg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gbugtlrje.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfwzkotoc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gnkwdpnwn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbaccprjx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/giddahhjj.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gnqwldqal.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gmchksumc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/grbnkxtxd.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/glhoppmah.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gucsflqnv.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gebtubwer.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/gksonzwpi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gkfqfkirb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/gnkdilits.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gissnuldk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/ghevbufeb.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/geavgjfhy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.yfazqb.com/Article/details/gsdugyoko.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/ghoupdwvj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/grqkgtdcg.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gnatmuzci.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/ggmtcdddu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gmtqwqyse.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/gmhfohwut.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/guklucvrx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.vehdjk.com/Article/details/gvkddltpl.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gyqklbibf.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/ggfjkfcvj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gwsvimgxj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/ggmueqgyk.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gftiqlnwu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gtcoqdidz.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gknamiuqf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gmkgzhonl.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/givybejyt.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gaalprgln.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gnkjrsvcn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/geqrzuipr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gfbxzcyic.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gvkcpwarw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gtgfnmnqr.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/gicxddpvm.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gwpnirgvw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/giflqodos.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/gyelzfbrl.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gftchulwu.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/glpypjqqk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gacoeihff.sHtML

[T23] Swift：函数
来源：http://read.share.tarul.cn/Article/details/gyremaibp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.yfazqb.com/Article/details/goodcyylz.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/grhmqyxqc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gpbgqxdcz.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gasjarlar.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/guhnavhzv.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gubxftfxe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/ggutatmfi.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gtkqabtmq.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbgzdlyw.sHtML

[T28] Swift：枚举
来源：http://3g.epnwcf.com/Article/details/grvbpjpnu.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/gufermmcw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/gffakeudf.sHtML

guard let x = opt else { return }
来源：http://baike.tarul.cn/Article/details/gzuyxslon.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/gaiaddplh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/gulvrdmib.sHtML

[T31] Lua：Hello World
来源：http://www.share.bbcook.cn/Article/details/gkbtttecq.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gzhyslyqn.sHtML

[T32] Lua：局部变量
来源：http://3g.sjlbkw.cn/Article/details/gilynzlyc.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/grmmajiuz.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/gdkyprdat.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/grixoosfj.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gogiwzcad.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/gbpnhunns.sHtML

[T35] Lua：字典表
来源：http://read.share.vehdjk.com/Article/details/gmdzyprws.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.tarul.cn/Article/details/geiyizfea.sHtML

[T36] Lua：函数
来源：http://www.blog.bbcook.cn/Article/details/geqixuvgp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.epnwcf.com/Article/details/gtastfcbc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gpcuzgvbb.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gwriicieq.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gqlwzrafb.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gxubbfuzo.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gewqfotgm.sHtML

string.find(s, "%d+")
来源：http://mobile.bbcook.cn/Article/details/gouoxruzt.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gkgkagqqj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gbplftwsc.sHtML

[T41] Perl：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/grvynuzqg.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gsyfdeowi.sHtML

[T42] Perl：变量类型
来源：http://blog.tarul.cn/Article/details/gqfqoblbm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/gsfdvwedr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gijcujjib.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gzqjxvyef.sHtML

[T44] Perl：条件
来源：http://wap.tarul.cn/Article/details/gxmxnkkiq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gjzsbzsqu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gmutkmdug.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.epnwcf.com/Article/details/gcilblyxh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.sjlbkw.cn/Article/details/gdtvhjtpv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gcjetkxjv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/gtwatoxdu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/gzokegiwq.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/gbqlyydag.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.bbcook.cn/Article/details/gcqfvlgid.sHtML

[T49] Perl：函数
来源：http://mobile.tarul.cn/Article/details/gojhgwlxo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gtnkhwvyv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqfrcbru.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gquiefbrr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/glnotbbep.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gxsoredps.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/grjiskvjw.sHtML

[T52] Scala：变量
来源：http://www.m.share.fktsv.cn/Article/details/ggenndlfk.sHtML

val a = 1;  var b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gsiwelsrf.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/gdgvpjkgx.sHtML

s"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gnoeooaue.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gwiuoomhf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.yfazqb.com/Article/details/gqyzihflt.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gwstbyljx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gpbybxkly.sHtML

[T56] Scala：样例类
来源：http://m.share.yfazqb.com/Article/details/gbdzanbrt.sHtML

case class User(name: String, age: Int)
来源：http://3g.epnwcf.com/Article/details/gcwchngzt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gjgqjokkd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/ghfsjdwga.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gmbpzgvqj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/gilsluihb.sHtML

[T59] Scala：循环
来源：http://3g.sjlbkw.cn/Article/details/gmlqobueg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gjwepwffn.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/ggcxrmuzn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gjqwbcmrc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gynrmqutw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gfpbuxsau.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwklmbdhv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/grdipbrdu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.tarul.cn/Article/details/gdjwkkieh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.epnwcf.com/Article/details/gbfshldoo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/gowalzduc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.tarul.cn/Article/details/gunidegnk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/gvzzcbmqj.sHtML

[U04] Py：变量调试打印
来源：http://blog.tarul.cn/Article/details/getalmpxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gwlrnxpnd.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gfnmtxudj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gvwaqsbya.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gassjvvjg.sHtML

{**a, **b}
来源：http://www.m.share.yfazqb.com/Article/details/gkydtjxdo.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fktsv.cn/Article/details/gqgcnwqag.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/gxabxykdg.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gpnjftdtc.sHtML

[y for x in nested for y in x]
来源：http://www.share.vehdjk.com/Article/details/gwncofghw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gbkfckrvg.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/glawhhssp.sHtML

[U10] Py：按值排序字典
来源：http://www.share.vehdjk.com/Article/details/gyvankara.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.tarul.cn/Article/details/gjrvfqska.sHtML

[U11] Py：生成器表达式
来源：http://blog.vehdjk.com/Article/details/gvtyvpavl.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/ggjcwnbez.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.epnwcf.com/Article/details/gzvjpacjc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gkjhdpeqq.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/gxnruotko.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/geoedtuwq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gdykchwbn.sHtML

defaultdict(list)
来源：http://www.blog.sjlbkw.cn/Article/details/ggwuozyne.sHtML

[U15] Py：高精度计时
来源：http://www.share.epnwcf.com/Article/details/gcfviilcs.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gfvaeguck.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/gnfaoppel.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/gdvmdpgqb.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/gmmlfjqrt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.tarul.cn/Article/details/gdtpdwclk.sHtML

[U18] Py：预编译正则
来源：http://blog.vehdjk.com/Article/details/gcqgvprtc.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/grhtltwde.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gjywjdvxf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gyfmflnpl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gnzarisyh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/grsyptywg.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.vehdjk.com/Article/details/ggywyjmwz.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gigvnkrca.sHtML

[U22] Py：矩阵转置
来源：http://baike.epnwcf.com/Article/details/gtrmjnpdh.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/giqyqpeun.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/gxrsitukf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gslwtifck.sHtML

[U24] Py：路径操作
来源：http://mobile.vehdjk.com/Article/details/gxajhgzvs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gjthlsfzc.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/gysskaajl.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/gfpbclmpv.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/guncyusdg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/gklenssna.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/gpiobjkro.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.vehdjk.com/Article/details/gtffridkt.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/gllmjfebg.sHtML

UserId = int
来源：http://read.share.bbcook.cn/Article/details/gewapphia.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/ggovwrkiw.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/gflfzvcdt.sHtML

[U30] Py：数据类
来源：http://m.share.yfazqb.com/Article/details/gaefqjbon.sHtML

@dataclass(slots=True)
来源：http://wap.yfazqb.com/Article/details/gabjzbgzq.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/gxkitcwyt.sHtML

python -m pytest -q
来源：http://baike.yfazqb.com/Article/details/gprwtzlbq.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/gqozkngir.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.yfazqb.com/Article/details/gtwrchipy.sHtML

[U33] Py：打包发布
来源：http://www.share.vehdjk.com/Article/details/gzapcybve.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.vehdjk.com/Article/details/gamobzcha.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gnopkgmhn.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gvmsndsbr.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/gchyebczm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/gdpfemajk.sHtML

[U36] Py：定时任务
来源：http://www.blog.fktsv.cn/Article/details/gzfuuccpc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gpvtstlco.sHtML

[U37] Py：读写 Excel
来源：http://www.share.tarul.cn/Article/details/gxdhvsnbq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.vehdjk.com/Article/details/guswcezuw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/gkllwsedc.sHtML

Path(__file__).resolve().parent
来源：http://wap.epnwcf.com/Article/details/gtrltxkjs.sHtML


<!-- 参考信息 -->