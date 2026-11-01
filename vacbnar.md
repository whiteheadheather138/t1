代发 wailian999

int main(int argc, char **argv)
来源：http://blog.epnwcf.com/Article/details/gnqorkynm.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/ggyqnojwc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gxexitpdq.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gpianvged.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gkoklfyfn.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/grhzuffur.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/guyusapoy.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gkpxmgdne.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/grqgsdrzs.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/guxfgwwpd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gngdjuxkd.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gdnpqxuck.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gzmmkitbe.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/gwbifirks.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/gfbihkwlc.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/gpymcpmrx.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/glzqhckpm.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gbqagumys.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gedcvlfir.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gnevtbblr.sHtML

static int counter = 0;
来源：http://blog.sjlbkw.cn/Article/details/giutuabhd.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/gqsamvbvq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/gbvxhowct.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/grlpwrgqp.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/guzdpdtxh.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gmcgjhuxu.sHtML

#endif
来源：http://mobile.epnwcf.com/Article/details/gcmxahtok.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gahylhwrp.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/gfuxdeswd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/gycwvskyb.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfecfyjyy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/ghhbeowap.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gtxtfveuq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/govceyowm.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/gkbdekizg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/gfkayxyfg.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/gdxqfdqqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gaqkecvoa.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gankdpoim.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gpfzczzsx.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gnqdqnqad.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gxyjlscfq.sHtML

[S38] C++：排序
来源：http://m.share.tarul.cn/Article/details/ghpoftjuc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gokhqfrcc.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/grtpczffe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fktsv.cn/Article/details/gggjjokky.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gmxmzdjxo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/gwcxlwovm.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/gwhfqrmxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/glzbzxudh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/grvwujnoh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fktsv.cn/Article/details/gwdjmeifs.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/glmsirkvv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gwloawrsx.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/golonjuiw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gbdsfpsfs.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gkinblzmr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gbvuxlmvu.sHtML

[S46] C++：函数模板
来源：http://wap.yfazqb.com/Article/details/ghhdpoyge.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gmyfwuxsz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gztmnrgxw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gvfpjscrx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/grftqbgiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.bbcook.cn/Article/details/ggtzfwvxj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gupvonvpr.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/gnsenvcmj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gnmruevvv.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/guxiwehdo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gyoaxxogm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxfbdmee.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/gkqytmrgb.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.yfazqb.com/Article/details/ggpeghrgy.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gtqxmvokp.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/griqzymuy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gqydkhsfk.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gkjooshrr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gzbgjqrxk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxggjtir.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gtbbirqgy.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gdnqmqjuq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gdrymgnei.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/gjmahvbid.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gfbanvgmf.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gciwqsigh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gozkmajuo.sHtML

[S59] C++：静态断言
来源：http://blog.epnwcf.com/Article/details/grusahtin.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/glticcvxl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/glxohofak.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gryiqwfye.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmzcrepzg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gtvsresey.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glwjnkxcs.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/ghmmtvetc.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gtuugswgs.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gbdgwlthj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/gvfnklbgq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gogcdnqvf.sHtML

"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gjuyknovy.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gtdmsafvm.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/ghfhvljmk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/gjpimdwkr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.tarul.cn/Article/details/gcrnhqkiz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/ghrojuxrl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gwzvezxlz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gghnfireb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gkfnordte.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gokekyoyf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gyrdaiuow.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gphbdchic.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gnkgwadda.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/ggjaoackw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/gvqptedvf.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gxsxjbodt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gnkqrihui.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gyybwxewe.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gmelqkwnk.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gnjoppfnm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/gitdqwixx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.bbcook.cn/Article/details/gtnnvgasd.sHtML

for (i in 1..10) println(i)
来源：http://wap.bbcook.cn/Article/details/gxsatgifc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gqsbkrflq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gxzcqsryt.sHtML

[T16] Swift：Hello World
来源：http://www.blog.tarul.cn/Article/details/giuuvvknu.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gtoyweatv.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gvanmgcbe.sHtML

var a = 1;  let b = 2
来源：http://mobile.epnwcf.com/Article/details/ghlhxhwpc.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/grmrjozpu.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gevipvdpc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/ghqdaddjn.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gjmewfgvx.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gwjmnkiuw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gtiimuicr.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gppbthrjf.sHtML

for x in a { print(x) }
来源：http://www.blog.tarul.cn/Article/details/gtpzfxjtq.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/gxvdaszin.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/gyvidpimr.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/goawjjhzo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gswwfbqal.sHtML

[T24] Swift：闭包
来源：http://www.m.share.bbcook.cn/Article/details/gfoveatdy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/guuwtarap.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gbaebfkjt.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gwfeyzmya.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gjqloifit.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gydqdognv.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/glftrhict.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gdirehfrr.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/giyhbgqwg.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gdpojammg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/gpuisfeoc.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gjycyoynr.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/gddoibnow.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/gormmscow.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gikgnrzsl.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gqvqstkhn.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gwkerqmhh.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/gpypujdko.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/gebskkemk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/gtghdxrcm.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gkwvdpquf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.bbcook.cn/Article/details/glnjykrsu.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gwxcclbim.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/gwefygeeo.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gkgaajwhk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxzityfs.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gwqhpntek.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gszqvrkdu.sHtML

[T38] Lua：条件
来源：http://www.blog.vehdjk.com/Article/details/gmfrtkzgf.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/goiukjdhk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gfddbesgk.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/ggewgtrlz.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gxxwrjgfu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fktsv.cn/Article/details/gukmsqfpo.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gappvmsfw.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gbzegifbb.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gmqnczayd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/gpqqofkvj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gcbxpfcmf.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/gnlsuqfwn.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/gwfqydiic.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.epnwcf.com/Article/details/gnjdkacij.sHtML

[T45] Perl：数组遍历
来源：http://blog.sjlbkw.cn/Article/details/gbpircncf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.bbcook.cn/Article/details/gwvobcylw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/gnweksmpz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/ghrukwunz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gcuhdoebx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gfcasictx.sHtML

[T48] Perl：正则替换
来源：http://blog.vehdjk.com/Article/details/gcoerlqtz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/grexgagqp.sHtML

[T49] Perl：函数
来源：http://3g.epnwcf.com/Article/details/ghjmvfhsy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/ggxweunsc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gzvsrpkzb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/gprckbped.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.tarul.cn/Article/details/gyyyddrbj.sHtML

[T51] Scala：Hello World
来源：http://baike.fktsv.cn/Article/details/gxnwspajt.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gwetqrahk.sHtML

[T52] Scala：变量
来源：http://wap.tarul.cn/Article/details/gbovfkssu.sHtML

val a = 1;  var b = 2
来源：http://read.share.tarul.cn/Article/details/gnmgamwws.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/gisjljunp.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gxfgdirlf.sHtML

[T54] Scala：集合映射
来源：http://mobile.yfazqb.com/Article/details/gdujgqnqr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvvxhrneb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gkjctoaqe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gjupoibji.sHtML

[T56] Scala：样例类
来源：http://blog.sjlbkw.cn/Article/details/gxienrrrx.sHtML

case class User(name: String, age: Int)
来源：http://blog.bbcook.cn/Article/details/gdihlhqqg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gtnknqeov.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gdalqlcth.sHtML

[T58] Scala：函数定义
来源：http://3g.tarul.cn/Article/details/gqmlkfomt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.epnwcf.com/Article/details/gxoatjjof.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/ggjlmjerd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gaueyfshr.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/gokgzyxsq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/gxyrdgaow.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvwkdgdso.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/gppmxryjs.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjhcwhsly.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcxydsue.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.epnwcf.com/Article/details/gwaxnthhs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gsnvpxxjb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gedvhuehu.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/goklnxxfi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gxuibfkng.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gxsmepnxp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gwudzyqnh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/gugispuzv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/ggxbzxjqm.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/ggdiaucil.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gmdjxyiff.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.vehdjk.com/Article/details/goalafwsu.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gthvrrpwn.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gywbutlor.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gdtcwqgfv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/gbjnkallw.sHtML

max(d, key=d.get)
来源：http://baike.yfazqb.com/Article/details/gqzvvljru.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/guergitul.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/gbzgtfgmz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.sjlbkw.cn/Article/details/gbmdnxpty.sHtML

(x * 2 for x in arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmglujhzr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gmrccsyvy.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/gsbciqrrk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/ghblbzaep.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/gdkehcdit.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gurpfhids.sHtML

defaultdict(list)
来源：http://baike.yfazqb.com/Article/details/gahhjpqui.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/giehnsack.sHtML

t = time.perf_counter()
来源：http://www.m.share.epnwcf.com/Article/details/gprlxkvmb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.yfazqb.com/Article/details/gxbutkmvq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gjjhfmpjv.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/goqrloqmy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/grvgvccey.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.bbcook.cn/Article/details/gfxmrbdhr.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/gcgggakkb.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.sjlbkw.cn/Article/details/grnrhicsf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.epnwcf.com/Article/details/glvurznvn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.vehdjk.com/Article/details/gzhknsgdz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/gajvziwru.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/glokgugxg.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gtqcblujd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.yfazqb.com/Article/details/gztycjygu.sHtML

list(zip(*m))
来源：http://blog.sjlbkw.cn/Article/details/gxynaioip.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gsgaqzfkb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gxokyjfxy.sHtML

[U24] Py：路径操作
来源：http://www.m.share.epnwcf.com/Article/details/gxtnomnao.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gukrkutfp.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.yfazqb.com/Article/details/ggitcnvjc.sHtML

csv.DictReader(f)
来源：http://blog.tarul.cn/Article/details/grzcedjhg.sHtML

[U26] Py：并发下载
来源：http://read.share.bbcook.cn/Article/details/gatxarylq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gofryciiu.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fktsv.cn/Article/details/gxcumqazc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gprejtzje.sHtML

[U28] Py：类型别名
来源：http://blog.bbcook.cn/Article/details/gumuwvbxi.sHtML

UserId = int
来源：http://wap.yfazqb.com/Article/details/ghglvhfej.sHtML

[U29] Py：属性校验
来源：http://www.blog.epnwcf.com/Article/details/gfkluyuij.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gzopaycvw.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxcauqea.sHtML

@dataclass(slots=True)
来源：http://wap.fktsv.cn/Article/details/gczazkdaf.sHtML

[U31] Py：单测
来源：http://www.m.share.bbcook.cn/Article/details/goypqmnhw.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/gxwcrccon.sHtML

[U32] Py：代码格式化
来源：http://blog.yfazqb.com/Article/details/gjjgljunp.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gamqxojoc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.epnwcf.com/Article/details/guavqoulr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/ggsyqvsbp.sHtML

[U34] Py：判断编码
来源：http://www.blog.epnwcf.com/Article/details/gtcrdvfnn.sHtML

chardet.detect(raw)
来源：http://www.blog.vehdjk.com/Article/details/gevttohvg.sHtML

[U35] Py：发送邮件
来源：http://www.share.bbcook.cn/Article/details/gusmohprv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.epnwcf.com/Article/details/ggtenqtkn.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/ghicrjdtc.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fktsv.cn/Article/details/graqtfpai.sHtML

[U37] Py：读写 Excel
来源：http://3g.epnwcf.com/Article/details/giasroetq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/gnrgufwza.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.bbcook.cn/Article/details/gxrpvazeg.sHtML

Path(__file__).resolve().parent
来源：http://blog.bbcook.cn/Article/details/gdeqbxisn.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.tarul.cn/Article/details/ghcdecwxo.sHtML

sys.stdout.isatty()
来源：http://baike.yfazqb.com/Article/details/ggtxbxskc.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.yfazqb.com/Article/details/gdbllhwtz.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gmkaifgjt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fktsv.cn/Article/details/gqdipxyla.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.vehdjk.com/Article/details/gsrjidtog.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/glanvncnj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.bbcook.cn/Article/details/gkazldvuz.sHtML


<!-- 参考信息 -->