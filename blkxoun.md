代发 wailian999

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gkoqlokdi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/ggeoyxbeg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.epnwcf.com/Article/details/gjrzoiqoy.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gpupuopmu.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gsenxwlzu.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gjwlmfwzp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/ghmysjnpv.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gdpsjlocp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/ggreovhmm.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gtdrtioaf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gpsmbmmht.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gtmbkhveh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/gkoyouwsa.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gqtddwgux.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gkvcswcfm.sHtML

[S24] C：获取本地时间
来源：http://m.share.tarul.cn/Article/details/gyjuqnnro.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/ghjjyucbo.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gfcgwfcyd.sHtML

memcpy(dst, src, n);
来源：http://baike.bbcook.cn/Article/details/gcievybjq.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gfrhqaerw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fktsv.cn/Article/details/gosbkuodf.sHtML

[S27] C：定义常量
来源：http://3g.sjlbkw.cn/Article/details/gdsiekkoh.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gkegvxvyh.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gjhnqunys.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/ghcsqjtri.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/geddhtbgz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/glcxqryyz.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/goofwypxz.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/gquhqhkye.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gchulpjzr.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/ggbmlhymy.sHtML

[S31] C++：Hello World
来源：http://baike.fktsv.cn/Article/details/gmsofgngo.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gxkqfotbo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gxtklwtqv.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gvjcmojjk.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gvdhoatci.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gnjpmolfp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.epnwcf.com/Article/details/gzfkgapbr.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/grlmrcdsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/ggpyxqugm.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gtxxfqmrg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/guptdxatk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.vehdjk.com/Article/details/gjmkcwowy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gwhvsqthv.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gemsfaisi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/gmvkdkuqp.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gxbabrlpc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gnyaqwxmv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gwbczckxm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gdbtzjnaq.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gnrfxotpv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gwnixlcjn.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gybstpnts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gxultvzpn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gbvtxbdji.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.epnwcf.com/Article/details/gjedtraaq.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gklcqjpvp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.sjlbkw.cn/Article/details/gawzdmkyz.sHtML

[S44] C++：引用传参
来源：http://blog.tarul.cn/Article/details/guhmfiasc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gublmpysg.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/grtcczrfz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/glqnlwxry.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/gachzeiek.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/gleompzcr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gtdbdfjyc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gsomcusmj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gzmpxoaoy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gvwdlpncs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/grrrouphj.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgjyeibh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gjmysnvxj.sHtML

[S50] C++：格式化数字
来源：http://baike.tarul.cn/Article/details/gnbzshcoc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gdackhpqm.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gisujvqkb.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gdbrntxxj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.tarul.cn/Article/details/gsyiwvcmf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/grhatjcxj.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/guknapplp.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gcwqmyrbl.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gkjbuzxme.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gehrjiadz.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gwvtvfytm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gnewmtlhy.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gejfthemr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gmhtpezjm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.sjlbkw.cn/Article/details/gwymiztop.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gidthvoee.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gpvomwxtw.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gpwmwmxbh.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gnqxyaqvz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gvoalexfe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gixwastlg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/gxlqiboyg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwgrmhcif.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gxgadkqdn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnwpffjsm.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gfvjggrev.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gtnvrjmvl.sHtML

[T02] Kotlin：变量
来源：http://baike.vehdjk.com/Article/details/gihydsadw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/ggxfdqudt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/gfuosoubk.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gsuuliyjq.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/ggmmcssre.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gsqiyzjnf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gatbhrnrr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gnjzkawkg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/glzmruoxf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gkciuubiy.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.epnwcf.com/Article/details/gqijrrvym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/grvxbapas.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gjjmkixfz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/guwauvluz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/goeasntex.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/gyotinyse.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gkfqjfbxe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.bbcook.cn/Article/details/gaishkrrc.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/ghxdhossx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gfiexowis.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/gsjsvozik.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gsrrdtkqw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gpjuxbcuq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gueiwirhh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gnumiqyyh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gcdlyhvqe.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/gelqlstis.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gfwvzvkhw.sHtML

[T16] Swift：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/ghgkxzenu.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gbubdnxjg.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/gnsrvmsma.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gjltzcakd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/giyrbczmb.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/geqyoicci.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gxqyvckkc.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/gyfpsifwv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fktsv.cn/Article/details/giwifjtwq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gfylnwipr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gudderapd.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/geewxtuez.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gqvtlcwcq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/giwccvddz.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gnbhxnhtc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gewpbulvd.sHtML

[T24] Swift：闭包
来源：http://m.share.sjlbkw.cn/Article/details/gxryvsyfv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.yfazqb.com/Article/details/gtqkpvwfy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gvvxbcneg.sHtML

struct P { var x: Int }
来源：http://3g.tarul.cn/Article/details/gftaevbvn.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gmlqogaqs.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fktsv.cn/Article/details/gyngdqhus.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gcyqkncxe.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/gdgjqvuyg.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gbqageyxj.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gktwhcuss.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gpgafytck.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gwoqddpun.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/geyftmiqt.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/gbxdpdatm.sHtML

[T31] Lua：Hello World
来源：http://www.share.tarul.cn/Article/details/gpzmjhteb.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gjuuosnqy.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/gqcmittnw.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/gftdkkdct.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/gryjcfetu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/grthdnucr.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/ggwkretat.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gsdveqbck.sHtML

[T35] Lua：字典表
来源：http://wap.bbcook.cn/Article/details/gkcmrmpll.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.sjlbkw.cn/Article/details/ggtbnmkbg.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/ghucnkpoi.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gtmxhduzi.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gmyjnqtgr.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/grcowydgi.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/gbldpjfye.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gzftrrggg.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/ggvamgwyo.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gtfdtkive.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/gxanlvdsl.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/grmkeeqya.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/gxcxshoxe.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/gwbvlfvhr.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/guybabonm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/gmjbhwgbv.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/gtmijijom.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/grgrmcmfq.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gwxappxma.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.epnwcf.com/Article/details/gfypwgnqe.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/ghwjkkoob.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gqhularpt.sHtML

[T46] Perl：哈希操作
来源：http://mobile.epnwcf.com/Article/details/gclynbhul.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gehokzbzd.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/gvfbzscfx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gxyohhmyf.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/glhdacokv.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gdxyrrmik.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gpsrqwemw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gpairzfot.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/ggymasijw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/ghwavzubw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gkpdbkgam.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/gyicmajdf.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gyxjfxtyk.sHtML

[T52] Scala：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gaycgfitg.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gjrwyxpfy.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/godeelqhe.sHtML

s"值: $b"
来源：http://m.share.bbcook.cn/Article/details/goirdsbxr.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/grlyvtlfg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gnfpzrjzj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gjhmlbrpn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fktsv.cn/Article/details/gsaxkqbrx.sHtML

[T56] Scala：样例类
来源：http://blog.bbcook.cn/Article/details/gkbvhqvac.sHtML

case class User(name: String, age: Int)
来源：http://blog.fktsv.cn/Article/details/grizevxsn.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gxjlczgen.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.tarul.cn/Article/details/glyzaavvy.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/gcslwsguv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gxwxamvod.sHtML

[T59] Scala：循环
来源：http://baike.sjlbkw.cn/Article/details/ggfmyasef.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gsgvleygc.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/grxcsbdma.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gukutzqdo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghpmbuttt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gdmcbjdvf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtqpiyntw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/gacdqrion.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.sjlbkw.cn/Article/details/gjkudnksf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.sjlbkw.cn/Article/details/gbuytfvxs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.yfazqb.com/Article/details/gvyvdqyki.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gsttklrin.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gscadfchm.sHtML

[U04] Py：变量调试打印
来源：http://mobile.bbcook.cn/Article/details/gpewxvwhz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.bbcook.cn/Article/details/gnjyqmpmt.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.bbcook.cn/Article/details/gcjpufkgk.sHtML

list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gbsfemput.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/gawjzxlzy.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/giqrrbdtz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/gxrupwbaf.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/glmeqooid.sHtML

[U08] Py：展平二维列表
来源：http://m.share.bbcook.cn/Article/details/gfpmpfyuk.sHtML

[y for x in nested for y in x]
来源：http://read.share.sjlbkw.cn/Article/details/gjcrhguzo.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.sjlbkw.cn/Article/details/geeaoaazs.sHtML

max(d, key=d.get)
来源：http://www.m.share.vehdjk.com/Article/details/gdtipllxb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.yfazqb.com/Article/details/gznsaseae.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fktsv.cn/Article/details/gvmwfkzds.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fktsv.cn/Article/details/gwnicpzrq.sHtML

(x * 2 for x in arr)
来源：http://blog.yfazqb.com/Article/details/gdcqamobi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fktsv.cn/Article/details/gxccfdlxe.sHtML

Counter(arr).most_common(3)
来源：http://3g.fktsv.cn/Article/details/gaunzaqac.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gpvbmyigo.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/glaintrau.sHtML

[U14] Py：分组收集到列表
来源：http://wap.bbcook.cn/Article/details/gcycvqzyk.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/glstndnzn.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gmrblmtzr.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/grklbzuxc.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.epnwcf.com/Article/details/gdkvwjgnx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fktsv.cn/Article/details/gkftixkqc.sHtML

[U17] Py：初始化日志
来源：http://www.share.yfazqb.com/Article/details/gbexzyadd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gvivkmssc.sHtML

[U18] Py：预编译正则
来源：http://wap.yfazqb.com/Article/details/gvzpfqwmf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.vehdjk.com/Article/details/gpxtyhfbt.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fktsv.cn/Article/details/godeqegfm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gtjoadgoe.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gftcgnxut.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtswgvcv.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.bbcook.cn/Article/details/gnwjsdgos.sHtML

@contextlib.contextmanager
来源：http://read.share.vehdjk.com/Article/details/gkjpapveo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.epnwcf.com/Article/details/gdbfkgugn.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gonziwcma.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/gbemjslhj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.bbcook.cn/Article/details/gqmfkviwd.sHtML

[U24] Py：路径操作
来源：http://3g.vehdjk.com/Article/details/gpiddmgxf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gccelutle.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gekihhwio.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gvbngpukt.sHtML

[U26] Py：并发下载
来源：http://blog.sjlbkw.cn/Article/details/gudqgmxii.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdlqbtrj.sHtML

[U27] Py：异步 HTTP
来源：http://blog.yfazqb.com/Article/details/gcifsaeuq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.tarul.cn/Article/details/gfxzqkifk.sHtML

[U28] Py：类型别名
来源：http://www.blog.fktsv.cn/Article/details/gvifdwpyh.sHtML

UserId = int
来源：http://www.share.tarul.cn/Article/details/gfbkdqrte.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gliqcfkhg.sHtML

@property 与 @x.setter 配合
来源：http://m.share.yfazqb.com/Article/details/gnkpzplzh.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gupuhsgqe.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gztcbhitg.sHtML

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/gxhipzruq.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/gupfssiiq.sHtML

[U32] Py：代码格式化
来源：http://read.share.yfazqb.com/Article/details/gfxnkyunn.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.sjlbkw.cn/Article/details/gywkvxnbq.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/ghqxmvpqs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/ggvobtagq.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gwwazbssp.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/gsrjzloyr.sHtML

[U35] Py：发送邮件
来源：http://baike.fktsv.cn/Article/details/ggetuagmc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.epnwcf.com/Article/details/guaoqzpqt.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/ghavleltn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/ggskzjeau.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.vehdjk.com/Article/details/gmstayahp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.tarul.cn/Article/details/gdjpwkdqf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.sjlbkw.cn/Article/details/gozyezwlu.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gpmsfudps.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/gfruszktx.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gsssagwau.sHtML

[U40] Py：打印到标准错误
来源：http://baike.sjlbkw.cn/Article/details/gokrkwien.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gcsknkdlw.sHtML


<!-- 参考信息 -->