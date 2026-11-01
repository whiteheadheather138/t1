代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/ggxbslcbz.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gtqfaltsj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gzhdwvxrb.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gxvnqfing.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gkdzrtrvo.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/ggdaevago.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gqxifuwoi.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gbrojlllh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/getpjuikl.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gyrzwmnzb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqwsiwwx.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuezeeqf.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gpwagxrwy.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gwsmxfwsb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gwvkevryd.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/ghsyvxomo.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gefolumpo.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gqipvrjgo.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gtsmzixuk.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/guzmvykxi.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/ghrrddboc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gnplrvyvt.sHtML

[S32] C++：字符串
来源：http://3g.sjlbkw.cn/Article/details/gbzpewevc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.vehdjk.com/Article/details/gzoqibzqh.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/grbikrxla.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gjdpoiivq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.tarul.cn/Article/details/ghcdvpxiv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gulnilzri.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gkuizhnlm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gehnmcrgd.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gmsohrbro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gauerpsof.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/ghfiyoltm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/gdtfndvuy.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gawbjfzxw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gasoetaim.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gllahpbgc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gezbmiulr.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/grfrunqhw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gqopnmdmz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/grtotxwtn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gsidwlsrd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/ghuqwfkpb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/ghbgtrnet.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gmgajudiz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/ggpnyheqb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/gvgpdcdna.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gqyxvadzj.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gvvxrxsmf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.tarul.cn/Article/details/govnqewlu.sHtML

[S46] C++：函数模板
来源：http://3g.yfazqb.com/Article/details/gvolfkzvm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gywurwswd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/ghxigyary.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gpakeflop.sHtML

[S48] C++：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gkqfagfdr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/guuylndmw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/gywpqoneq.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gubvzkcqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gcvsmvjdy.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/glqnwlifw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyztsaol.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gdiggjbnb.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gmylgkups.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gboiakzka.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gevovgpvf.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/goezxrrxm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/gojrqmgzm.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/glozzxdoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gvwxnwlll.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gnvqszxio.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gmtfaezun.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gmrpxbimb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.epnwcf.com/Article/details/gjgfikiwc.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gpmdodbon.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gzvnvchhf.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gzyjwmcpa.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gtnidbkps.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gwljjipfc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gdtwuylmr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.sjlbkw.cn/Article/details/gjozluksg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gopsjgtnn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnxfjenky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gzrtvzlzz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjffuqclo.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gxyewpcsn.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gfmlzslgx.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gnneggfnw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.epnwcf.com/Article/details/gylittnjh.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.sjlbkw.cn/Article/details/gwdzlitvh.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/grqlwzuem.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gwhfyhrqq.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/guocbbiqf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/ghwnaybxo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/gbzrvmcmz.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gyxeansib.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gxdgahoqt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gqobowfzp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/ghlklvgwp.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gvihuyeyj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/gokospgkn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.tarul.cn/Article/details/gbqsgoxho.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/gsgzfcidq.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gbikzxnod.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/ghzrfmooh.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/gyqlyozvz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fktsv.cn/Article/details/gbcaggxca.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fktsv.cn/Article/details/guszdgtnk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gcbenvydq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gvbzyfikk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gvuakxdee.sHtML

[T14] Kotlin：循环
来源：http://mobile.fktsv.cn/Article/details/gmglaemoz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gelfksrvx.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/ghucfmmsv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gfadyehtn.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gycrlkdav.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gtcyzvrke.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gdtktsnqs.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/gulkqxhqs.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gfjwjvthk.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/gsobwcwpk.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gtxpithea.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/gvrrvjxkc.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/gvusrbgog.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/ghbhvqbht.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/gzmjnbybz.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gelkasskd.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gsvaqvorb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gufbcmvxi.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gtthxxraa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/guugdjigw.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/gvtslnmtn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gppmqbnlr.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gkhddyspx.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gvmrswpqo.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gdopkoieb.sHtML

class A: Base { override func f() {} }
来源：http://wap.tarul.cn/Article/details/gqkmeszva.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gobggtxpw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/gdoxbljad.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/getnyxjhn.sHtML

enum Color { case red, green }
来源：http://3g.sjlbkw.cn/Article/details/gmgkknjwv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gubgsuorj.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/girmvjhhc.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gnjldapwu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gocwlvkvp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gidjrfqyx.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/geoupxbir.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/gbgwkukif.sHtML

local a = 1
来源：http://blog.tarul.cn/Article/details/grkoorgjs.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gldjelnmj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/gyhkkwhmw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/ggbeicfpd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.epnwcf.com/Article/details/gphcpdaqb.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/ggghqwfzs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/grsxhonxt.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/gvotzuham.sHtML

function add(a, b) return a + b end
来源：http://mobile.bbcook.cn/Article/details/gwbdhzwia.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gahetmotr.sHtML

"a" .. "b"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjpbmukg.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/ghrlnmfia.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gbewiqwzc.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gtedvjdwe.sHtML

string.find(s, "%d+")
来源：http://read.share.bbcook.cn/Article/details/gpslhcohe.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gkngfiapg.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gibumkxxo.sHtML

[T41] Perl：Hello World
来源：http://read.share.bbcook.cn/Article/details/gpzwatjwj.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/gqqyfobev.sHtML

[T42] Perl：变量类型
来源：http://m.share.bbcook.cn/Article/details/gsfpfxabm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/glhndtiig.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/goyserqzl.sHtML

"值: $a"
来源：http://wap.fktsv.cn/Article/details/gnnielnzx.sHtML

[T44] Perl：条件
来源：http://m.share.sjlbkw.cn/Article/details/gltgvafwx.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.yfazqb.com/Article/details/gojxxmnoy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gjskioqnv.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.bbcook.cn/Article/details/gshmcenes.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fktsv.cn/Article/details/gyffihnxt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.yfazqb.com/Article/details/gkulsnnai.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gtetdcsqf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fktsv.cn/Article/details/gupmpqxwh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.epnwcf.com/Article/details/gglfhbmth.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gfejrpiuf.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gixzapfie.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gfspqfsas.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gknklzlsv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/govuxfbie.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gpwxsvaat.sHtML

[T51] Scala：Hello World
来源：http://baike.tarul.cn/Article/details/gwkupokuo.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gxoxcqpey.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gjcofmxkb.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/glirtcpzp.sHtML

[T53] Scala：字符串插值
来源：http://3g.tarul.cn/Article/details/gsfjlgjfz.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/glgoslbgz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gjfwfrgsq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/grnlqfniv.sHtML

[T55] Scala：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gnvaejyoq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/ghozfcyit.sHtML

[T56] Scala：样例类
来源：http://www.m.share.tarul.cn/Article/details/ghgubzaox.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gvzvbajpc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gsdaxmgeo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gtyoedokd.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gsskqfvjq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fktsv.cn/Article/details/gzkjcnxbv.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gkgjnvyex.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.yfazqb.com/Article/details/gavspfifa.sHtML

[T60] Scala：折叠
来源：http://baike.fktsv.cn/Article/details/giopxyxhe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gphpnspog.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqljvmukn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gtrwrnmll.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmhyvkxfj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/goaefqvpl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/gmahkoodc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.sjlbkw.cn/Article/details/gzekovett.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fktsv.cn/Article/details/gttxcxolb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gbtsbmyxh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.bbcook.cn/Article/details/gtxdhnuth.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gzazuiagk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gswlnvzhb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gwlofktoz.sHtML

list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gueixhdbs.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fktsv.cn/Article/details/gyegstvwo.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gdywspjdj.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gzpqnkyol.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fktsv.cn/Article/details/gelzykmmb.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gmwsrxdfx.sHtML

[y for x in nested for y in x]
来源：http://3g.fktsv.cn/Article/details/gvcxeexea.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.vehdjk.com/Article/details/glybkhdmm.sHtML

max(d, key=d.get)
来源：http://blog.tarul.cn/Article/details/gkkbjvgnc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/gycayesiq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.yfazqb.com/Article/details/guudrfwug.sHtML

[U11] Py：生成器表达式
来源：http://wap.vehdjk.com/Article/details/gdyfhccda.sHtML

(x * 2 for x in arr)
来源：http://blog.sjlbkw.cn/Article/details/groksatcn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.epnwcf.com/Article/details/gpwgjvpyj.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gvhxxgxzu.sHtML

[U13] Py：固定长度队列
来源：http://baike.sjlbkw.cn/Article/details/gwojboqts.sHtML

deque(maxlen=10)
来源：http://3g.vehdjk.com/Article/details/ghovdfjmd.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/gtseykfza.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/grpiyxqzz.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/grrnygjhc.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gykwlpowa.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.tarul.cn/Article/details/glqcwdtfs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.vehdjk.com/Article/details/gccsekoiy.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/ghgjauzhd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmheldsq.sHtML

[U18] Py：预编译正则
来源：http://m.share.fktsv.cn/Article/details/gradodhxm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/gzpvhmdci.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.yfazqb.com/Article/details/gwasppjhs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/ggdhcudbx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.bbcook.cn/Article/details/gszhdidwk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gznrjaebc.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.epnwcf.com/Article/details/gjliobepk.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gbbpljxvu.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.bbcook.cn/Article/details/gbsulczkd.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/giaytjkdk.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gubexftyj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.yfazqb.com/Article/details/gbmivyvtq.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/gtcbzkqal.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gkosltqks.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gktgwjblu.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/ghmechrby.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/gvwuqkmmy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.sjlbkw.cn/Article/details/ggxhpuxtb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.yfazqb.com/Article/details/gmuwqvldc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fktsv.cn/Article/details/gpznuixyb.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/gotiqhmvj.sHtML

UserId = int
来源：http://www.share.sjlbkw.cn/Article/details/gfmqswwjx.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gatxdrvqt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gtdnxmniu.sHtML

[U30] Py：数据类
来源：http://read.share.yfazqb.com/Article/details/gqysdendj.sHtML

@dataclass(slots=True)
来源：http://read.share.epnwcf.com/Article/details/ghemfnnex.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gyzygddpx.sHtML

python -m pytest -q
来源：http://blog.tarul.cn/Article/details/golcvaiga.sHtML

[U32] Py：代码格式化
来源：http://m.share.fktsv.cn/Article/details/gihiavgsl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/gndtysrwh.sHtML

[U33] Py：打包发布
来源：http://blog.sjlbkw.cn/Article/details/gozjbdntt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fktsv.cn/Article/details/gcmvujkcq.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gdrpkoqbe.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gupwbiowp.sHtML

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/gdvnoabzf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/ggmvfwkfa.sHtML

[U36] Py：定时任务
来源：http://m.share.vehdjk.com/Article/details/gpcotiior.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fktsv.cn/Article/details/gvrkxrlks.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gofkwzvmv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/gpkgjrdsm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/guvdkpgqj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.tarul.cn/Article/details/gkvmihpcl.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/gcruxgrud.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/gsmuwpuee.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/gffdraglx.sHtML

print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gfnhrhccv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.tarul.cn/Article/details/gzstfsnmv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.yfazqb.com/Article/details/gmfiheute.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.vehdjk.com/Article/details/gjfucaacd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.bbcook.cn/Article/details/guefyvgzf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.yfazqb.com/Article/details/gouvqokvf.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/ghiyufgcp.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/goumrptqy.sHtML

declare(strict_types=1);
来源：http://3g.tarul.cn/Article/details/gdvrdsrxw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/gabseuuhv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gerqlidsm.sHtML

[U46] PHP：可空类型
来源：http://blog.bbcook.cn/Article/details/gnuxmvsdb.sHtML

?string $name = null
来源：http://3g.yfazqb.com/Article/details/glpydqqzq.sHtML


<!-- 参考信息 -->