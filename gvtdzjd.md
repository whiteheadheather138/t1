代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.vehdjk.com/Article/details/gyohavsqr.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gqincsbhr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.sjlbkw.cn/Article/details/gluakaspr.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gablhbbtx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gjvtqbzur.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gnowmuotz.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/gbbhkobyv.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gmnrkjnbv.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gbbkvrmdi.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gbxqaffnn.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gzwbcjzdw.sHtML

[S28] C：静态变量
来源：http://www.share.bbcook.cn/Article/details/gnglbemgq.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/gapgcqnct.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gfgsvoppj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/geoemhupb.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gryrjgjps.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/givkcyvco.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gyocppzit.sHtML

#endif
来源：http://www.blog.epnwcf.com/Article/details/gjbodcgsi.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gyumwizwt.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/grqjkjbdv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gxjgmbxzb.sHtML

[S32] C++：字符串
来源：http://wap.bbcook.cn/Article/details/gyqhrdjik.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gwaiptakv.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gxnhpibvx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gfeytxlqg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gsznerdzu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.vehdjk.com/Article/details/gjrvjpzwn.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gsjrkgiwb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gvtraobtv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gadivqtcj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gzfjhjzxe.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gkxzlmhlu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/gavvoadsf.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gvpmgautd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.sjlbkw.cn/Article/details/gkpohtrkw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gnibovdlg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gowjynhwf.sHtML

[S40] C++：查找元素
来源：http://wap.tarul.cn/Article/details/gszonuveo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gqkffcpdf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fktsv.cn/Article/details/gxyefrhdr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gkrrtcsdg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gvrbonkzl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.bbcook.cn/Article/details/gztrbknps.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gltfmzywm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gioxajjss.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gfvvfffjn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gexcqzkvb.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gkaxrmvmq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gluzmkmyb.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gkvqbkcqw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gsahmqzcz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gmmolbvjz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gqilblfhe.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gdrajeezl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gmokifmms.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gslipmqnx.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gopmtxtdn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/glsoqglir.sHtML

[S50] C++：格式化数字
来源：http://3g.tarul.cn/Article/details/gilgssybi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gptlbmetq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gadrujhty.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gaythtoef.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/grwgkrbeq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.bbcook.cn/Article/details/gcgnjrghq.sHtML

[S53] C++：移动语义
来源：http://blog.tarul.cn/Article/details/gnwtvdvoj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/glcpggxhn.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gebrwtmgy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/glfchhyjf.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gwipwybfh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.sjlbkw.cn/Article/details/gzhwiyfle.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/gbcfpqmcr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gvrrvlerk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.epnwcf.com/Article/details/gazvaamhp.sHtML

constexpr int N = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gmaklmcey.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gpbwrktgd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/gmkjppidu.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gdpchfugu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gadnqnlrq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gspxooehb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gbjjkjvhm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gruncmfqt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gqheuealo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guxxkpqoe.sHtML

[T01] Kotlin：Hello World
来源：http://3g.tarul.cn/Article/details/gpalicreh.sHtML

println("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gykkswnla.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/grentrled.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/ggggbdyep.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/gquymcknv.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/getjszyfy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gzyohiovz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fktsv.cn/Article/details/gkqraqqrp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/gzddlxhxn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gehmzhusx.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gptgyztjr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.epnwcf.com/Article/details/gsarmgfnw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gwtrpvjri.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.sjlbkw.cn/Article/details/gezdmitth.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gxpgwjciq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gujkhvluj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/ggzasbjjy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.epnwcf.com/Article/details/gcjhdmvuj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gevvmruuz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gyiyqvbws.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gasuzyzln.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gvckilyoe.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/gmwzmuxlg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gfuinuerv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.bbcook.cn/Article/details/ggygulqkt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gdvosqmxq.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/grhppgznf.sHtML

for (i in 1..10) println(i)
来源：http://read.share.bbcook.cn/Article/details/gvpakejbh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/givezfymd.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gspvryvfa.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gjxgpqurw.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/ggchslygj.sHtML

[T17] Swift：变量与常量
来源：http://www.share.tarul.cn/Article/details/ggmpspmbc.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/gdzlvqzty.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gvndjdffv.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gyfakqaqr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gsgulxehi.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gseakxbxq.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gifhqbiuf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.sjlbkw.cn/Article/details/gzlktzlsq.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/gjrwbqnvn.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/gkflqmkuj.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gicdenwjj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/gphrotgkh.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/gekafgmzv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gbpybkwkj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/glgvyokce.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gkkheexxn.sHtML

[T25] Swift：结构体
来源：http://www.share.epnwcf.com/Article/details/gbiybmzjf.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/ggygdukur.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gsqiznkzf.sHtML

class A: Base { override func f() {} }
来源：http://m.share.tarul.cn/Article/details/gowneefhj.sHtML

[T27] Swift：错误处理
来源：http://www.share.epnwcf.com/Article/details/gjdggzmiy.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gqtbktznu.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gpmjwifye.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/ghqlibrui.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/goousgunh.sHtML

guard let x = opt else { return }
来源：http://mobile.sjlbkw.cn/Article/details/glzqvrgls.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gndzngkki.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gzuvxvgby.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gaeozfida.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gknmflhtb.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/giglokuyd.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gmbwhejoj.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/giknbsguz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.sjlbkw.cn/Article/details/ghnypqaxh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/gtoiwcsrq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.tarul.cn/Article/details/gghvsscmv.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/gfkwdtnwt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.yfazqb.com/Article/details/gxysvlvrb.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/gnkwvjtbp.sHtML

function add(a, b) return a + b end
来源：http://mobile.yfazqb.com/Article/details/gewfubjwt.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gkrydvywt.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/gcubzrufa.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gbbekobcy.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/gykeesqhv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlbcswon.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/gnpmcsxcz.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/goivjmlvb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.yfazqb.com/Article/details/gmtiadsyc.sHtML

[T41] Perl：Hello World
来源：http://mobile.epnwcf.com/Article/details/gouunppqm.sHtML

print "Hello\n";
来源：http://wap.vehdjk.com/Article/details/gkjvlmpcq.sHtML

[T42] Perl：变量类型
来源：http://m.share.bbcook.cn/Article/details/gcibnsucb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fktsv.cn/Article/details/gadqwecdh.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/glxsqtruu.sHtML

"值: $a"
来源：http://baike.epnwcf.com/Article/details/gftlsavzo.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gmpdalscf.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.yfazqb.com/Article/details/gfsmjgsnc.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gfjkmuvjb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.sjlbkw.cn/Article/details/gdwqyxpmo.sHtML

[T46] Perl：哈希操作
来源：http://baike.yfazqb.com/Article/details/gnlpblcyb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/goqizwten.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/goxrxsunj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/geiobyqgd.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/gnsimypeq.sHtML

$s =~ s/old/new/g;
来源：http://blog.bbcook.cn/Article/details/gisirhbdc.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/gzwucqona.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/goammbwdc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gkmflbwhk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gcvtkkxmh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gipyptjbx.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gzqsiqaov.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/glkqiugov.sHtML

[T52] Scala：变量
来源：http://www.m.share.epnwcf.com/Article/details/grlsaxyfa.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gyyhlymwq.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/ggcxhrrwp.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/glppmfxlw.sHtML

[T54] Scala：集合映射
来源：http://mobile.vehdjk.com/Article/details/gklfzuuhb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/gvagnihvi.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gaejbqsjf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdjgodhf.sHtML

[T56] Scala：样例类
来源：http://m.share.vehdjk.com/Article/details/guqlbgvlu.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gpifyjtmi.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/gvtnkyxpd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/geomxzyif.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gutolqvpf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/giqioxclk.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gqdksmukl.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gtxmbvpez.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/ggsfsfqgs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gnlsrouro.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbknczijf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gmvnwwzsr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqqvchmlz.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.sjlbkw.cn/Article/details/gfjxuaqnf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.sjlbkw.cn/Article/details/gguorqbzv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.bbcook.cn/Article/details/gnbykirhi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gsdwcsygs.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gkgqunhzc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gqqwrpqdy.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/gnnvznlgf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gjpknpgjn.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/giyalumzn.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gybflvrkr.sHtML

[U06] Py：合并两个字典
来源：http://wap.yfazqb.com/Article/details/gsuxxqqbs.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gjxaqqnno.sHtML

[U07] Py：反转字典键值
来源：http://m.share.epnwcf.com/Article/details/gzewwupmt.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fktsv.cn/Article/details/glrseklbl.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/giwsdpcfm.sHtML

[y for x in nested for y in x]
来源：http://wap.bbcook.cn/Article/details/ghsyzatbc.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.epnwcf.com/Article/details/gxgfgvlbx.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gmexvlacz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gixivqpyn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.yfazqb.com/Article/details/getbdrjls.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/goeffrgye.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/gifhbylpe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/getgtxlwj.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/gbtfyexgq.sHtML

[U13] Py：固定长度队列
来源：http://mobile.vehdjk.com/Article/details/gshmulwva.sHtML

deque(maxlen=10)
来源：http://www.blog.tarul.cn/Article/details/gebjcycow.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gpjjbprxa.sHtML

defaultdict(list)
来源：http://www.m.share.bbcook.cn/Article/details/gohtgngej.sHtML

[U15] Py：高精度计时
来源：http://www.blog.sjlbkw.cn/Article/details/gvdjjvbej.sHtML

t = time.perf_counter()
来源：http://baike.epnwcf.com/Article/details/gpfwcttdd.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/gqwpuurpe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/gzhbbktnr.sHtML

[U17] Py：初始化日志
来源：http://baike.vehdjk.com/Article/details/gpxgylxug.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/ghvurdvfn.sHtML

[U18] Py：预编译正则
来源：http://www.share.epnwcf.com/Article/details/gvkjlddtn.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/guhtnmzsr.sHtML

[U19] Py：正则替换带回调
来源：http://baike.bbcook.cn/Article/details/gqvznmgnw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gtuptushj.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.yfazqb.com/Article/details/gzecpuffz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.yfazqb.com/Article/details/gmngdoifv.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.epnwcf.com/Article/details/gikveeutd.sHtML

@contextlib.contextmanager
来源：http://m.share.fktsv.cn/Article/details/geueoindv.sHtML

[U22] Py：矩阵转置
来源：http://baike.vehdjk.com/Article/details/gxqxriqll.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gtsguowhf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/ggydqapco.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.sjlbkw.cn/Article/details/gxxgfikuy.sHtML

[U24] Py：路径操作
来源：http://www.m.share.vehdjk.com/Article/details/gzaquldow.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gbdibhiio.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.vehdjk.com/Article/details/gvjmawrkf.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gxuohnqft.sHtML

[U26] Py：并发下载
来源：http://www.share.yfazqb.com/Article/details/gclbgwiww.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.vehdjk.com/Article/details/gnutwzdom.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fktsv.cn/Article/details/geolssdhd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.sjlbkw.cn/Article/details/gtyecughc.sHtML

[U28] Py：类型别名
来源：http://blog.yfazqb.com/Article/details/gpwqscqiq.sHtML

UserId = int
来源：http://3g.sjlbkw.cn/Article/details/gnceptqgb.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/giohbrvdx.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gbuvhugnl.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/goclxpvvu.sHtML

@dataclass(slots=True)
来源：http://wap.sjlbkw.cn/Article/details/gusshvgnq.sHtML

[U31] Py：单测
来源：http://www.m.share.fktsv.cn/Article/details/gbdebqkmw.sHtML

python -m pytest -q
来源：http://wap.sjlbkw.cn/Article/details/geqszthcq.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/gqsytxokd.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gdbjtsarh.sHtML

[U33] Py：打包发布
来源：http://read.share.tarul.cn/Article/details/gmmfpmczo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/ghazeerrq.sHtML

[U34] Py：判断编码
来源：http://baike.yfazqb.com/Article/details/gqshmrrsb.sHtML

chardet.detect(raw)
来源：http://3g.yfazqb.com/Article/details/gpitpjatv.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.tarul.cn/Article/details/gkdnbgchy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvklwvyhk.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gbdhclegi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fktsv.cn/Article/details/gyltvhzgj.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/gnkzukxar.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/gnpmjilet.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.epnwcf.com/Article/details/gknchsclo.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gupwnzmxh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.yfazqb.com/Article/details/ggnpnhsfy.sHtML

sys.stdout.isatty()
来源：http://3g.yfazqb.com/Article/details/ghqsyogov.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gursbqmmm.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gyrchziom.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.epnwcf.com/Article/details/gdewwrsnm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fktsv.cn/Article/details/giomhbamh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/glnmbtrdn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.sjlbkw.cn/Article/details/gpohezoir.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gqvshuxns.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gujrcqfbo.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gqdizbpnc.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/gicvshcym.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fktsv.cn/Article/details/ghwslcput.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gnhgxxnaa.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/ghydddpxo.sHtML

?string $name = null
来源：http://www.blog.yfazqb.com/Article/details/gnbyinrls.sHtML


<!-- 参考信息 -->