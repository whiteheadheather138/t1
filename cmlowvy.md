代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/gkiwsygon.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gxftznqpn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gjxncuqgn.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gikdtxzgg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/guzlzjoid.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/gajeyaauy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gilszhede.sHtML

[S24] C：获取本地时间
来源：http://read.share.yfazqb.com/Article/details/gdsvurnky.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gzuwxqseg.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gqemcqska.sHtML

memcpy(dst, src, n);
来源：http://blog.tarul.cn/Article/details/gyilujzea.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gyhvdiedd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gfzxkchwb.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gwmsulaxu.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gjyxksmla.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gwlbtdith.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gbgdonkay.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gelwhpdan.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gnpibbcmv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gzxrlveib.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gejjnceob.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gazwwtxhw.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/giaynafpf.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gecrltvyz.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gpcjkgcaq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gfnjavsti.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/grbdadlhi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.sjlbkw.cn/Article/details/gxqgzjzkc.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/ggqondyhw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gvtmdfjtl.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gwcsoanqr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/grxtgiibx.sHtML

[S35] C++：map
来源：http://read.share.bbcook.cn/Article/details/gvwtnewyw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gnwyepsky.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gryudjscy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gecmnnhwf.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gbfgwbibn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.vehdjk.com/Article/details/gxuuhwaec.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/gwvrkuisu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gnqyemdmj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gtvvqnpnu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/gucnrcoec.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/geeyzrqbq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/gbrhhlqez.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gqtraewfx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gdtyqbtsf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fktsv.cn/Article/details/gkchmzkwy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gadsqgngl.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/gvtyfujuy.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gzehmgltb.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gqfidtmrn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/ghmlomhfy.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gxfzxxkxb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gppvovznq.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gyabgyorq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/glplyyocy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.tarul.cn/Article/details/gmtmiqhgm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gutjoyyvi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gyplihisv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gktsfirho.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/glsmjgweu.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gyuwjfqfh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gecyakzyz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gipouzlqg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gmdcrsvah.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gstyemlps.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.epnwcf.com/Article/details/gfwtloqpg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/gqkhwsnuz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/gwsovmdeg.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzyyynxt.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gwmmqlsmk.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gkahpneid.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/gwaumwwhr.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gkrvzaysn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.yfazqb.com/Article/details/gccygzcke.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/gvgkfsfng.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gpnxrpbok.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gwizcrvge.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/guetpmfrz.sHtML

[S58] C++：命名空间
来源：http://baike.sjlbkw.cn/Article/details/gbgnyxabu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gcptbxtax.sHtML

[S59] C++：静态断言
来源：http://mobile.tarul.cn/Article/details/gxqjiahtd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gebxnzcwo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/ggnphvonc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gmgedbjfu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxtikkziz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/grlwfdsyf.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbsvbrqgz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gpwtsgeir.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gjmdnqvjj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.epnwcf.com/Article/details/gfizeeldz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gvlxfwwuz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/gmbpdtilx.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/guxgoaqxv.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gobxvkhch.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gqooqglom.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gdktislrp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gjuxxsnzo.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjltegdo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gjydiksfb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gfhaxmvpe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gswpzkbzz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gcmonivzl.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/ggmqyjveo.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gmzpqiysf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.tarul.cn/Article/details/gomjigohv.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gykssrrbl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gpcgtxlwt.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gwzqrmwwq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gtlqxyroa.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/gigjpkkas.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/gdxwfohrh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/ggujeaqtb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/ghnodafsk.sHtML

[T14] Kotlin：循环
来源：http://wap.epnwcf.com/Article/details/gaxquppjt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/grfxwebei.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/grapjhktv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.sjlbkw.cn/Article/details/gujsceimd.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gtejyapmp.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gquyvwxxq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gqidfncrc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvnkkzsb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gezqpmfnb.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gxcybwthl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gmdgnexoz.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/gnhfohiom.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gqbpkleyf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/gmtthabsv.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gtjjsosbs.sHtML

for x in a { print(x) }
来源：http://read.share.epnwcf.com/Article/details/gxbawuuhu.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gquvmojkm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gursllvox.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gqlheonpr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/gycgppbec.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/giwitzear.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/goiipdxry.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/gpjjlotfn.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gxheglgal.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.vehdjk.com/Article/details/gcxivzcvk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/ggjmajmen.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gzychjaoc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gikoburyb.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gdjfaonfn.sHtML

enum Color { case red, green }
来源：http://blog.tarul.cn/Article/details/gnogzaggb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gwlrhqytu.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gmbsrnngr.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/ghxxiijaw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gduxcwgiv.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gcucxffnw.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/ghwepjooi.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gspvcoziv.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/gthofsunr.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gpxsvvxci.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/gtbmzfwft.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/glkwoaexi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/ghenkegpe.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/ggldiudnj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.tarul.cn/Article/details/glgmykskg.sHtML

[T36] Lua：函数
来源：http://read.share.bbcook.cn/Article/details/ginpkjruz.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gqaienvbe.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/grqytwzos.sHtML

"a" .. "b"
来源：http://blog.bbcook.cn/Article/details/ghhfgcjkc.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/gtygtyzzd.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/gfzhvjfof.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gplkghszh.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/gpvbysxwm.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/ggezbouva.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gxozgkzgj.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gdpbgvugu.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/gztaslbft.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gfimzqccx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gwykqeumf.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gionyijsi.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gcdoimokd.sHtML

[T44] Perl：条件
来源：http://www.share.yfazqb.com/Article/details/gmcgbekfj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gsrgwcfzw.sHtML

[T45] Perl：数组遍历
来源：http://baike.vehdjk.com/Article/details/gkctfcrcn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.yfazqb.com/Article/details/gxzbigjzw.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gcawavkji.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gyyxdaqtc.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/gktjnjdgx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.vehdjk.com/Article/details/gkudphonz.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/gbfgcxogs.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gmlfiftlh.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gazvsynhj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/ggjjsawmr.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gozgrdikw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gleiibqsm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.vehdjk.com/Article/details/gpkdelnbb.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/galzpahxo.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gnorbznve.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gvkfdrdez.sHtML

val a = 1;  var b = 2
来源：http://wap.epnwcf.com/Article/details/goitsmyqs.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gpbxliycr.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gbbnytitn.sHtML

[T54] Scala：集合映射
来源：http://www.share.bbcook.cn/Article/details/glirnvfey.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/gkfxwdgzb.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gdfgjenpm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwxhvrtrp.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/guccauhmu.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gyeccbhpp.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/gjnmtfyfb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gntlzthmu.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gcluizynk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gbmukrxkf.sHtML

[T59] Scala：循环
来源：http://m.share.fktsv.cn/Article/details/gfjsdkkdf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gwvabzsal.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/goyedfyfj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.epnwcf.com/Article/details/gqzrjhzma.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjgdethdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/ghsscmyqv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmjwpuipx.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fktsv.cn/Article/details/gsaitzfws.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gkmblvynz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gppibjrgq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gmlxgbsup.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.tarul.cn/Article/details/ghjihnppc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/grtrmfuzj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fktsv.cn/Article/details/gvaaknvdp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/gxvxdwifi.sHtML

[U05] Py：列表去重且保序
来源：http://3g.sjlbkw.cn/Article/details/gkjdiiziz.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gdqnpnhrw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fktsv.cn/Article/details/gyhetfogf.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/ggcojpwau.sHtML

[U07] Py：反转字典键值
来源：http://read.share.bbcook.cn/Article/details/gevbzpbfi.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gxddrdxqa.sHtML

[U08] Py：展平二维列表
来源：http://www.share.bbcook.cn/Article/details/gmrzqsupf.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gdbmgqzme.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/glaginmkz.sHtML

max(d, key=d.get)
来源：http://3g.vehdjk.com/Article/details/gebyhppjc.sHtML

[U10] Py：按值排序字典
来源：http://baike.bbcook.cn/Article/details/gvefswokh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fktsv.cn/Article/details/gnsblfyre.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/gbiacdcvz.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gqitciyrl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/ghgiwggwg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.tarul.cn/Article/details/grjnkadda.sHtML

[U13] Py：固定长度队列
来源：http://wap.epnwcf.com/Article/details/gvypmhfrj.sHtML

deque(maxlen=10)
来源：http://3g.sjlbkw.cn/Article/details/gpowxiscv.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.epnwcf.com/Article/details/grwrvhcur.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gkcysgjzn.sHtML

[U15] Py：高精度计时
来源：http://wap.fktsv.cn/Article/details/ghuqfryeu.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gwvdajzkq.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.epnwcf.com/Article/details/gicoyncng.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gsqisbqwd.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gotwohhjy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/gkezflqzk.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/ggxvoqtzc.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/gmkfxjkry.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.bbcook.cn/Article/details/gzbtanybx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gtzspjpgw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.tarul.cn/Article/details/gdiqderdq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.bbcook.cn/Article/details/gniadufjx.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gjojmsbno.sHtML

@contextlib.contextmanager
来源：http://www.share.yfazqb.com/Article/details/gicywzcsc.sHtML

[U22] Py：矩阵转置
来源：http://read.share.vehdjk.com/Article/details/gzzziogko.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/gstyxosms.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gbnjvjfyd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.epnwcf.com/Article/details/gloewptdx.sHtML

[U24] Py：路径操作
来源：http://m.share.bbcook.cn/Article/details/gzrhkcgky.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/guorodsue.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gjhbsszip.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/ggkjbuwez.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/gmwdfkpkp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/geguvhgeq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.vehdjk.com/Article/details/ghlrrdefb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.tarul.cn/Article/details/ghxequxnr.sHtML

[U28] Py：类型别名
来源：http://read.share.sjlbkw.cn/Article/details/geymsuvab.sHtML

UserId = int
来源：http://blog.vehdjk.com/Article/details/giottcbkk.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gkfsagdky.sHtML

@property 与 @x.setter 配合
来源：http://m.share.sjlbkw.cn/Article/details/gtehlbkdu.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/guawmyjwd.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gmvrgmuoi.sHtML

[U31] Py：单测
来源：http://www.share.fktsv.cn/Article/details/ghvsxwwre.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/gapovzzub.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.vehdjk.com/Article/details/gibvkidil.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.epnwcf.com/Article/details/gdyowwdws.sHtML

[U33] Py：打包发布
来源：http://3g.yfazqb.com/Article/details/gdphctsaq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.vehdjk.com/Article/details/gopfmayig.sHtML

[U34] Py：判断编码
来源：http://www.share.epnwcf.com/Article/details/gibmgqkoa.sHtML

chardet.detect(raw)
来源：http://www.blog.vehdjk.com/Article/details/gfcxmbasj.sHtML

[U35] Py：发送邮件
来源：http://m.share.yfazqb.com/Article/details/gauvirwbk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.vehdjk.com/Article/details/gjpwdxkck.sHtML

[U36] Py：定时任务
来源：http://blog.sjlbkw.cn/Article/details/gyilwawyb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/gazpuougf.sHtML

[U37] Py：读写 Excel
来源：http://baike.bbcook.cn/Article/details/gnqqvsgya.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fktsv.cn/Article/details/gnwbdzbob.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.bbcook.cn/Article/details/grkrvppse.sHtML

Path(__file__).resolve().parent
来源：http://www.share.sjlbkw.cn/Article/details/gbhuakrjy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/gzmvesxhh.sHtML

sys.stdout.isatty()
来源：http://www.blog.tarul.cn/Article/details/gcuoxzpzf.sHtML

[U40] Py：打印到标准错误
来源：http://baike.sjlbkw.cn/Article/details/gcjmdjpuq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gcrrgrhkw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fktsv.cn/Article/details/ghtfwczgq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gxwojgeyr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gecpbpeuk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fktsv.cn/Article/details/geumaeqdy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/gsrcuilmu.sHtML

namespace App\Http;
来源：http://blog.sjlbkw.cn/Article/details/gurumulsy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gxdyemdbg.sHtML

declare(strict_types=1);
来源：http://mobile.vehdjk.com/Article/details/gagioleaj.sHtML


<!-- 参考信息 -->