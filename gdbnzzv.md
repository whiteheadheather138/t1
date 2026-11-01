代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.bbcook.cn/Article/details/gtosjtxxq.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gkjsrwqbi.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gorooozsw.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/ghhjvldcr.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gvmbkovvd.sHtML

[S27] C：定义常量
来源：http://3g.yfazqb.com/Article/details/gbkhipeiy.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gopathyvg.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gbnecikxr.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gdmyyafie.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gxbrktpii.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/gujquohcw.sHtML

[S30] C：头文件保护
来源：http://read.share.vehdjk.com/Article/details/ggbctpjqg.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/ggowufmnl.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gxqugdiiy.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/gbrsxyevj.sHtML

[S31] C++：Hello World
来源：http://mobile.yfazqb.com/Article/details/gzykgyzqv.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gtfbrrscw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/ghinromxe.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/ggqisvuyd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gsymfifun.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/gcdzczixk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gubptlzhf.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/ghmcsftet.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fktsv.cn/Article/details/glkdshthl.sHtML

[S35] C++：map
来源：http://wap.sjlbkw.cn/Article/details/ggfpfkdnv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gvtlqbgml.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gdpuilvma.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gizxnzcsf.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gklbqcxpq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/goycbgftp.sHtML

[S38] C++：排序
来源：http://wap.epnwcf.com/Article/details/gaimwqdro.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gidqrhglu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.epnwcf.com/Article/details/gnlsqizkp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gxmiwfkcg.sHtML

[S40] C++：查找元素
来源：http://baike.vehdjk.com/Article/details/gywsemfru.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/gzundeppo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.epnwcf.com/Article/details/gylozbbvo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gyycfrjvy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gvzqdjbng.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/gkphevevs.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gxdfsecoj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gjqvbfsue.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/gmfvinsgv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/grajcgekl.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gtvchwakd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gmkchtzqq.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gintipfou.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/gihugovpw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/gugahxgky.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/ggyuzyxis.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/glogrttzl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gsrafxpxd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gyjchyagv.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gjnozbjsu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gdzqzjahe.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gkxvwfrpq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gmjeschor.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gtrsluplp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/giimelbba.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.epnwcf.com/Article/details/gewbeiylf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/gizjjnawn.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gtpwpxfva.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gqcuenrpj.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gvvyeqbtp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/ghncgzxss.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/gbsishnfd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gzbqjeldp.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gazsfbiwc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.vehdjk.com/Article/details/gexeadevg.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gsmhxqluj.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gofewnsbi.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gupjvtgov.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/ggpwguwgh.sHtML

[S59] C++：静态断言
来源：http://www.share.bbcook.cn/Article/details/gluatmibm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.vehdjk.com/Article/details/gjldejjva.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/gnkwiikkh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gwqmysxzq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfakhladt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gmvryrcpk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/giwrfqzzy.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gbifotisk.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/getwobldc.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/ghvzwpfid.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fktsv.cn/Article/details/gskxqzogc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gxevapawb.sHtML

"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gmjtvbjyl.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gbmdenmys.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/garnrhvuj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.sjlbkw.cn/Article/details/gzkturway.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.bbcook.cn/Article/details/gsblgeayh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gwtjvtlzq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/giulywgii.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gugduotbq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gsajbhxqy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/gpskperol.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fktsv.cn/Article/details/gjjpclztt.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gplpezxou.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gswvysdps.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gaezccwfq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.bbcook.cn/Article/details/gnrtdqnhp.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/ghqmnxznv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.vehdjk.com/Article/details/gqnetqhjk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/ggudkjuws.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gvnpqoapm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gupbomjzi.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gaseyovaq.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gkdpruwrd.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gkkbjvvdi.sHtML

[T15] Kotlin：接口
来源：http://m.share.sjlbkw.cn/Article/details/gehvgeeki.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/grgkusupc.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/ghtwanbki.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gyhtjwxgc.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gzmfvzkmz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gwqbzzhcm.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gxzgwsdpt.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gksaaikpk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.sjlbkw.cn/Article/details/ghibbetdo.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gpwfivnez.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gzhuhgozy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gcuspydve.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gobfqnxyz.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gaqafbjfn.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gqrxmymhz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gefmgipcv.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/gqtbomgdj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gjlgcjjlf.sHtML

[T24] Swift：闭包
来源：http://mobile.yfazqb.com/Article/details/gymgdilwf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gibzaslxl.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gngbciwcg.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gkliycfex.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gasypefjo.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gsvstvogk.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/gcewafedk.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.epnwcf.com/Article/details/gjqdkwwxt.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gajrverpr.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/gbphaxakt.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.vehdjk.com/Article/details/gisaeowho.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gggcgggrz.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gysnjokly.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.vehdjk.com/Article/details/grpnlkyfg.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gmoaujqnz.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/ghetzcmsk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.yfazqb.com/Article/details/gdqfzlwau.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gsrjjhpof.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gbaczvpja.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gbzavazvd.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/gnenxmrdf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/ghgytxlac.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gnrpabjrl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.bbcook.cn/Article/details/gmkknmsuo.sHtML

[T36] Lua：函数
来源：http://m.share.sjlbkw.cn/Article/details/gqzjcjncb.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gnhmvorvp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/guecwsaup.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gwsnbmniv.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gsbanseto.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gkufhebhj.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/gbtosyimy.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gbztxqqrq.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/gteipxkzn.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gjqtqpedh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gjgcwimcf.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gixwyqahx.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gkjwijnho.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/ghadyfzgi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gjxrstxag.sHtML

"值: $a"
来源：http://baike.sjlbkw.cn/Article/details/gbvdgjrmz.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/guqljbpfp.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gewiazyzu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/gplqzqfps.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gauiasdkh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.yfazqb.com/Article/details/gdmrqwipl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gaacdmatc.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.sjlbkw.cn/Article/details/gorirepmq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.yfazqb.com/Article/details/gbcmbjrjb.sHtML

[T48] Perl：正则替换
来源：http://read.share.bbcook.cn/Article/details/gfebfchhw.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gniblmzfg.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gfuxudbse.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/grbmcytqu.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/ggexuvsoj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.epnwcf.com/Article/details/gwbzipuik.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gihqeyckr.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/grzjwzetn.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gclpdzemw.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gbtnzprnp.sHtML

val a = 1;  var b = 2
来源：http://blog.yfazqb.com/Article/details/gdhpdcafx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gatfdsnbx.sHtML

s"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gqfnzljof.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gbpswahvg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.tarul.cn/Article/details/gxoqtzkbz.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/gxphzhvnu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gjoznqlej.sHtML

[T56] Scala：样例类
来源：http://mobile.epnwcf.com/Article/details/grhdtrzrd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/girjoovbx.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gkqavjwdo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.bbcook.cn/Article/details/gmuchrvgt.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/grqwblruv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/gfnhenbbg.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/guwhsnsom.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.epnwcf.com/Article/details/gqjoehdla.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/govodflbl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gxvesbqpe.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmraagufp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gxqqixrxj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbsjtehoc.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.tarul.cn/Article/details/gnxwhyyig.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/gmvskpedh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/ggwjinwxj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/grptkgkqi.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.epnwcf.com/Article/details/gdtjdlttb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/gybtnyfmg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.sjlbkw.cn/Article/details/gwcrandoo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.bbcook.cn/Article/details/gbsprjsfn.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gqbhsiuzh.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gtiknhaha.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/gamcjfgjt.sHtML

{**a, **b}
来源：http://mobile.sjlbkw.cn/Article/details/gfjtxxrxg.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/gkmsuzers.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/ggplvllwv.sHtML

[U08] Py：展平二维列表
来源：http://m.share.epnwcf.com/Article/details/ggnvsiqpq.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/guczvaafp.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.bbcook.cn/Article/details/gooojoeow.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/gqbnzurul.sHtML

[U10] Py：按值排序字典
来源：http://read.share.sjlbkw.cn/Article/details/gflyzyvbn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.tarul.cn/Article/details/gpljzcmoa.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gpswaoxus.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gcszoqmcc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gryxyzmlq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gkhhvvtch.sHtML

[U13] Py：固定长度队列
来源：http://read.share.vehdjk.com/Article/details/gomeevoop.sHtML

deque(maxlen=10)
来源：http://blog.fktsv.cn/Article/details/gtclmjrgt.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gdzwubctp.sHtML

defaultdict(list)
来源：http://www.share.epnwcf.com/Article/details/gnuxrietx.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gprznkfez.sHtML

t = time.perf_counter()
来源：http://3g.vehdjk.com/Article/details/glcjbcqil.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/gheejoeqm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.vehdjk.com/Article/details/gwxjukxcu.sHtML

[U17] Py：初始化日志
来源：http://read.share.bbcook.cn/Article/details/gybnircez.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.vehdjk.com/Article/details/gdgkizsgt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.tarul.cn/Article/details/gqjcsdyta.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gorkvpydg.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.epnwcf.com/Article/details/gusjfnogd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.yfazqb.com/Article/details/glzraativ.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.yfazqb.com/Article/details/glihdlukl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gohbqinyk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.tarul.cn/Article/details/gncsxckav.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gxtoafmxm.sHtML

[U22] Py：矩阵转置
来源：http://mobile.yfazqb.com/Article/details/garhmechc.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/gqhhgvpyv.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.tarul.cn/Article/details/gshpesqln.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.tarul.cn/Article/details/ggwypyxvq.sHtML

[U24] Py：路径操作
来源：http://m.share.tarul.cn/Article/details/gmusdcppw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/ghtpwmhig.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.bbcook.cn/Article/details/glvlgyksz.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gprwwyjvi.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gkpxzlqdy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.vehdjk.com/Article/details/gdxeenvhk.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.vehdjk.com/Article/details/gqpiproxr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fktsv.cn/Article/details/gtxjjehys.sHtML

[U28] Py：类型别名
来源：http://wap.yfazqb.com/Article/details/gptqgaofi.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/goeacigmu.sHtML

[U29] Py：属性校验
来源：http://m.share.yfazqb.com/Article/details/gsnlzptjh.sHtML

@property 与 @x.setter 配合
来源：http://baike.sjlbkw.cn/Article/details/gyzulcjhs.sHtML

[U30] Py：数据类
来源：http://read.share.vehdjk.com/Article/details/grpblvlud.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/ghmnhetzl.sHtML

[U31] Py：单测
来源：http://wap.epnwcf.com/Article/details/gwvdyfxrd.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/gmuhlwkhy.sHtML

[U32] Py：代码格式化
来源：http://baike.vehdjk.com/Article/details/ggyneakag.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.bbcook.cn/Article/details/gmjwdtzop.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fktsv.cn/Article/details/glktexpjf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.yfazqb.com/Article/details/gduplxjdw.sHtML

[U34] Py：判断编码
来源：http://www.blog.sjlbkw.cn/Article/details/gsppuwmbn.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/gnuvhfred.sHtML

[U35] Py：发送邮件
来源：http://3g.sjlbkw.cn/Article/details/gfgpjchmx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/gymwtvadv.sHtML

[U36] Py：定时任务
来源：http://baike.fktsv.cn/Article/details/gootopilj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.sjlbkw.cn/Article/details/glheufrrs.sHtML

[U37] Py：读写 Excel
来源：http://mobile.tarul.cn/Article/details/gjvemhnkc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/gwdqhyxoz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fktsv.cn/Article/details/guvrjbage.sHtML

Path(__file__).resolve().parent
来源：http://www.share.yfazqb.com/Article/details/gbmluyvwb.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/glkykrugg.sHtML

sys.stdout.isatty()
来源：http://www.blog.fktsv.cn/Article/details/gbhkhspql.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/golykikro.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gauoaoepe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gptpdviad.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.epnwcf.com/Article/details/gnopehfxw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.bbcook.cn/Article/details/gqlqlnqhq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/gdbzwvvxr.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fktsv.cn/Article/details/gwafytajg.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gssqvkgvc.sHtML

[U44] PHP：开启严格类型
来源：http://3g.tarul.cn/Article/details/ggodtdssa.sHtML

declare(strict_types=1);
来源：http://www.blog.yfazqb.com/Article/details/gscemqslu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.bbcook.cn/Article/details/gzwociwww.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gzqmtdxuy.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/gwxktkkph.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gnwgvqazu.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gntkxnomk.sHtML

int|string $id
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnmaauct.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gfoviukla.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gafhjpkys.sHtML


<!-- 参考信息 -->