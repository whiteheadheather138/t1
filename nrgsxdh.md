代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gfiouccer.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/gyzpyaudb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gwqesubhw.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gnrfajveo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/gunnojgrm.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gxvavaoqg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.vehdjk.com/Article/details/gjjfddoyr.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gslcdzsyn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gcfngdueo.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gjimwgoci.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/glgozleje.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gwdkupiih.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gzbzmruwt.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gpmygtztd.sHtML

const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gumztchqr.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gtmpgsqdl.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gmuargdht.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gkeqvdldh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gwcawbzsk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gbyrtwrbe.sHtML

#ifndef X_H
来源：http://www.share.sjlbkw.cn/Article/details/geobvabkr.sHtML

#define X_H
来源：http://www.share.vehdjk.com/Article/details/gzzlorddz.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gauyoohjn.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/grkfitxst.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gbbknlurl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gvaqppnau.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/glchsjnmu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gawmjwshj.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/gevmlqebf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/gelfwjgfr.sHtML

[S34] C++：遍历 vector
来源：http://blog.bbcook.cn/Article/details/gbfwvvuhp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/gqxojqoyi.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gxaqbzvev.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gefwnavxs.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gncwfiujv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gdjnkhthp.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/gxlbwqeod.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gjthzlalk.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/gnqszatun.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.vehdjk.com/Article/details/gfysksugl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gcearjhch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/gcrygrtfq.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/gtgvrtrjz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/ggdptgbfs.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/giqmtgrhx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.vehdjk.com/Article/details/gusmmcaqr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gcuhtaocd.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gjvrhbipw.sHtML

[S43] C++：智能指针
来源：http://read.share.vehdjk.com/Article/details/gsctnqion.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/glnwwjlcl.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gycvqjxza.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/gprlkzilr.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gqnynpcqu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gltzbvmqq.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gxiyuqxjw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gttpfgupf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gsmggmeni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.tarul.cn/Article/details/gzfznhrnl.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gdaxifsma.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/gmxbewfbu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gkwxxidsy.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gzceaexqv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gnlhooyqf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.epnwcf.com/Article/details/gsgwhtwyx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gzphpdkhm.sHtML

[S51] C++：显式类型转换
来源：http://blog.vehdjk.com/Article/details/gojsgumno.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gwjamsgjn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gqakoxhvi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.vehdjk.com/Article/details/gfbitbpaz.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gfrrvomng.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/gvhhqdnjt.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gklsryprz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gnnsxhduo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.vehdjk.com/Article/details/gchmxtkji.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/gaisruuor.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/gioedflhv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gharrbkah.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gdyuozoju.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gfdhxrpig.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gcoflrnpl.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fktsv.cn/Article/details/gfzigyecr.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gabulrwxj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gyndofdje.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gkzucfapb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/giqthgucp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpyxgzsky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gecmqugrc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gndkgeonr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gzvuglkbw.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gsygxgyip.sHtML

[T02] Kotlin：变量
来源：http://www.blog.yfazqb.com/Article/details/gqdvwobdn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gbhvipmmr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gurkxpmdi.sHtML

"值: $b"
来源：http://baike.vehdjk.com/Article/details/gpgeboykw.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/gpxwgqfft.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.vehdjk.com/Article/details/gdexhjyjw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/gkmudulmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fktsv.cn/Article/details/gslsrusfp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gpixggprk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.yfazqb.com/Article/details/gybaofdqo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/gibdnotgr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gdarpjzxe.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/gpxfydcgg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/ggrytkpuo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/ggxywlxmx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gwykaupma.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gbhapiuop.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.yfazqb.com/Article/details/ggmdrutga.sHtML

[T11] Kotlin：协程
来源：http://www.blog.epnwcf.com/Article/details/gkjlwzjaj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gnodxaorc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gkascrovx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gfbzzlstw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gypupmjrh.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/guwnqkhwe.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/gbyxyrman.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/grmfkwkud.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/gdzdtqliz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gdgtvigjh.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/ggolacfqa.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gjnnuqags.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjgvogcw.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gablcltgy.sHtML

[T18] Swift：字符串插值
来源：http://mobile.epnwcf.com/Article/details/guljfpxuo.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gxerwojpx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gkbcjiquk.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gknbejqmk.sHtML

[T20] Swift：数组操作
来源：http://wap.vehdjk.com/Article/details/gkwuqlrxa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/giaqebwcc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.vehdjk.com/Article/details/gaxpkchjx.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/guwppcbyq.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/grhvgzhix.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gasihzfyx.sHtML

[T23] Swift：函数
来源：http://mobile.sjlbkw.cn/Article/details/gqwjetpmj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gqfeimhhl.sHtML

[T24] Swift：闭包
来源：http://www.blog.yfazqb.com/Article/details/grkkcyiwd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gdodknerw.sHtML

[T25] Swift：结构体
来源：http://m.share.fktsv.cn/Article/details/gjdgkkwtw.sHtML

struct P { var x: Int }
来源：http://baike.sjlbkw.cn/Article/details/gqwxdsvzr.sHtML

[T26] Swift：类与重写
来源：http://wap.epnwcf.com/Article/details/glsfnyuxv.sHtML

class A: Base { override func f() {} }
来源：http://baike.yfazqb.com/Article/details/giexbzwqi.sHtML

[T27] Swift：错误处理
来源：http://mobile.yfazqb.com/Article/details/gpkkqmeyx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gtyjuykrl.sHtML

[T28] Swift：枚举
来源：http://blog.fktsv.cn/Article/details/gnddudpxh.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gboahkvyq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.epnwcf.com/Article/details/glkzqjnpd.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gqnomkvcd.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gcytdcpkb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/gkygvkjdx.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gefcbagfy.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gbmbyabew.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gwdwgnqnr.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gjxgtgzwt.sHtML

[T33] Lua：表（数组）
来源：http://blog.yfazqb.com/Article/details/gnnitjjqy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.yfazqb.com/Article/details/genloyvuk.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/ggrleyqqq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.bbcook.cn/Article/details/gofwynomd.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/ghztvdjka.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/glnyixfym.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/giifubhmn.sHtML

function add(a, b) return a + b end
来源：http://read.share.tarul.cn/Article/details/gygzxbwya.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gsrbjelih.sHtML

"a" .. "b"
来源：http://read.share.yfazqb.com/Article/details/giexnsxnp.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gceiyxabs.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gfstaahng.sHtML

[T39] Lua：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gswxbsgio.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gkoqtbakp.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gpyuthbwb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.bbcook.cn/Article/details/gvathfmnj.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/gmzmntmpi.sHtML

print "Hello\n";
来源：http://m.share.vehdjk.com/Article/details/gdjugcurj.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gazsxraqp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.epnwcf.com/Article/details/gjtsfztdn.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gihaogrct.sHtML

"值: $a"
来源：http://baike.epnwcf.com/Article/details/gydwkiyyl.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gsduzshde.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gozfculxr.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gnmijykxo.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.bbcook.cn/Article/details/gajcegoll.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gwjhxwmyk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gkoribvsf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/ggfsogguy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.vehdjk.com/Article/details/gzjlgmmro.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/gnzdkmtfz.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gyuuptcfu.sHtML

[T49] Perl：函数
来源：http://wap.yfazqb.com/Article/details/gckmniusb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gyydckcos.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gtupfarhh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gnxghdbvb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/gtbjcwbke.sHtML

[T51] Scala：Hello World
来源：http://www.share.fktsv.cn/Article/details/gbwnrbqji.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/glnkyqeog.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gbvzyxuhw.sHtML

val a = 1;  var b = 2
来源：http://m.share.vehdjk.com/Article/details/gmerqrvzn.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gppwbqzws.sHtML

s"值: $b"
来源：http://baike.vehdjk.com/Article/details/ggqwciigu.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gebkfcamc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gtczztcxf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/gqasogzfp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gxghveblp.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/gnwjrqdgo.sHtML

case class User(name: String, age: Int)
来源：http://3g.fktsv.cn/Article/details/gubhhewqe.sHtML

[T57] Scala：模式匹配
来源：http://wap.bbcook.cn/Article/details/gmqaxtmva.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/ghmagphrf.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gaijfmdrq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.bbcook.cn/Article/details/gyrwsoisq.sHtML

[T59] Scala：循环
来源：http://blog.epnwcf.com/Article/details/gtevhezwq.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/ggdyksmna.sHtML

[T60] Scala：折叠
来源：http://blog.vehdjk.com/Article/details/galbavlly.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gfbhidxcn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glhlkdcqj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/gtdfhfdno.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxgryvtun.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.tarul.cn/Article/details/gevfwkqrp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/guggznlqq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gdmdgejus.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.tarul.cn/Article/details/gebyccoyw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/glzqnxxno.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gyrkihbuv.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/guqxlqung.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gffppwhgt.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.yfazqb.com/Article/details/gxmixrbue.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gokbyaunt.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fktsv.cn/Article/details/gwyhrxwmz.sHtML

{**a, **b}
来源：http://www.share.sjlbkw.cn/Article/details/gbwnwmcrx.sHtML

[U07] Py：反转字典键值
来源：http://blog.bbcook.cn/Article/details/giqrrpooo.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/gsynhgbij.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gumjlccyw.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/ghywfynsp.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/gtiytoejh.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gtstwyeng.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/ggyxuyrpd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.tarul.cn/Article/details/gossmvakw.sHtML

[U11] Py：生成器表达式
来源：http://blog.vehdjk.com/Article/details/gsxhtonxm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gygubtomq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.tarul.cn/Article/details/gznowokgg.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gmpuvriue.sHtML

[U13] Py：固定长度队列
来源：http://www.share.vehdjk.com/Article/details/gonqyjbqv.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/guthktpyx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/giuirzzul.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/gxhocsmbu.sHtML

[U15] Py：高精度计时
来源：http://wap.epnwcf.com/Article/details/glcnovcvx.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gdmlholex.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fktsv.cn/Article/details/gmuzxcsde.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.bbcook.cn/Article/details/gfxafiqor.sHtML

[U17] Py：初始化日志
来源：http://blog.bbcook.cn/Article/details/gprsuacxi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.epnwcf.com/Article/details/guloxsawv.sHtML

[U18] Py：预编译正则
来源：http://read.share.epnwcf.com/Article/details/gdkyjdxxe.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.epnwcf.com/Article/details/ggzxveylj.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.yfazqb.com/Article/details/gjjwrefdr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/gpzkqrpoj.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.epnwcf.com/Article/details/gcfcpamat.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/grixshftn.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gdibqhjtu.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gfeurrhvp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/gfdgufvlc.sHtML

list(zip(*m))
来源：http://mobile.epnwcf.com/Article/details/gqwlmqzpi.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/glozrzfij.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/ghfvohcmm.sHtML

[U24] Py：路径操作
来源：http://baike.tarul.cn/Article/details/guwgnzrjg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gftpwkqya.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.epnwcf.com/Article/details/gigwwbkaz.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/gcxnxmczj.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/gqjqjnhtc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.epnwcf.com/Article/details/gmiyjlgok.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/gahymqoks.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gjzvruuih.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/gtpszihub.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gikqkyxur.sHtML

[U29] Py：属性校验
来源：http://wap.yfazqb.com/Article/details/gijkerzkz.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gynpkvfcv.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gytqvvjyt.sHtML

@dataclass(slots=True)
来源：http://www.m.share.epnwcf.com/Article/details/gtfblbdbs.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/girkmzbop.sHtML

python -m pytest -q
来源：http://wap.bbcook.cn/Article/details/ghdqvirod.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gddhekbjz.sHtML

ruff format . && ruff check --fix .
来源：http://baike.sjlbkw.cn/Article/details/gtsxrkaql.sHtML

[U33] Py：打包发布
来源：http://wap.yfazqb.com/Article/details/gwmdyrffp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.vehdjk.com/Article/details/gzqfwinmt.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/gfntphnwb.sHtML

chardet.detect(raw)
来源：http://www.m.share.yfazqb.com/Article/details/ganhhrzxu.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/gususlzyd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.sjlbkw.cn/Article/details/gychlkfco.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/gehqbbvyy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.tarul.cn/Article/details/glyhpeakb.sHtML

[U37] Py：读写 Excel
来源：http://blog.bbcook.cn/Article/details/gpgfxxfjc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/givyidqmb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.epnwcf.com/Article/details/gbzzhzppz.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gwfnixizb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.bbcook.cn/Article/details/ghqebhdar.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gxbfdbwky.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.tarul.cn/Article/details/gbxinmejb.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gbzmaqigb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.tarul.cn/Article/details/gocwqsrbb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gkdtjjxmg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.sjlbkw.cn/Article/details/gtpheseqp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.sjlbkw.cn/Article/details/gxsxhxiiq.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gievktwpy.sHtML

namespace App\Http;
来源：http://wap.epnwcf.com/Article/details/gesxxthnb.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/gcpubdykx.sHtML

declare(strict_types=1);
来源：http://mobile.fktsv.cn/Article/details/gzhywpklx.sHtML


<!-- 参考信息 -->