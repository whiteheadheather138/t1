代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gfyvomroj.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gnerqomen.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/ghhwjcpxs.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/glvuorttw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gbqqzopzi.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/ghsgubsym.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/ghaxmgaib.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gwddlhzop.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/goflccztk.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gbgobitaf.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gvsfggdxl.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gnpjokkhu.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gdsqfetvu.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gkkywlnca.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gfyyfgdwj.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/gpryjwipf.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gynriqhnv.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gwhtvugkd.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gfnwnbtde.sHtML

[S31] C++：Hello World
来源：http://blog.bbcook.cn/Article/details/gycaqhpyo.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/gbcdydxpx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gdzsctdkm.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gesfahicz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/guquatfbg.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/grwcyppvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gozmdgoos.sHtML

[S34] C++：遍历 vector
来源：http://3g.tarul.cn/Article/details/gbimkbhdn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gtnxohdfi.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gkzljckvo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gsujzbhxc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gkxvwhets.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gaelajsqf.sHtML

[S37] C++：set
来源：http://3g.epnwcf.com/Article/details/gjdvflfae.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/gfqorapeb.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/grirdokqh.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gkdkagsfh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gngcujssy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/gerwyehnd.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/gqhydogtb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/gqgsfoggn.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gqjbkzqax.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gitdfhzxs.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gbmecbtqv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gbycwicgc.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gmpglhiga.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gqrtxupvf.sHtML

[S44] C++：引用传参
来源：http://www.share.yfazqb.com/Article/details/gbrfcgfgn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gbyklnglf.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gnmkxrxbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gkylwvarx.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gnrukrlgc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/guiuhleut.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gckqtahlf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/ghzeapxih.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gehneblfb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gtvctphfe.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/ggckcxzrx.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/grdoyevxl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/geexqmlpx.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/glocinwnd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fktsv.cn/Article/details/gefijyuki.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/gaxzncxgd.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gzvbxzfqb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gkzstgyfo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gunhpfcii.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gqessxqfz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.tarul.cn/Article/details/gygprlxoc.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gyqisisla.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gcsgxpwrm.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gjtibrpis.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gspqtfnak.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gkcjvwtty.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.epnwcf.com/Article/details/garqytjvm.sHtML

[S57] C++：编译期常量
来源：http://baike.tarul.cn/Article/details/gpmflunpt.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gtflnbcva.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gzcnrqhck.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gthdgjfpo.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/grujhzrow.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gkybgfzyc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gkdcosdwt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/ggbtisnpn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdosrnpwf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gkywcryuw.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsahcdjeg.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gkjdoynuh.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gqgotgrtl.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gouzulmye.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gcvjfvimc.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fktsv.cn/Article/details/gkljxyspj.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gzmrxmdkm.sHtML

[T04] Kotlin：空安全
来源：http://wap.fktsv.cn/Article/details/gtkaoroja.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/grrapkjzi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.yfazqb.com/Article/details/guzhgegnd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gxcyvaodo.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/gmvvwvjrf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/goiqhnrnt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.tarul.cn/Article/details/gntqloqoi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/ghkphgvyu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/gtirjssly.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gttafucqf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/ghryxfuhn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.tarul.cn/Article/details/gzixaxpus.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gaewbbmka.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.tarul.cn/Article/details/gtiwnfrou.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gcabnxyfv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gfqcsotrz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gcqzlybtu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gmwvhjzgv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gakjkpitq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gqdkbgzhc.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gyznsbmxd.sHtML

for (i in 1..10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gcpttrsiu.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gnhextrbr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gberfhhqc.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gjtlammic.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/genlibpti.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/ghkwlulng.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/glueoghfr.sHtML

[T18] Swift：字符串插值
来源：http://3g.bbcook.cn/Article/details/goerwpevn.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gwslgvqmm.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/geqawktun.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gpskmmzcg.sHtML

[T20] Swift：数组操作
来源：http://3g.tarul.cn/Article/details/gbpeyxjyf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gdvhvrbae.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gfpmbuicq.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gabiznkfe.sHtML

[T22] Swift：字典
来源：http://read.share.epnwcf.com/Article/details/geckdxpux.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.bbcook.cn/Article/details/ggngjklma.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/ghzslclcl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gmwhezrns.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/gpqrkugdo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gafgpybuz.sHtML

[T25] Swift：结构体
来源：http://blog.sjlbkw.cn/Article/details/ghkwjfqpx.sHtML

struct P { var x: Int }
来源：http://www.blog.yfazqb.com/Article/details/gyrvfrknj.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gpuzkkxhs.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/gbkmtsftz.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gpasdxvvp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.epnwcf.com/Article/details/gnotonhkg.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gaghsrtkr.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/gpuhsudnl.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gmnspdjll.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gwgpqngjz.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gsohqoxsy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/gucasxyol.sHtML

[T31] Lua：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gyokgeyeg.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gdytuuzzi.sHtML

[T32] Lua：局部变量
来源：http://www.blog.vehdjk.com/Article/details/gqgbgpbtb.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gfxlbvvlb.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/giaqxbycc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/gwseradqn.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gxihqaueb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gbiqkzmsm.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/gmnlirvdh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gxufzqlhj.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gsniqsoju.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gkizmnauh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/gtymoiiuy.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gponujyja.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/ghqolhzbv.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gphzmbtrt.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gsyzlaydr.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/gieltuiha.sHtML

[T40] Lua：元表
来源：http://mobile.yfazqb.com/Article/details/gqpplmvox.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gjibeifnf.sHtML

[T41] Perl：Hello World
来源：http://wap.tarul.cn/Article/details/gtnfistvc.sHtML

print "Hello\n";
来源：http://read.share.epnwcf.com/Article/details/gwpoyjqrn.sHtML

[T42] Perl：变量类型
来源：http://read.share.yfazqb.com/Article/details/gemldbuiq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.sjlbkw.cn/Article/details/glihbfdfh.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gjmlcybec.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/ghiavsivc.sHtML

[T44] Perl：条件
来源：http://wap.tarul.cn/Article/details/gkkksitxs.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gaaqooyxl.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fktsv.cn/Article/details/gdcatubgg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/guneitpfx.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/glbxigois.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/gigdghxcu.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/ghbxrvchv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnchvueij.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvgfeutk.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gjzgezdda.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gyuaicovd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gfroiyfmg.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gshpeyhvj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gcegayxxz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.tarul.cn/Article/details/gpdfojxfd.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/gachbmeke.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gfhviwyec.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/givnpxmrv.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gwqnqodxr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwxxzbtg.sHtML

s"值: $b"
来源：http://wap.fktsv.cn/Article/details/gjmqfvpru.sHtML

[T54] Scala：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gmvxyewck.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/giszlvpgz.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gphhtnewr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/gazveocfa.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gkrbrhtrm.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gwpfgvlvh.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gjdylvbpq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gvpnakhqo.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gxoemyhgt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/grspekinm.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gpxyizhct.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/guklkwjrg.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gjjqkbegh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.epnwcf.com/Article/details/gsiouklmx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjejmvkmv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/glkbgtypc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqacvcrzf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/gvhjpxgjp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.epnwcf.com/Article/details/glpicaihb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gmlrstgba.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/gjbclwdfj.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gpzltmlcq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.yfazqb.com/Article/details/gazazhhwy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/gzguuxidt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/grxwtrylt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/giaiqssqa.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/glzutpcxi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/ggoujntur.sHtML

{**a, **b}
来源：http://m.share.vehdjk.com/Article/details/gntwlpimg.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/guzsjdxpo.sHtML

{v: k for k, v in d.items()}
来源：http://3g.bbcook.cn/Article/details/gevtuedkt.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gndlxrpaj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.sjlbkw.cn/Article/details/gjrvdfjng.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gcmarqgcy.sHtML

max(d, key=d.get)
来源：http://www.share.fktsv.cn/Article/details/gkbfsowcz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/glpbotbzq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.bbcook.cn/Article/details/gklvjlohd.sHtML

[U11] Py：生成器表达式
来源：http://www.share.yfazqb.com/Article/details/goemgrsqw.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gyezgxsbm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.yfazqb.com/Article/details/gtwukykuo.sHtML

Counter(arr).most_common(3)
来源：http://blog.yfazqb.com/Article/details/gkjlvebbw.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/gcfqksery.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/grrwzdoqn.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/gpfdddpql.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gahhdvavg.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/gdujdyzoc.sHtML

t = time.perf_counter()
来源：http://m.share.fktsv.cn/Article/details/gwiwznyir.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/gkrshezgr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gqgrvxlhy.sHtML

[U17] Py：初始化日志
来源：http://wap.epnwcf.com/Article/details/gvxhzexek.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.bbcook.cn/Article/details/gvhplzvhp.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gynbcnzdh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gdncxpjmj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/gnjaitrgt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.epnwcf.com/Article/details/gpexgtqma.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gainpmiwa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.tarul.cn/Article/details/gizzebavp.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gwtkgoilj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhukbbyg.sHtML

[U22] Py：矩阵转置
来源：http://baike.epnwcf.com/Article/details/gfyekztvm.sHtML

list(zip(*m))
来源：http://m.share.epnwcf.com/Article/details/ggqvozprp.sHtML

[U23] Py：分块读取大文件
来源：http://wap.yfazqb.com/Article/details/glfhooicm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.yfazqb.com/Article/details/gwtgbsvzs.sHtML

[U24] Py：路径操作
来源：http://mobile.sjlbkw.cn/Article/details/gvodntmgo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gizelekyn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gnlxbjpoj.sHtML

csv.DictReader(f)
来源：http://baike.yfazqb.com/Article/details/glojsvaiv.sHtML

[U26] Py：并发下载
来源：http://3g.vehdjk.com/Article/details/gzxcjgwxs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.vehdjk.com/Article/details/glsuzqvyz.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/gbbhbsrbj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.vehdjk.com/Article/details/ghsontdrg.sHtML

[U28] Py：类型别名
来源：http://baike.vehdjk.com/Article/details/gyjnjuxrq.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gkbwnimlp.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/guxfaxhfj.sHtML

@property 与 @x.setter 配合
来源：http://mobile.tarul.cn/Article/details/ghkmgonsr.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gwpjhceuj.sHtML

@dataclass(slots=True)
来源：http://www.share.fktsv.cn/Article/details/gyduuppmn.sHtML

[U31] Py：单测
来源：http://read.share.sjlbkw.cn/Article/details/gavpqwbqh.sHtML

python -m pytest -q
来源：http://www.share.bbcook.cn/Article/details/glzkkhowp.sHtML

[U32] Py：代码格式化
来源：http://baike.sjlbkw.cn/Article/details/gcoxyqrlb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/grtwfgzfo.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gzevcwipo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/gnufpytlr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gkrahjlho.sHtML

chardet.detect(raw)
来源：http://3g.bbcook.cn/Article/details/glnmffczd.sHtML

[U35] Py：发送邮件
来源：http://mobile.fktsv.cn/Article/details/gdyhyxjfe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.tarul.cn/Article/details/glxdtjppf.sHtML

[U36] Py：定时任务
来源：http://www.blog.vehdjk.com/Article/details/gxajmxzdv.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.yfazqb.com/Article/details/gxxifgyss.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/geiytekrs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/gwjyjyswq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.sjlbkw.cn/Article/details/gkvreoclf.sHtML

Path(__file__).resolve().parent
来源：http://wap.vehdjk.com/Article/details/gzzvxogtr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.vehdjk.com/Article/details/gorhacwyr.sHtML

sys.stdout.isatty()
来源：http://baike.vehdjk.com/Article/details/gthpqyoyn.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gqeyruhkx.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gerqliuld.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/gyapicymq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.vehdjk.com/Article/details/gyjicwxhp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fktsv.cn/Article/details/gdtloktyv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.sjlbkw.cn/Article/details/gabksbgdw.sHtML

[U43] PHP：声明命名空间
来源：http://3g.tarul.cn/Article/details/ggmcsdlye.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/glqcruegd.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.tarul.cn/Article/details/gqlvuulew.sHtML

declare(strict_types=1);
来源：http://www.blog.yfazqb.com/Article/details/guozoejfj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gyprqxcyv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gxmtlmgxj.sHtML

[U46] PHP：可空类型
来源：http://read.share.fktsv.cn/Article/details/gvbfbuwyg.sHtML

?string $name = null
来源：http://3g.bbcook.cn/Article/details/gcwqwjctp.sHtML


<!-- 参考信息 -->