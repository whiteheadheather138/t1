代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gjdwpzwgo.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/ghnjzgfoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/glhjuxrwf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gvxheuuux.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gaoccxipj.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gjsjmflvz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gfrzsfmfq.sHtML

[S24] C：获取本地时间
来源：http://mobile.sjlbkw.cn/Article/details/grpdnkapo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gkgpkqcri.sHtML

[S25] C：内存拷贝
来源：http://read.share.yfazqb.com/Article/details/gaixkobef.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/goassnvul.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/grfvfehbm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/gsetkgnnc.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gszqzdnfq.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/ghumplnrg.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gwfdsfrys.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/ghoyctgnn.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gyhndgfzg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/gbobezicd.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/glhssuylt.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/gvzdksurg.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gzmkizdyy.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gyonxihyb.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gzrobbycm.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gtvrdltch.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fktsv.cn/Article/details/gnrwifclv.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gjocwglbs.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gzikyqzti.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fktsv.cn/Article/details/guehwgvfq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/gjevrewjb.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/goryesnya.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.sjlbkw.cn/Article/details/gtqzqemec.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gmhzdwmtd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwttnfnkq.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gzmeqovyb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gmdgsdeea.sHtML

[S37] C++：set
来源：http://mobile.vehdjk.com/Article/details/gggakwldr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/ghwhgmrwu.sHtML

[S38] C++：排序
来源：http://read.share.tarul.cn/Article/details/ggcpgsvqr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.epnwcf.com/Article/details/gbtlsulfe.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gqgxqrbjd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/gzaiohfby.sHtML

[S40] C++：查找元素
来源：http://wap.tarul.cn/Article/details/gosjluxba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/ggavzmjuu.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gnrjnzrzi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gcbatylbv.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/gzpmxjcyl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.bbcook.cn/Article/details/gkshqcsly.sHtML

[S43] C++：智能指针
来源：http://3g.vehdjk.com/Article/details/gltuiyatk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gfwvimifg.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/ggpwnippg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gppqdxbkw.sHtML

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/gjruxljoa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.vehdjk.com/Article/details/gtvsgzpmv.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/gpwdxyweu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/ggfevkdba.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gbxbopafl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.sjlbkw.cn/Article/details/gmweqsdkb.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gfgjkstki.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gppuhkmsa.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gxsvwrvis.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gkgyrkhgv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gicjtvahz.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gymvgregl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gfzlavgrm.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gcykqzlxk.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/gdgeytyob.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/grnvndsrk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gezxdsock.sHtML

[S53] C++：移动语义
来源：http://www.m.share.bbcook.cn/Article/details/gjtqcyhel.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gqsygaxlt.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/gqylbelhp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gwmcljtrh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gbfydajou.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/glxcgbtjf.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gyedcomqb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/gvkkpjcts.sHtML

[S57] C++：编译期常量
来源：http://baike.tarul.cn/Article/details/gyuiqrdcu.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/grdpbbhru.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gqkycxwze.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/ggsanmkoj.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/gvmujqlbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gpwdutaii.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gkepwzufy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gukufrzdw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmqqydmnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gtddkkdpk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gifxucdke.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gtzzqtjsc.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/goicaduxo.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/gwavrzsuc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/gsiadjtlu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/ggogcezoy.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gfuwubidc.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/ggykgnfke.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gnnhpgeaj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gtznkxlwd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.sjlbkw.cn/Article/details/gwkzioerd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gfhlochax.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gbvayhglz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gjzehivac.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gcrhjjkwm.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gqolncjrs.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.bbcook.cn/Article/details/gxpjrlqef.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/gkqibgvla.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/ggbptxwun.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/guvsxfveq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/ghfqiqaar.sHtML

[T11] Kotlin：协程
来源：http://read.share.epnwcf.com/Article/details/ggdphdoxj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.bbcook.cn/Article/details/gdlxuyqhi.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/geljbmelh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gullabars.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gdwfwuzsd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/ghqxpuhlj.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/gdjxznqwu.sHtML

for (i in 1..10) println(i)
来源：http://baike.tarul.cn/Article/details/gbbcohdgz.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/gkcahpgfb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/glepygfyg.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gvytvzngi.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gogpsplrr.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gkvkcigoe.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/grajwstze.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gpgjcyrkn.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gfilbwzdo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/guauuojhz.sHtML

if let n = opt { print(n) }
来源：http://read.share.bbcook.cn/Article/details/gotksxcyg.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/gykduexml.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gvtkwdbci.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gamtxuxad.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gfvkldpab.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gljksvlxt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gtjkukaen.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gjcyuuyyl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/guxzhyflr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.yfazqb.com/Article/details/gwwrdjojl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.epnwcf.com/Article/details/gmohvwivr.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gwnfqvuik.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gutojvlys.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/gtieyurbl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/gvgehanfu.sHtML

[T27] Swift：错误处理
来源：http://blog.bbcook.cn/Article/details/gobvznxwr.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gmndfdusb.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/gmlnnekjj.sHtML

enum Color { case red, green }
来源：http://www.share.bbcook.cn/Article/details/gdynsmgag.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gxmlsnlen.sHtML

guard let x = opt else { return }
来源：http://blog.vehdjk.com/Article/details/gtaabkgrt.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gktvohxba.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gciadikmp.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gtphtbwgu.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gfjmahygt.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/gljfgmjlv.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/gnsuvyjmp.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/gjmprioxn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.vehdjk.com/Article/details/gssihqbku.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gdvyatvuo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gzzlvfnzz.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/glripwvnt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/gdzkmxvmn.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gsgyblvtu.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/gvhkdkujl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gamihnmrz.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gvimoaxgj.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/glygnfsuy.sHtML

if x > 0 then print("正") end
来源：http://baike.fktsv.cn/Article/details/glzqtrpsk.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/ggpfiqcsk.sHtML

string.find(s, "%d+")
来源：http://www.blog.vehdjk.com/Article/details/gceegmlwc.sHtML

[T40] Lua：元表
来源：http://www.blog.epnwcf.com/Article/details/gkjdmtmkn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/gdcxseiuf.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gwqvekkas.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/geulmbloi.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gdjwakcni.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/gmvynpess.sHtML

[T43] Perl：字符串插值
来源：http://blog.tarul.cn/Article/details/gbhroswpa.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/gnelwromd.sHtML

[T44] Perl：条件
来源：http://3g.fktsv.cn/Article/details/gxlowehqd.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/gakdnzdqf.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gklyrgrdj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.vehdjk.com/Article/details/ghyrxfanl.sHtML

[T46] Perl：哈希操作
来源：http://3g.vehdjk.com/Article/details/gofcwvxtg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gkihslqcv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/gsytdgzda.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.epnwcf.com/Article/details/ggoftafkc.sHtML

[T48] Perl：正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gfhbimpcn.sHtML

$s =~ s/old/new/g;
来源：http://blog.yfazqb.com/Article/details/gtiphhfwe.sHtML

[T49] Perl：函数
来源：http://baike.fktsv.cn/Article/details/gyainreso.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gddpipbrf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gsglsiwbo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gvtkwgymf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/glkuzrojb.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gwtwwbnib.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gmqndkzas.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gsjfhqyxu.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gvxtdkxyr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gjntuvqmd.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gzhnbyhhz.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gupsqrmae.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gcsukqafe.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gggajrorl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.vehdjk.com/Article/details/gmrctxykj.sHtML

[T56] Scala：样例类
来源：http://www.blog.tarul.cn/Article/details/gofyxuyih.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/glpnqknob.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gvszbjtzn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/gcmsvyiqu.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gregpjkdc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.bbcook.cn/Article/details/gbqdtdict.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gjecqrynx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gtsforxql.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/gpfuitbcv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gvbprvbnn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxpvskfxg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxlorkero.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtzciwumx.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.yfazqb.com/Article/details/gulxgggio.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.vehdjk.com/Article/details/godaxhpbb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gffxdstqb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gjbuwqljw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gkztmowwx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gidweboms.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.yfazqb.com/Article/details/gocadpxfr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/gkaoqadva.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/gcrjlptjo.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gyqvttzky.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gdmcamvxd.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/gmnumjesk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gqdbhvwar.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gzwppjqfm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gmkbkvlrl.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/gbsiwvqbz.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fktsv.cn/Article/details/ggqhlaqwu.sHtML

max(d, key=d.get)
来源：http://www.m.share.bbcook.cn/Article/details/goujygkwp.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gqpdanqlt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.bbcook.cn/Article/details/glkyeqabl.sHtML

[U11] Py：生成器表达式
来源：http://mobile.tarul.cn/Article/details/gthcecput.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gaudcfcex.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.sjlbkw.cn/Article/details/gsnimfniq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.vehdjk.com/Article/details/gcmxgfmam.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/gksshwdji.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gsawkziet.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/ghadbwgdm.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gjiaznzyh.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/ghdrnvueo.sHtML

t = time.perf_counter()
来源：http://mobile.fktsv.cn/Article/details/gvgdkqgpw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/gikzgazki.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gzmdwnchz.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/ggyttzuca.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/glpqhhnnr.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/guuaojekg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.vehdjk.com/Article/details/gxgxrqais.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gzmxlymyv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.yfazqb.com/Article/details/gdcegldbo.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gwkzompse.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.bbcook.cn/Article/details/gowavjcow.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gbmqryyxd.sHtML

@contextlib.contextmanager
来源：http://mobile.yfazqb.com/Article/details/gmoxxfovb.sHtML

[U22] Py：矩阵转置
来源：http://3g.vehdjk.com/Article/details/gaarkvkty.sHtML

list(zip(*m))
来源：http://read.share.fktsv.cn/Article/details/gijuvvegk.sHtML

[U23] Py：分块读取大文件
来源：http://wap.epnwcf.com/Article/details/gxmzgztio.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.tarul.cn/Article/details/gsmxuyiji.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/ghgeubnub.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gaotonpvz.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gqfycleak.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gzbpffhio.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/ghsxwklhy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/gneputgmd.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/gzglxyygr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.sjlbkw.cn/Article/details/gmuxctbcw.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/grifxgcng.sHtML

UserId = int
来源：http://mobile.epnwcf.com/Article/details/guqlzdhac.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/glaymqovs.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/grwdewtjs.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/gpyfaoxvn.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/gsqpoltje.sHtML

[U31] Py：单测
来源：http://mobile.epnwcf.com/Article/details/gqyvbizof.sHtML

python -m pytest -q
来源：http://wap.vehdjk.com/Article/details/gqwlwiudd.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gpoqlscaf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.epnwcf.com/Article/details/gmxsdfqjr.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/goyivrhlp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/gpirsazuq.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gyvbpqsms.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gjltfupmf.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/gkypxpxyi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.bbcook.cn/Article/details/ghzisyhiu.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gvdmtzozq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.vehdjk.com/Article/details/gjucctgye.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/gvzdnjhqg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gyvjktdgg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.sjlbkw.cn/Article/details/gnxrboggk.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gwqhymhgv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.sjlbkw.cn/Article/details/grgxxstyh.sHtML

sys.stdout.isatty()
来源：http://www.blog.tarul.cn/Article/details/gqwiemnfx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/gvyunswdp.sHtML

print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gaaedcjhq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.yfazqb.com/Article/details/gonvgeapj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.bbcook.cn/Article/details/gignlfpzc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/gbhazedjp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/gwaxumhec.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/gshvbodcj.sHtML

namespace App\Http;
来源：http://www.m.share.tarul.cn/Article/details/gyedhgizs.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gavxgbrdz.sHtML

declare(strict_types=1);
来源：http://wap.sjlbkw.cn/Article/details/gaevotzil.sHtML


<!-- 参考信息 -->