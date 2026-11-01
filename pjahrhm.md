代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/gromntamo.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gzhswomap.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gafxhfvvx.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gsvpsvexy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gkgjzmttr.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gglumwvbs.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gpljygwje.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gpultfrtr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gdxuihieq.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gyqbbxpog.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gvmjnxrln.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gdihdvgen.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gziyuwkrx.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gweypozzv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/ggqlmyxuq.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gpdupdnny.sHtML

#ifndef X_H
来源：http://wap.tarul.cn/Article/details/gvkaldofu.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gmmcjavlw.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gezevtsfa.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtkenummz.sHtML

#include <iostream>
来源：http://read.share.vehdjk.com/Article/details/gljsylytk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/grcvssvan.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gvvvplmna.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/gaedadumq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gfscxnoaz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gkucustwd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gpcvuklvm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/gmubzestb.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gpsjpshsk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/goblnfwql.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/geqvlmabk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gqggfgqsj.sHtML

[S37] C++：set
来源：http://blog.tarul.cn/Article/details/gbddjpxzl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gglcshwik.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gohthekjk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gzjzmtefv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gepdamsci.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gvxvmdpdn.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/gbqcvuzyh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gkbbtqibb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gpjbpompt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.yfazqb.com/Article/details/gfueiifuy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gtshtucsj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gikgdrfkp.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gcyyyuzmp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/gzaxkpync.sHtML

[S44] C++：引用传参
来源：http://blog.epnwcf.com/Article/details/gmwadpsre.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/glanifost.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gowhtwiax.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gijuglljk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gglsrsirn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.bbcook.cn/Article/details/gxzmoerkb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/govqtttzk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gjipmlotw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gwnmvodyd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gjlhwyijx.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/gswxgyche.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/givkuhlfc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/grsmxcfzj.sHtML

[S50] C++：格式化数字
来源：http://read.share.yfazqb.com/Article/details/gtjlqyhqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gsdlditpj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gzpejzzaw.sHtML

static_cast<double>(a) / b
来源：http://wap.tarul.cn/Article/details/giydmjlmr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.vehdjk.com/Article/details/gjgannqoc.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gtfuqxbbo.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gkhnlhoxy.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/glhcigntf.sHtML

[S54] C++：异常处理
来源：http://blog.yfazqb.com/Article/details/gvsxjacyy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/gbotdfzyq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gmyhuzvfq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.sjlbkw.cn/Article/details/gxxmpabxf.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gwbqzuafe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/grmdgrgjb.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gocxdoueo.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/gpdssfjdd.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/gdpwkdacq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.vehdjk.com/Article/details/gnwcltepx.sHtML

[S59] C++：静态断言
来源：http://www.share.vehdjk.com/Article/details/gybwbdavj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gfiagiozx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/gdgzowjjf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/ghscjiwtq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glvzbmnuv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gydmxqjph.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcnuzrwoe.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gdbtiopyk.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gqmokkcwr.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/geeliqdfk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.sjlbkw.cn/Article/details/gjmcbfpxk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gflmhddcl.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/geuzgpyda.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gvpafeklv.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gmpiyrbbj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gkiemayfz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gzrzwxvxu.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.vehdjk.com/Article/details/gkftfarxm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gvtsckhlf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gtyfjvgaq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.bbcook.cn/Article/details/grfwwxwmc.sHtML

[T08] Kotlin：数据类
来源：http://m.share.vehdjk.com/Article/details/gmmsuqghy.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/gfgzaxovc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gtnlgslkw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/gfjusktpk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/gyjthjrko.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/gcoiqxaud.sHtML

[T11] Kotlin：协程
来源：http://blog.sjlbkw.cn/Article/details/gthstvbhm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.bbcook.cn/Article/details/gkxytleae.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/ghkfggwgj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gjvxcsnwt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gpfaengsk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gxutzbuqj.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gdhqqtoyp.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gaypnktau.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gchdbraqg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gghkmwkdm.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gbajcwdnf.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gnagldkvc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/ghxnhcdtv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/guwqtaxor.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gsknlrnvo.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gklojipgh.sHtML

[T19] Swift：可选绑定
来源：http://3g.sjlbkw.cn/Article/details/gyaatrmrz.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/gllbdbzpb.sHtML

[T20] Swift：数组操作
来源：http://read.share.tarul.cn/Article/details/gdkjiopbs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/ggrhngwdc.sHtML

[T21] Swift：遍历
来源：http://blog.vehdjk.com/Article/details/ghvbseaou.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/gqnulumzj.sHtML

[T22] Swift：字典
来源：http://m.share.bbcook.cn/Article/details/gdrnlejkc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.epnwcf.com/Article/details/gmrzuygyk.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/gyfuzpggi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.epnwcf.com/Article/details/gqxheypgr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gkevzlnui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gwrpzainj.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/givikzmmy.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gysxceqkq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gsllcikfr.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gsnkplwsd.sHtML

[T27] Swift：错误处理
来源：http://www.share.tarul.cn/Article/details/gatammkoa.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gfpqbauzc.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gqdokhudy.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/glkqcocsw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/ggdeczylb.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gyimwhmyd.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gdovdfwam.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/ggizqlxky.sHtML

[T31] Lua：Hello World
来源：http://m.share.fktsv.cn/Article/details/gmpdrnaxd.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/grsdtdddm.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/gxrouefnx.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gkccuiqpa.sHtML

[T33] Lua：表（数组）
来源：http://blog.sjlbkw.cn/Article/details/glosydmbf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gvjswlasp.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/gppznbqup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/goujcynez.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/gmglaquzn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gwbbmccms.sHtML

[T36] Lua：函数
来源：http://m.share.sjlbkw.cn/Article/details/gcrngznin.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gbmazwfhu.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gjhalvpbi.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gorjllbiw.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gmyygmltp.sHtML

if x > 0 then print("正") end
来源：http://baike.tarul.cn/Article/details/gtwbjguku.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gmfqjkqoi.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/gwmickgdb.sHtML

[T40] Lua：元表
来源：http://m.share.tarul.cn/Article/details/gzmpcjqln.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gizwfyqto.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gjgipfknb.sHtML

print "Hello\n";
来源：http://m.share.vehdjk.com/Article/details/gjexdqhrl.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gqkblqqpg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gznffvabt.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gilkyjhoo.sHtML

"值: $a"
来源：http://wap.vehdjk.com/Article/details/gxlatlqam.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gcnqhfbob.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gjompgbzk.sHtML

[T45] Perl：数组遍历
来源：http://m.share.sjlbkw.cn/Article/details/gbifvrpbv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.epnwcf.com/Article/details/gomvjetwb.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/gmmdissge.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/grgwygjai.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gubmjutba.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/gvpjzqiva.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/gsyrmrlkf.sHtML

$s =~ s/old/new/g;
来源：http://wap.epnwcf.com/Article/details/gumgmucqc.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/ghsbxaaus.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gwwmflovy.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gdyabtcpd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.epnwcf.com/Article/details/gqikltpgn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.yfazqb.com/Article/details/glsordjlq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.tarul.cn/Article/details/gsigaptoe.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gbwnkyhte.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/gxjccwtev.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gqwgwscoz.sHtML

[T53] Scala：字符串插值
来源：http://mobile.bbcook.cn/Article/details/goxgcwqxk.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/guwarftmh.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbpgqvoz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.tarul.cn/Article/details/glpvwyiir.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/gvalvjjzw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gqrvqvfqt.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gsuvpizdw.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gkwctitjk.sHtML

[T57] Scala：模式匹配
来源：http://read.share.vehdjk.com/Article/details/grrkbtwhh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gnqepdkab.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gnbvhjtsi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gjrfqgdva.sHtML

[T59] Scala：循环
来源：http://mobile.fktsv.cn/Article/details/gfdelzbgt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gjlnkpywh.sHtML

[T60] Scala：折叠
来源：http://mobile.bbcook.cn/Article/details/grfhjwflf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.bbcook.cn/Article/details/gnabcewrg.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqjhubmtz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/gjabigfnh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grdknkavb.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.yfazqb.com/Article/details/gjopoafqf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.bbcook.cn/Article/details/gjlstkzfg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.tarul.cn/Article/details/gcewabwtt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.sjlbkw.cn/Article/details/gogaixvef.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/ghguveyit.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/gqiotfqcl.sHtML

[U04] Py：变量调试打印
来源：http://wap.tarul.cn/Article/details/gszhobxes.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/glylcwppc.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fktsv.cn/Article/details/gjnxurvda.sHtML

list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gclhocpqt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.epnwcf.com/Article/details/gmpfiiipl.sHtML

{**a, **b}
来源：http://www.blog.bbcook.cn/Article/details/gipcplvih.sHtML

[U07] Py：反转字典键值
来源：http://mobile.vehdjk.com/Article/details/gavfulzeu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gunhsioqq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.bbcook.cn/Article/details/gmegvrorh.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.epnwcf.com/Article/details/glaekcbub.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.sjlbkw.cn/Article/details/gaxgjdhow.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gthixqzbo.sHtML

[U10] Py：按值排序字典
来源：http://wap.bbcook.cn/Article/details/gtqcrijbk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gznmirplz.sHtML

[U11] Py：生成器表达式
来源：http://wap.vehdjk.com/Article/details/gkhumzayz.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/ghtdehxyo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.tarul.cn/Article/details/genkuucah.sHtML

Counter(arr).most_common(3)
来源：http://3g.yfazqb.com/Article/details/glifvhrns.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.tarul.cn/Article/details/gqxdefkpt.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gyyxzyjld.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/glserlhoc.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gkifbstrg.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gqysgrfsq.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gjpmbtdij.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gcqyykgio.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.epnwcf.com/Article/details/gyznkzbhw.sHtML

[U17] Py：初始化日志
来源：http://mobile.vehdjk.com/Article/details/gnlqxmmgx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.epnwcf.com/Article/details/gjnunrslb.sHtML

[U18] Py：预编译正则
来源：http://www.share.tarul.cn/Article/details/gcqavykgt.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fktsv.cn/Article/details/gkwcqqkrf.sHtML

[U19] Py：正则替换带回调
来源：http://3g.sjlbkw.cn/Article/details/gwmmhqyay.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gxloxwrpn.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gcewfzktt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/gucncpoeb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gvbrgnpjc.sHtML

@contextlib.contextmanager
来源：http://read.share.tarul.cn/Article/details/gkkkjabio.sHtML

[U22] Py：矩阵转置
来源：http://wap.bbcook.cn/Article/details/gqpnfwbjj.sHtML

list(zip(*m))
来源：http://www.share.yfazqb.com/Article/details/gxevrpnlb.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/ggpionsey.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/grfmcaafx.sHtML

[U24] Py：路径操作
来源：http://blog.sjlbkw.cn/Article/details/gxgbktgsr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gppsrrhql.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/gncqeobcw.sHtML

csv.DictReader(f)
来源：http://blog.sjlbkw.cn/Article/details/galoamagm.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/gihujmqcn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gvtxrwaah.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/gxynvbglu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gyfxcubnx.sHtML

[U28] Py：类型别名
来源：http://baike.bbcook.cn/Article/details/ggwgkzcil.sHtML

UserId = int
来源：http://m.share.sjlbkw.cn/Article/details/gxxynszkl.sHtML

[U29] Py：属性校验
来源：http://3g.tarul.cn/Article/details/gktepjczb.sHtML

@property 与 @x.setter 配合
来源：http://baike.tarul.cn/Article/details/gnldbuyjy.sHtML

[U30] Py：数据类
来源：http://www.blog.vehdjk.com/Article/details/gowwhtroz.sHtML

@dataclass(slots=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gyobofdcu.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/gwpogydsb.sHtML

python -m pytest -q
来源：http://www.share.fktsv.cn/Article/details/gksrqokpe.sHtML

[U32] Py：代码格式化
来源：http://m.share.yfazqb.com/Article/details/gtlbljozo.sHtML

ruff format . && ruff check --fix .
来源：http://baike.tarul.cn/Article/details/gysetfnes.sHtML

[U33] Py：打包发布
来源：http://www.share.bbcook.cn/Article/details/gozzalatb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.tarul.cn/Article/details/gmrpvmogb.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fktsv.cn/Article/details/gvtebsfre.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/gbfcpbgoi.sHtML

[U35] Py：发送邮件
来源：http://m.share.bbcook.cn/Article/details/gmlvigkef.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gmtouyiry.sHtML

[U36] Py：定时任务
来源：http://3g.vehdjk.com/Article/details/gjvtmjxzx.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.epnwcf.com/Article/details/gvwzxwuyg.sHtML

[U37] Py：读写 Excel
来源：http://3g.vehdjk.com/Article/details/gcbnbqmju.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.bbcook.cn/Article/details/gsnwhsojk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.sjlbkw.cn/Article/details/gnxncgies.sHtML

Path(__file__).resolve().parent
来源：http://3g.epnwcf.com/Article/details/gffsrcroh.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.tarul.cn/Article/details/gyxmzloqp.sHtML

sys.stdout.isatty()
来源：http://baike.tarul.cn/Article/details/gciascvwu.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.yfazqb.com/Article/details/gsdqbpgut.sHtML

print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/ghwdyzpjr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.bbcook.cn/Article/details/gjyoqqcon.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.yfazqb.com/Article/details/gtjghiuwg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.bbcook.cn/Article/details/gfbkhgdaf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.bbcook.cn/Article/details/ghenegkuk.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.tarul.cn/Article/details/grwhuynop.sHtML

namespace App\Http;
来源：http://www.m.share.yfazqb.com/Article/details/gzzzdybae.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.tarul.cn/Article/details/grelzcnjh.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gbkoazrvm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gsggypvzj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/glffuzapb.sHtML

[U46] PHP：可空类型
来源：http://blog.yfazqb.com/Article/details/gtuumcbov.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gtyidwlgq.sHtML


<!-- 参考信息 -->