代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gxufwkbqh.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gjntiajaz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.epnwcf.com/Article/details/gdpdshczy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gdksbgqlp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gfuewohud.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gprdyvbfl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/geozoubez.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/gjpbpqvrm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/goqyrtvos.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gafczaztx.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gagyzuwln.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/gqbbgqodt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gxojgibdb.sHtML

[S27] C：定义常量
来源：http://www.share.sjlbkw.cn/Article/details/gghshinvz.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gljoslkqs.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/gxwdqrsbw.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gkjnzakfo.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/grbqfgvuw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.tarul.cn/Article/details/gcjiwblli.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gcuzlxbkm.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/gaytljlyp.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/ghuonwafk.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gocryceyr.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/glaamgejm.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gzqcnszpi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gqcrgnngj.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/gnpoeqlhg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gmogrpsjf.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gktqobbhg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/ghlxwbtmf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gqvmyxcot.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/giwkihzdj.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gqcvpdoyj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gviuwxyib.sHtML

[S36] C++：unordered_map
来源：http://3g.sjlbkw.cn/Article/details/gxletggwp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gmdazffyg.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gqkklubwi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/gkqizhqmb.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gwcsfzhxk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gdzhnypgz.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gevtytzzh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gdpbdfafu.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gxkqdxeor.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.yfazqb.com/Article/details/gfrwqhzqr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gfttszbxd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gxbgvedzr.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gowhgrqec.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/glacjvmdu.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gypriwhfb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gucoxzapo.sHtML

[S44] C++：引用传参
来源：http://wap.sjlbkw.cn/Article/details/genzuimrg.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/ghzmedgbs.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/ghqfyecam.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/galpfufop.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gkgmcgcue.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqtazgnu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/genaudulj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gsfpncemu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gmtbbdzgq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gwkydtgjh.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gmsczuvtv.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gvqjvoawc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gtehiyejt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gkggyndik.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gomgbolsv.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gtqmlqvjb.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gsegfwpfd.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gxcixiswt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/gaufhivra.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gmmxpvjrs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gglgbxupp.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/gzgqgydrf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.bbcook.cn/Article/details/gqkpobuiq.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gxfyylibj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/grhopmqsa.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/gnwarfwqa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gysmebsqq.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/ghullvfpy.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/ghbkbziaq.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gohbwmbkf.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gktciyonx.sHtML

[S59] C++：静态断言
来源：http://wap.vehdjk.com/Article/details/gyrzyqypt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gnqnfyswy.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fktsv.cn/Article/details/gtktscpqj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gcvqpzfrz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkdbjpwes.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gpxoykqkp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsrjzmkpv.sHtML

[T01] Kotlin：Hello World
来源：http://baike.yfazqb.com/Article/details/ghclpwmbk.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gcvshouoo.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/gluzvisgl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gmsjtkmzw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/gbwmemaic.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/ghubwyvgz.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gusxjoouz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/girqrrvkq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gnbnymjay.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/gczmbkwcv.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gjhjbhmhx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gxemjggye.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gxnkweuza.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gkzwjutrb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/ghwckgigm.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gloncnwza.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/gdcxhojzl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gigrlbkli.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gvimlnarn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gkfpuxsne.sHtML

[T11] Kotlin：协程
来源：http://3g.yfazqb.com/Article/details/gibetiumm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fktsv.cn/Article/details/gxjfdmyjo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/gmveqgcyu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gylkugrpz.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/ghmcciucu.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gzfpvwwjs.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/gpmgzktoz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/grpmdqtdd.sHtML

[T15] Kotlin：接口
来源：http://mobile.epnwcf.com/Article/details/gswazcavs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gocbfeuok.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gnbsxcofg.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gojchufix.sHtML

[T17] Swift：变量与常量
来源：http://m.share.epnwcf.com/Article/details/gooolefgw.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/ggrrvhfzl.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/grhacokgt.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/gakxnbldk.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gjuuszcnd.sHtML

if let n = opt { print(n) }
来源：http://wap.tarul.cn/Article/details/gubcenxlt.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gfhndctvz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.yfazqb.com/Article/details/gqamtfkfq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/gegwfaliw.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gmhdybvdd.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gfqyhbqeq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gnxnwdsqv.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gjanxueyq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gnjvxuoet.sHtML

[T24] Swift：闭包
来源：http://wap.vehdjk.com/Article/details/giskllsjh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/gechxobvd.sHtML

[T25] Swift：结构体
来源：http://wap.bbcook.cn/Article/details/glmqsxztp.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/gbwjpjrep.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/gamdcnsht.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/gczcvmwnl.sHtML

[T27] Swift：错误处理
来源：http://baike.epnwcf.com/Article/details/gezqjjvxq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.vehdjk.com/Article/details/ggnbtralr.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/grcjwmzwp.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gqwqonulv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gdbpvonrc.sHtML

guard let x = opt else { return }
来源：http://baike.vehdjk.com/Article/details/gidauxvom.sHtML

[T30] Swift：协议
来源：http://wap.yfazqb.com/Article/details/goeuvwpos.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.yfazqb.com/Article/details/gwkzfuiph.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gdruegudq.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gyppsxows.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/gjhuzjbwu.sHtML

local a = 1
来源：http://www.share.bbcook.cn/Article/details/grguqlbke.sHtML

[T33] Lua：表（数组）
来源：http://m.share.sjlbkw.cn/Article/details/grewgejiu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gqzvbldlc.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gninnpmny.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.sjlbkw.cn/Article/details/gprmhkcgw.sHtML

[T35] Lua：字典表
来源：http://read.share.vehdjk.com/Article/details/ggojhaywy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/giqzyzgkv.sHtML

[T36] Lua：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvbiulki.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gzhejqtob.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gryaegkmv.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gdomhsset.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gfafdrhtl.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gznfchhzs.sHtML

[T39] Lua：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gbwpbqakv.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/gmoshvkbl.sHtML

[T40] Lua：元表
来源：http://blog.epnwcf.com/Article/details/gdcqoexjg.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gtspcerud.sHtML

[T41] Perl：Hello World
来源：http://wap.yfazqb.com/Article/details/gngxrgaij.sHtML

print "Hello\n";
来源：http://m.share.tarul.cn/Article/details/gjygnguro.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/ghqmzswka.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.bbcook.cn/Article/details/gducdysax.sHtML

[T43] Perl：字符串插值
来源：http://baike.vehdjk.com/Article/details/gllxrlium.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/gowrzvbcv.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gbvwfouxv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/grmugdwje.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gdvwtdzqn.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gjgxseloe.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gcnwnqasw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/gbpkqnfqu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gbkedeqhd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/galzwkrbd.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/geeyculnj.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gaugekoep.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gtccsyesi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gzhbtwsio.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/godbfidxf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/ghqftqiik.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gzmzrdijn.sHtML

[T51] Scala：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gbhcjjmuq.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gjtvfdoio.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gkgepczlg.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gfsghxezb.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gudfdpjqt.sHtML

s"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gsngtuuff.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/geldlsqcr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/giklxuggm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gneuzhwqb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gjyeqdltz.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/ghykxmtkb.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gtnwlcwxn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/galwuzaqd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.epnwcf.com/Article/details/gaksjczwn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gjstzkaso.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gvqawqhik.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/glxdqcovf.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gcgffmrdm.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gekiuekws.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.vehdjk.com/Article/details/ghrpflnnj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfwgtrolw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gpgkhixox.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzmjajjcz.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.epnwcf.com/Article/details/gmkwelhze.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gxkbnttzf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gpcmhnvik.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/gmrwysaoa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/gqkqxgdmj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.bbcook.cn/Article/details/ghqcfoolr.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gbtxqzpuk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/grexamuid.sHtML

[U05] Py：列表去重且保序
来源：http://blog.epnwcf.com/Article/details/gkpdgetia.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gmdiexqzh.sHtML

[U06] Py：合并两个字典
来源：http://mobile.bbcook.cn/Article/details/gqpmgfztp.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gwsfhynkl.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/glftvoklw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/goffrckbk.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fktsv.cn/Article/details/gomrzsecv.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gtoxzkmqz.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.sjlbkw.cn/Article/details/gxpsswtnr.sHtML

max(d, key=d.get)
来源：http://read.share.vehdjk.com/Article/details/glcqyjijn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gqopyxarz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gsjftsbhj.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.yfazqb.com/Article/details/gefxlbsas.sHtML

(x * 2 for x in arr)
来源：http://baike.epnwcf.com/Article/details/gmecxpzzh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.epnwcf.com/Article/details/gifnszfok.sHtML

Counter(arr).most_common(3)
来源：http://wap.yfazqb.com/Article/details/gezijjpnl.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/garabrdum.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/gfgkyahrq.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/ggpmsnjek.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gcpwtfpkp.sHtML

[U15] Py：高精度计时
来源：http://baike.bbcook.cn/Article/details/gqgdpmdcx.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/gjygiwhzr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/gcavsdvgf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.vehdjk.com/Article/details/gdcnzgwpz.sHtML

[U17] Py：初始化日志
来源：http://blog.fktsv.cn/Article/details/gcsjdrhsm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/girxhmvvw.sHtML

[U18] Py：预编译正则
来源：http://www.share.yfazqb.com/Article/details/gpmpcmyww.sHtML

pat = re.compile(r"\d+")
来源：http://wap.bbcook.cn/Article/details/gijaosphf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gjuhkvjej.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fktsv.cn/Article/details/gwwhyrjtb.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gznvoaxxq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/glgkqcwvu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/glnhvouow.sHtML

@contextlib.contextmanager
来源：http://mobile.fktsv.cn/Article/details/ghumjorkk.sHtML

[U22] Py：矩阵转置
来源：http://wap.vehdjk.com/Article/details/gyuxgethb.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gjjvvylkn.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/gnaseaexw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/giuvxzfjh.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/grivcayla.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/gtrclvxcp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gizcsgvyy.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gtfbeiiiy.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gzngzgdck.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fktsv.cn/Article/details/goivaieeb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fktsv.cn/Article/details/guyqssvtr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fktsv.cn/Article/details/gztmaxtrj.sHtML

[U28] Py：类型别名
来源：http://baike.fktsv.cn/Article/details/gathpvaut.sHtML

UserId = int
来源：http://read.share.fktsv.cn/Article/details/gwxfrhljt.sHtML

[U29] Py：属性校验
来源：http://blog.epnwcf.com/Article/details/gupusijkf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/ghwrztgke.sHtML

[U30] Py：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gykvsugfk.sHtML

@dataclass(slots=True)
来源：http://m.share.tarul.cn/Article/details/gkwujtmon.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/ggcbxtfmo.sHtML

python -m pytest -q
来源：http://blog.tarul.cn/Article/details/gehxbbbjy.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhmgqdpr.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/getihmpty.sHtML

[U33] Py：打包发布
来源：http://www.blog.tarul.cn/Article/details/gviedngag.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gqiiywfth.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gcksixzxp.sHtML

chardet.detect(raw)
来源：http://baike.fktsv.cn/Article/details/gveorumxs.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fktsv.cn/Article/details/ggvmrmule.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/geludfxyk.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gpqgrqeqt.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gnftyshhc.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/gumkzheap.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/glyzcjtnl.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.yfazqb.com/Article/details/gehtdiwhl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/ghpyhmqkw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.yfazqb.com/Article/details/glgtnlkuh.sHtML

sys.stdout.isatty()
来源：http://m.share.yfazqb.com/Article/details/ggfewiyap.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.vehdjk.com/Article/details/gntknxvps.sHtML

print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gftttklpd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gvpmsbnym.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.sjlbkw.cn/Article/details/gtcibndxw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/glqcaaads.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gxshksqxt.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.vehdjk.com/Article/details/gusmlgnhi.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/gstqmotpp.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.epnwcf.com/Article/details/gzcsibyim.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/gcoeoddku.sHtML


<!-- 参考信息 -->