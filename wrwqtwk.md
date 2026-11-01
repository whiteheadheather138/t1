代发 wailian999

int main(int argc, char **argv)
来源：http://mobile.fktsv.cn/Article/details/gpnfyedfc.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gknheupbk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gvsmihqbp.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gfwnjwpro.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/ggsankhpy.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/ghkuuyqgx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.bbcook.cn/Article/details/gvgzolcqx.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gcgzdruyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/ghkzctavu.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gsnbyxeah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gpabresjy.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/grcpovofy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/ggqnygbsv.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/ghfpwbvml.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/goukelurv.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gsxmlhvgp.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/ghuuddmnn.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/ggrwqenmi.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gdppkkhev.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gtnqbwqzg.sHtML

static int counter = 0;
来源：http://mobile.vehdjk.com/Article/details/gxpyqyzsn.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gzmgoiyuo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.bbcook.cn/Article/details/gcsrrwuky.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gstokiwrf.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gnccjlysi.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gzaysaipr.sHtML

#endif
来源：http://baike.epnwcf.com/Article/details/gwzuwsaac.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/govdylqhh.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/grlkjvhbu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gmikqebrr.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/getsugnri.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gpturdbpz.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gzdyzbfvt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gefpjujvz.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/gctelgsgp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gmhemiidz.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gocxaiyto.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/goiodqmuy.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.epnwcf.com/Article/details/ggyrajakq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gwzdzxguv.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/ghkupdayh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/glnvcwsaw.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gzlqwgvsm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gartrgtdk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdimyqwd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/govgmlzhh.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/gutpqdorg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gkrmckmto.sHtML

[S41] C++：类与构造函数
来源：http://m.share.yfazqb.com/Article/details/gemdxvrzx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gzsubahau.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gdgzeefjp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/ggdzohlwj.sHtML

[S43] C++：智能指针
来源：http://m.share.yfazqb.com/Article/details/gqhbhhjfg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gkadpdqyo.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gjokaeicq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/gvufdfokj.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/ggcyyscmr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/grbgabjfb.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gqzirllot.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggyluhwbq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbjfzbwp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjasxuaug.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gbcoquhvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/geticgcny.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fktsv.cn/Article/details/gyncqpwnb.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gloibkfcd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gbdooukiw.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gsxvavbbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gixqaweis.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gwfqzddkk.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gnkldgjbl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fktsv.cn/Article/details/gdqjeyqef.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqduwdfyl.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/grthrqmaw.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gawkdqukd.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/glsnaxuif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.vehdjk.com/Article/details/gakvbeupa.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gngrvjgsj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gijcfwzsy.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gqdvamxui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gjmxmtcgk.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/grmqflsxw.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gvsqxnhby.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gzirqxajm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gfzrpqlbc.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gsfyoylkk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gdypmcysm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gepdcnejx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/ghfxrbizy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfytyoxzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/grsfkweac.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqwusvszc.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.yfazqb.com/Article/details/ggfzqukgi.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/glmmoadvr.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gdkyohons.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gpqbidqtq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/ghltiervl.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gcowqucxq.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gyeagpgck.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gaxmsfvxo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gcychfgpo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fktsv.cn/Article/details/gogncufdb.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/garemqrsj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gldorezbe.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gtrnzmeua.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gexmkwqha.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gcrlynbqh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gtyhybwau.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gnfmmxcjg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gicktxdyh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gvsasdhgi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gtxojtiol.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gewwzgfly.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/gjtvfgpwb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gaiwhumzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcggxpnsx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gkjzyajak.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/gdqcweuty.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gbhgstnwj.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gycmnaawu.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gujzbotmq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/grnjivxoh.sHtML

[T16] Swift：Hello World
来源：http://3g.tarul.cn/Article/details/guvcwlzsx.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gsafjtlfq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gylnwljjp.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gqpueftsi.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/ggaanzxts.sHtML

"值: \(b)"
来源：http://baike.bbcook.cn/Article/details/gprkllqec.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gxfjkpnqh.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gjdmdknyd.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/gacrowubu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.tarul.cn/Article/details/gybefnszt.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gqdqhjign.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/gnkurvlvw.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/gxaubgysx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gntqwmdnx.sHtML

[T23] Swift：函数
来源：http://www.blog.epnwcf.com/Article/details/gbdugyxzq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/gwoouyeev.sHtML

[T24] Swift：闭包
来源：http://blog.tarul.cn/Article/details/guunithsa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gcfqagfpk.sHtML

[T25] Swift：结构体
来源：http://3g.epnwcf.com/Article/details/gqmmibjmw.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/gdwtveljt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/glvhshtef.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/gqxcyoqfk.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gigkjncku.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/gpzcnwknp.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gssnawdxa.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gizxqcxtt.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/gnxkzcnwo.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gediojyzt.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/gznoxvlil.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.vehdjk.com/Article/details/gogqutgcx.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/galbazdgi.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/ggaygxgyk.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gpiednptp.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gwnfumsgn.sHtML

[T33] Lua：表（数组）
来源：http://www.share.sjlbkw.cn/Article/details/gcxoncmky.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.yfazqb.com/Article/details/gcymmlolw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gxlcurvlx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.bbcook.cn/Article/details/gkzpzyhzv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrznzykn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gofrgigcg.sHtML

[T36] Lua：函数
来源：http://blog.sjlbkw.cn/Article/details/genslacnz.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gzbaudncm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/gicxgshmx.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/gderdwpkg.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gpbrmwcya.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/gbjafygda.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gkugujjhi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/goombhxrt.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/guwfihxxk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.epnwcf.com/Article/details/gmfbsddua.sHtML

[T41] Perl：Hello World
来源：http://blog.vehdjk.com/Article/details/gszzzarhk.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/gitouqwsj.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/gmklwdwqw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.sjlbkw.cn/Article/details/gvwrpkyrl.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/glapgshrg.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/geuifsibo.sHtML

[T44] Perl：条件
来源：http://3g.bbcook.cn/Article/details/ghnbcityo.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.sjlbkw.cn/Article/details/gnqpwowwi.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gtyttshxt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gitxrzjio.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/grtkwvfmc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gyvcxqiqb.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gkhhommac.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/gepqnpiba.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/guyabnhte.sHtML

$s =~ s/old/new/g;
来源：http://read.share.epnwcf.com/Article/details/gaxkrmqxt.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/goktcnret.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gplsbkuvz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gyhailrhp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gmeemtrjb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gfqfrenpb.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/gatpovvyt.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gtccpsnpi.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/glmpvdsnl.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/ghlfrliab.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gwgiztumg.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/grkcdcskv.sHtML

[T54] Scala：集合映射
来源：http://3g.yfazqb.com/Article/details/gyqcjkefj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gspriaijd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/ghabatzdu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gwocybukj.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/glagoowkh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gimrqsawr.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gnvdvaaij.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/grllgfjjk.sHtML

[T58] Scala：函数定义
来源：http://mobile.tarul.cn/Article/details/gsjrccrwn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/goznerzta.sHtML

[T59] Scala：循环
来源：http://read.share.epnwcf.com/Article/details/gmrnrfqtr.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/gylwschqh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gxurqgggm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/gajqkldfs.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdwcsrcfb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/glhdjhfwh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzaakryrb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gvuxzgoop.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.tarul.cn/Article/details/gbsrshpea.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.tarul.cn/Article/details/ggvmsymcu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/gbnlstwiw.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gbbgafvev.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/gieqatjms.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gbkqdsqwk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fktsv.cn/Article/details/gtuxzkgxr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.sjlbkw.cn/Article/details/gyutfqwru.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gooyecnqp.sHtML

[U06] Py：合并两个字典
来源：http://blog.fktsv.cn/Article/details/gwjfenlhk.sHtML

{**a, **b}
来源：http://read.share.yfazqb.com/Article/details/gblbckaur.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/gowvnxhij.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/guyoqkzdv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.bbcook.cn/Article/details/gogkggseg.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/grrhqookj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.tarul.cn/Article/details/gebfbjwli.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gvvejdjtk.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/ghtleliwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.yfazqb.com/Article/details/gbuzbanzy.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/gscctdjmp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/glpoyukbm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/ghqqeqczo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gehmurcbj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/gcmakehcp.sHtML

deque(maxlen=10)
来源：http://www.blog.vehdjk.com/Article/details/gbjrmgkeo.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gdlzfxtii.sHtML

defaultdict(list)
来源：http://mobile.vehdjk.com/Article/details/gsubvdqzx.sHtML

[U15] Py：高精度计时
来源：http://mobile.vehdjk.com/Article/details/gqmbpqlsk.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/ghnngcczu.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gwkukbima.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.vehdjk.com/Article/details/gdeeeczbx.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/ggegxvcbf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.sjlbkw.cn/Article/details/gizhbxgfs.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.epnwcf.com/Article/details/gacepgnoz.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/gxqgxkrtu.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gqjbsztge.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/gzjyplgcz.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.bbcook.cn/Article/details/gvmdzplug.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gvsgpnsuk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gdmbilrqy.sHtML

@contextlib.contextmanager
来源：http://www.m.share.bbcook.cn/Article/details/gfieptmcd.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/goeicslvm.sHtML

list(zip(*m))
来源：http://baike.yfazqb.com/Article/details/gdkzhmjfr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/goofcsjza.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.epnwcf.com/Article/details/glpmcmgvi.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gdnmzpfpg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gmnusqchg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/gwulzolct.sHtML

csv.DictReader(f)
来源：http://wap.epnwcf.com/Article/details/gkxesoijj.sHtML

[U26] Py：并发下载
来源：http://www.share.epnwcf.com/Article/details/gymokhhtz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/gqgasjrot.sHtML

[U27] Py：异步 HTTP
来源：http://baike.tarul.cn/Article/details/gdydsbqhu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.yfazqb.com/Article/details/gkzcpvkbo.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gehksoflk.sHtML

UserId = int
来源：http://mobile.fktsv.cn/Article/details/gukcpdgyl.sHtML

[U29] Py：属性校验
来源：http://m.share.vehdjk.com/Article/details/gsnthqrer.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/gxiluzttv.sHtML

[U30] Py：数据类
来源：http://www.blog.bbcook.cn/Article/details/gsklcxivd.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gkmrzuhmp.sHtML

[U31] Py：单测
来源：http://m.share.bbcook.cn/Article/details/gsyhygted.sHtML

python -m pytest -q
来源：http://www.blog.yfazqb.com/Article/details/ggaschftz.sHtML

[U32] Py：代码格式化
来源：http://m.share.vehdjk.com/Article/details/gxvowvmgd.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.tarul.cn/Article/details/gaqskvwrz.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/gcfakeyrk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.sjlbkw.cn/Article/details/gautsusci.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gdigghtry.sHtML

chardet.detect(raw)
来源：http://baike.tarul.cn/Article/details/gtoboborp.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/gdblffesp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gvqpcfogp.sHtML

[U36] Py：定时任务
来源：http://wap.fktsv.cn/Article/details/gtopzglol.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.vehdjk.com/Article/details/gmieszqgq.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gmonhteyr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.vehdjk.com/Article/details/gtxwaejde.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gsuiopfkg.sHtML

Path(__file__).resolve().parent
来源：http://3g.tarul.cn/Article/details/gmxmetkph.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/gcfbzomfx.sHtML

sys.stdout.isatty()
来源：http://www.blog.sjlbkw.cn/Article/details/ggqxhfgww.sHtML

[U40] Py：打印到标准错误
来源：http://blog.vehdjk.com/Article/details/gkmrpjkeh.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gqkwataxf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/gmhepnghn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/gqmvxkukv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gppigkcag.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.bbcook.cn/Article/details/guyccdfqp.sHtML


<!-- 参考信息 -->