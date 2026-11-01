代发 wailian999

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/gyhormdtu.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/gzsecsbyh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/ghlqzplmv.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gidwtaffk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/galbfmmmk.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gcewnlizp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gboqnkfjc.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gntrskqow.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.yfazqb.com/Article/details/gkspedqpr.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gqgtcvrty.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gscgykkba.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gttmjpciq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.vehdjk.com/Article/details/gihkgdzfi.sHtML

[S25] C：内存拷贝
来源：http://baike.bbcook.cn/Article/details/gkgkwtemm.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gmbuhtfmk.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gbdfilnaf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.epnwcf.com/Article/details/gzwoeicte.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gcwjbglwi.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/grlkbcypg.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gcynzepas.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/grdrmcacr.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gfyocubhk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/ghgjkwtco.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gewafzhgx.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gqysmlnuk.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gixojrgrw.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/ggktktgoe.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gyhfxhwsm.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/ginjdrnvz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.bbcook.cn/Article/details/gijqkfeee.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gtvuvkgnk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/glkdxrfjl.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/ggvcshivm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/gwqwsaioo.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gmjuknykk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.vehdjk.com/Article/details/gyqazlszx.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gytzudhok.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/ghqabnckt.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/ggsesrtnm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/glnxbcdux.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gsiuxjfsf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/glqfdyudo.sHtML

[S38] C++：排序
来源：http://wap.yfazqb.com/Article/details/galmnmvyg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/grqundypj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gimpzizrr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gaxppuyxo.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gxhrtgpvd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.sjlbkw.cn/Article/details/gvnyuujli.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gketzepha.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.sjlbkw.cn/Article/details/gzrbeivdd.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/gyiyxnnal.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gcvivewqe.sHtML

[S43] C++：智能指针
来源：http://www.blog.tarul.cn/Article/details/ghyyujvys.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gnrmmejov.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gwfeblpmd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gmmrxiefn.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/gpilrnshm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gzexihljs.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gufcmkqcp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gjvhrnhaj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fktsv.cn/Article/details/gwotyxmif.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghpbfmeli.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/garooxexh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gotefpzlx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gdpvhjrrf.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gvmhthcdc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gpdvjwdpr.sHtML

[S50] C++：格式化数字
来源：http://3g.vehdjk.com/Article/details/goztddjzc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/glcofkkdw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gmauudhiy.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gqiafpgud.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gasjpgvbf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/goxyficqu.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gxnlqkjqk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/ggatanmjl.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gbkgwuhxp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gvkqwawst.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/garrjlvad.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.yfazqb.com/Article/details/glpilfaek.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/ggwctrxtk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gdqlzgcxe.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gsxboumqi.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gzrlvyeqj.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gzdtmwqyy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gpgliiebs.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/gegxtmruc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gtmvjirvv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gqplziune.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gvrzbxmli.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsbpztdqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/geadcbgvs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/garveturg.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gtnsecpxe.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gefclhpmv.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/givyjejni.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gbkiawokr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gagzegkob.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/ggbpxpxkc.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gpyrqffif.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/guyfbdvux.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gxxrkvxum.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gwfcoimke.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/gmseaauhg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.bbcook.cn/Article/details/gvyqqrexj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gfuosduhh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/gmakrmmpk.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gqetjuqrl.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gcoccshes.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gugnqdews.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/gditmfosn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/grrieihdq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gnlqhlxbx.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gheoracbt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gnqdrayzr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/guxskyauq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gpuiuajxj.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/ggbcomocy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/garapiybx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gkcnfijng.sHtML

for (i in 1..10) println(i)
来源：http://baike.fktsv.cn/Article/details/ghwgotrby.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gvmktezho.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/grvcxterb.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gmsgshnno.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gomjezkvd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gnddlqxgk.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/gbgufczuu.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gsxzlfcxo.sHtML

"值: \(b)"
来源：http://www.m.share.vehdjk.com/Article/details/gwfiltybd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.tarul.cn/Article/details/gjwekepyl.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/gqearotkq.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdmwsvzl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.vehdjk.com/Article/details/gesgokkbw.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gokdhgzgs.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gpnasskzn.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/gjvykaxcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gwjunwwcn.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gprdbryob.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gjgiysjbk.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/gdexsclzl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.epnwcf.com/Article/details/ggjcpfqjy.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gjaqxynww.sHtML

struct P { var x: Int }
来源：http://www.blog.sjlbkw.cn/Article/details/grcumljnm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gwjypdacq.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gttncjkbx.sHtML

[T27] Swift：错误处理
来源：http://baike.tarul.cn/Article/details/gzgqoxndq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/gcstcvxqb.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/guqqdcltw.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gkmgxohha.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.sjlbkw.cn/Article/details/gdwpvzckl.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gpqatbhpg.sHtML

[T30] Swift：协议
来源：http://read.share.bbcook.cn/Article/details/gyztqcibx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gzgrpodiv.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gjaflcgdj.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/ggfuhllwx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.tarul.cn/Article/details/gtwmmzzhh.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gwnvvrixy.sHtML

[T33] Lua：表（数组）
来源：http://read.share.sjlbkw.cn/Article/details/gbjubfybe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/graoettsm.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gyhuqjxte.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/gtycsejea.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/gtdvavrhq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gmqkmftpu.sHtML

[T36] Lua：函数
来源：http://3g.tarul.cn/Article/details/gmxuynpyr.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/gziumcord.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/grheatcfv.sHtML

"a" .. "b"
来源：http://www.blog.sjlbkw.cn/Article/details/gxnqrugni.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/groozotcr.sHtML

if x > 0 then print("正") end
来源：http://3g.tarul.cn/Article/details/gwkpoihhp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gadyxflmu.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/gwimkedwp.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gkmevxjot.sHtML

setmetatable({}, { __index = base })
来源：http://baike.epnwcf.com/Article/details/gckodumzl.sHtML

[T41] Perl：Hello World
来源：http://blog.yfazqb.com/Article/details/gyclgnrvd.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gvjuujllv.sHtML

[T42] Perl：变量类型
来源：http://m.share.epnwcf.com/Article/details/gldksonyc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/grywomkdk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/glclkfcuw.sHtML

"值: $a"
来源：http://blog.epnwcf.com/Article/details/gojlwmadg.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/ghgfpgglq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/gunrngsba.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gxatwvqfs.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.vehdjk.com/Article/details/gczzwafwp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.tarul.cn/Article/details/gpaszejkz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfjbzpwkj.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/gicxuhsnl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/gdecuumbv.sHtML

[T48] Perl：正则替换
来源：http://read.share.tarul.cn/Article/details/gzruyaqiq.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/glyhgvsjb.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/gocgnabtf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gbdsdkdpc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gwqtqdgiz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/gckpgqmyz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fktsv.cn/Article/details/giyxxxfos.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gshgzatdq.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/gayudmzvm.sHtML

[T52] Scala：变量
来源：http://read.share.bbcook.cn/Article/details/gelrhiouj.sHtML

val a = 1;  var b = 2
来源：http://mobile.vehdjk.com/Article/details/gsozqovkz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gohbtchit.sHtML

s"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gffpljfvg.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gulrlkuuh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/gfmcngbbx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/glbppukjg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gfzodltyr.sHtML

[T56] Scala：样例类
来源：http://m.share.yfazqb.com/Article/details/gptzqhxsk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/gvtddwopl.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gpwerzhuu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gakoiessk.sHtML

[T58] Scala：函数定义
来源：http://blog.vehdjk.com/Article/details/gfoqksclb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/grczcsvhf.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gpbiqrdzk.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.bbcook.cn/Article/details/grxductdv.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gpraxyzyj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/ggpawsazn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gojwculef.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/govbvwwmg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/grswxstpt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/gzpdcfdki.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.bbcook.cn/Article/details/ghaispeub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gvlgjkjkr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.sjlbkw.cn/Article/details/gkqghnjsb.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gtrfbaldj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/gwohrmmkq.sHtML

[U04] Py：变量调试打印
来源：http://wap.epnwcf.com/Article/details/gyzvtgjmo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fktsv.cn/Article/details/gbxuostzh.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/givxinrwq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gcduhaivy.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gtxrtmuvy.sHtML

{**a, **b}
来源：http://3g.bbcook.cn/Article/details/gzyskdlil.sHtML

[U07] Py：反转字典键值
来源：http://mobile.sjlbkw.cn/Article/details/gqancbclt.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.epnwcf.com/Article/details/grlydijht.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gboqefetz.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gkdmcimnj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.yfazqb.com/Article/details/guqwuchlv.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/gecvsejpu.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/gwrxyjvbi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/gbuisioaf.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/gnrpbsxfl.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/gdqnkihqu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gndeixiod.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gfgwairls.sHtML

[U13] Py：固定长度队列
来源：http://3g.vehdjk.com/Article/details/ggqcysvij.sHtML

deque(maxlen=10)
来源：http://www.share.vehdjk.com/Article/details/gdelgibrf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gfcgpjvzl.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/grjuqnfbc.sHtML

[U15] Py：高精度计时
来源：http://blog.bbcook.cn/Article/details/gsopsymav.sHtML

t = time.perf_counter()
来源：http://blog.yfazqb.com/Article/details/gievlefhi.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gunzxiiou.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.vehdjk.com/Article/details/gkneuyxzy.sHtML

[U17] Py：初始化日志
来源：http://www.share.sjlbkw.cn/Article/details/gobyfasft.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fktsv.cn/Article/details/gindizluh.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/gxaoradkv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gtnybrngr.sHtML

[U19] Py：正则替换带回调
来源：http://wap.yfazqb.com/Article/details/gcumgeqku.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gwqmbugag.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/guycbgpih.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gftocygol.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gsqawxeph.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gxzorssit.sHtML

[U22] Py：矩阵转置
来源：http://m.share.sjlbkw.cn/Article/details/gvwytutms.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/gvgwwcylo.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fktsv.cn/Article/details/gewdzznpf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.yfazqb.com/Article/details/gidrpepnq.sHtML

[U24] Py：路径操作
来源：http://www.blog.tarul.cn/Article/details/glqoythrz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gbermplnc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.tarul.cn/Article/details/ghgzkttjo.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gjvbpuqvh.sHtML

[U26] Py：并发下载
来源：http://3g.sjlbkw.cn/Article/details/guoplqqfs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fktsv.cn/Article/details/glfyybhsi.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fktsv.cn/Article/details/gjtqacncl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.sjlbkw.cn/Article/details/geqvaccyo.sHtML

[U28] Py：类型别名
来源：http://m.share.tarul.cn/Article/details/glapjdhmn.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/glahbbnpc.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gcamrhoeh.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/gkisagcmx.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/guhrlejoa.sHtML

@dataclass(slots=True)
来源：http://baike.bbcook.cn/Article/details/gidkfcbka.sHtML

[U31] Py：单测
来源：http://3g.sjlbkw.cn/Article/details/gjrzrgpqk.sHtML

python -m pytest -q
来源：http://mobile.fktsv.cn/Article/details/gkvyriwlp.sHtML

[U32] Py：代码格式化
来源：http://mobile.epnwcf.com/Article/details/gshelizqh.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/gvnhtjwze.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/geuzmuyik.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/gnwlgnhhc.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gzshoxmut.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/gwsnjesya.sHtML

[U35] Py：发送邮件
来源：http://www.share.yfazqb.com/Article/details/gggvvfquf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gldfixosc.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gnlgcetbu.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.tarul.cn/Article/details/ghzddhjmb.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/gtdyiloii.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.vehdjk.com/Article/details/gdzfnhwts.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/glatewcwt.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.vehdjk.com/Article/details/gprztkqjh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fktsv.cn/Article/details/gdnxtioej.sHtML

sys.stdout.isatty()
来源：http://wap.vehdjk.com/Article/details/gaqecmjki.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gucknopkd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/givouylfb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.yfazqb.com/Article/details/gvpjpviqz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gojkodxxx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gmjdpdpun.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.vehdjk.com/Article/details/gftqsftjf.sHtML


<!-- 参考信息 -->