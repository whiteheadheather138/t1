代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/glzqvzfpb.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gfutfwjun.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/ghpjcutfj.sHtML

[S26] C：内存清零
来源：http://read.share.epnwcf.com/Article/details/gnribfxyi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/ghjxrhwau.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gznfuasvn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gmenzgkjv.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/grcwncwnb.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gdwmyboet.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gooknslpc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.epnwcf.com/Article/details/gvqzxrwqk.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gsmgxgdnj.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gqudpdqpg.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gzfcasfjl.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gwpodssfc.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/goxlnhyqk.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gvxxpcfkz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gwyiwdobk.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gyfyxxekh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gcidzfies.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gxohbbznp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gdadgkezj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/ginxhjsck.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/gccmvoumx.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gkebvtezk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gjlrzdvpd.sHtML

[S36] C++：unordered_map
来源：http://mobile.epnwcf.com/Article/details/gimiycmop.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/goswlibsv.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gidadodla.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gndngqvtq.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/gqjrmvsik.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gumrczsnh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gnfqmosnp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/gkztnlbdv.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gkfhcndoa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gtnvzntqx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gpcygukgu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gjgyzwubd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gewxrmnlq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.yfazqb.com/Article/details/gwbexmkya.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gyjvvafwm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gcndlbgoe.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/gpbbkwdug.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gbroaakwl.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gmsqtvnfo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gcpdbdopc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gfzkgfqwk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggsyzgdkb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gxiauemfx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gpgcpguay.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gkwrcnbkj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gcurrhfhj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gikoznbjp.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/ggnhimrke.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gmcpgrdwo.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gztcggijz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gjccydxiz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gyfdyngim.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/glavzzmvn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.epnwcf.com/Article/details/gnamsgwta.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gdhfvwyun.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/ghuaugjct.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gpehfuvrl.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gaxzpykca.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/gzxmzqsyz.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gnbpgmurq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gqetowssm.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gvrjlcsov.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gezxqmgys.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/giyotolmq.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gpcfyptoy.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/gndqaejuo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.vehdjk.com/Article/details/gvamtotji.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gjpakuulk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/guodyczfc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gelfowtch.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.bbcook.cn/Article/details/gtslnxgsp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqbzjgimq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gunahhcxu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdjhxmasu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gquqaczki.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gaaguvkmw.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/gpqijgelg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gbavzikps.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gyqsxpdbc.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gwbwptlwo.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gdxzliadp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/gfpebweld.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/giyzyoryf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/geshsojsq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/guqrhgyxl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/grjaosrmc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gsspzqnyv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gwpxiqpdm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/givbybssh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gkglkimfs.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gyyzqsjfj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/grujtjvqg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gpxijejsq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gqbeounxh.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gkoeyzvdh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gvhjfsdzp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.bbcook.cn/Article/details/gxtjaenzf.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/gerhrywsu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gxrzzntbq.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fktsv.cn/Article/details/gmpyxxlwo.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/gmhtrjibg.sHtML

for (i in 1..10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gnfxnkxjg.sHtML

[T15] Kotlin：接口
来源：http://m.share.bbcook.cn/Article/details/gaseitvcg.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.tarul.cn/Article/details/gfoshpoie.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gfvjeybtm.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/ggieuonmw.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gkfnzmzfg.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/ggachvigq.sHtML

[T18] Swift：字符串插值
来源：http://m.share.vehdjk.com/Article/details/guzsbhuil.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gbebimwsn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gahnuhlkh.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/geoqhqunj.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gplmiknic.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/goeurknvc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/ggfsqjlfq.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gucyezvis.sHtML

[T22] Swift：字典
来源：http://read.share.fktsv.cn/Article/details/gvrbcjksu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gcszljmhe.sHtML

[T23] Swift：函数
来源：http://3g.tarul.cn/Article/details/ghwehlvls.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gnxebgntd.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gawgbhvta.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/gqbvwyhza.sHtML

[T25] Swift：结构体
来源：http://www.m.share.vehdjk.com/Article/details/gpwkofwsu.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/gtizbdszu.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/givzoareu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.sjlbkw.cn/Article/details/gqxfwkdkq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gjrppzqiu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gzfccpocw.sHtML

[T28] Swift：枚举
来源：http://3g.tarul.cn/Article/details/gxirqfpsu.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/gafncelgq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/gmuggxdgf.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gziswujos.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/gvldhnyqm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/gvcdwxbdo.sHtML

[T31] Lua：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gfaalwyos.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhewniea.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/giesxkdlu.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gnsogxpda.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gduymgswg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.epnwcf.com/Article/details/gutmfdtlu.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/gwnnrkxdx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.tarul.cn/Article/details/gzmanodve.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gnufjqkai.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gnujaugbu.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/groenueqj.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/gcijtslck.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gjajnxeiv.sHtML

"a" .. "b"
来源：http://wap.bbcook.cn/Article/details/gzcqfmjxu.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gtelvubte.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gzlwpbhvh.sHtML

[T39] Lua：模式匹配
来源：http://wap.vehdjk.com/Article/details/gmdwyjcmz.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/gezvvjzbr.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/glykzbrqb.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gnjfooaip.sHtML

[T41] Perl：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gsdksyqcn.sHtML

print "Hello\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gvanhecyf.sHtML

[T42] Perl：变量类型
来源：http://read.share.yfazqb.com/Article/details/gymtkvgqo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gjtzvtdez.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/grdgrnlsy.sHtML

"值: $a"
来源：http://wap.tarul.cn/Article/details/gxxpvmxgn.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/gxmladmrc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gyegihjcf.sHtML

[T45] Perl：数组遍历
来源：http://wap.yfazqb.com/Article/details/gvgjxufap.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/ggqbxqhrf.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.yfazqb.com/Article/details/gjppzbhkw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.vehdjk.com/Article/details/gkjpqvjrz.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gitfktson.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gekxpqruk.sHtML

[T48] Perl：正则替换
来源：http://m.share.vehdjk.com/Article/details/gvnfaxvzh.sHtML

$s =~ s/old/new/g;
来源：http://blog.sjlbkw.cn/Article/details/gmkclltpp.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpvxfzga.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoapyhsn.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gyhlttjjh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.vehdjk.com/Article/details/gemzeakjo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/gghriwgaz.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/ggapsdtqt.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gsoqgtfye.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gzknohaoo.sHtML

val a = 1;  var b = 2
来源：http://mobile.vehdjk.com/Article/details/gzqyyibyd.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gpjrfqygm.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/geiccfnra.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/gylgpzssj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gspcnrpgt.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gjvfutbaj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/galrqdzkp.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gnyrjvkzg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gkwnvcobd.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/gjqiwefrx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/gpuyibqpg.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.bbcook.cn/Article/details/glyporgrn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/gzkubplha.sHtML

[T59] Scala：循环
来源：http://read.share.yfazqb.com/Article/details/glstqdpyf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gzauzqcxq.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/ghdjbiuxx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/gpcxhnkwj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkekbubek.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gmkaqebev.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gehfvycbd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gjtvioccz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.yfazqb.com/Article/details/gnmgzvvub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/gizgrtmvj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.bbcook.cn/Article/details/gqaugpdla.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/gzhlasftv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fktsv.cn/Article/details/gxmfjahaq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gzdkimsoe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gmnltcfma.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gpbueoion.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gynjzhucu.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gvxpkpcam.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gctlokjoj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/grsvnofpo.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/gofrbaodl.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fktsv.cn/Article/details/gdqgjfjds.sHtML

[y for x in nested for y in x]
来源：http://www.share.bbcook.cn/Article/details/geyxuaeoe.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.epnwcf.com/Article/details/grbusxstx.sHtML

max(d, key=d.get)
来源：http://m.share.fktsv.cn/Article/details/gtubilfas.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.yfazqb.com/Article/details/ghhpflbqn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gqvlhreko.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gokmbarjp.sHtML

(x * 2 for x in arr)
来源：http://3g.vehdjk.com/Article/details/gpjhwjsao.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.tarul.cn/Article/details/glhmnokgx.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gjlpumtzr.sHtML

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/gwdspuwdy.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gztnhwzzv.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/ggudbtybb.sHtML

defaultdict(list)
来源：http://baike.sjlbkw.cn/Article/details/gjvxhbuew.sHtML

[U15] Py：高精度计时
来源：http://m.share.bbcook.cn/Article/details/gvxflmdft.sHtML

t = time.perf_counter()
来源：http://baike.fktsv.cn/Article/details/gbzeaedns.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gitjldqka.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.epnwcf.com/Article/details/glsknxzxq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.tarul.cn/Article/details/gnvktadtu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.epnwcf.com/Article/details/gstpubqqz.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/gycmextws.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/ghecxmlau.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/givjwyimq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.bbcook.cn/Article/details/gbmtdajdy.sHtML

[U20] Py：缓存函数结果
来源：http://baike.bbcook.cn/Article/details/gzclzjtva.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gcwvkvdqf.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/ghveffpzn.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gsloahueh.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/gviifcmki.sHtML

list(zip(*m))
来源：http://baike.yfazqb.com/Article/details/gojrcdcyo.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.vehdjk.com/Article/details/gagsldpmt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gesdtunbc.sHtML

[U24] Py：路径操作
来源：http://www.share.tarul.cn/Article/details/gfthayibz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/ggijxpwty.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.epnwcf.com/Article/details/gcdnaotsc.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gucwourpn.sHtML

[U26] Py：并发下载
来源：http://wap.tarul.cn/Article/details/gauzbpomx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.epnwcf.com/Article/details/gtxhmtces.sHtML

[U27] Py：异步 HTTP
来源：http://blog.vehdjk.com/Article/details/gzfkpiwvw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gzscwprug.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/gguqwmvhz.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/ggqgcnqpf.sHtML

[U29] Py：属性校验
来源：http://3g.fktsv.cn/Article/details/grudpclwd.sHtML

@property 与 @x.setter 配合
来源：http://read.share.vehdjk.com/Article/details/gveszxeti.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/gubjoxage.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/gxjddfvgn.sHtML

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/geoglfinr.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gtcmhdqep.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gywblzqux.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.vehdjk.com/Article/details/gghvqvxja.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gztnuants.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/garfigwte.sHtML

[U34] Py：判断编码
来源：http://blog.fktsv.cn/Article/details/gapndrnco.sHtML

chardet.detect(raw)
来源：http://www.m.share.epnwcf.com/Article/details/gcniywrhj.sHtML

[U35] Py：发送邮件
来源：http://www.share.fktsv.cn/Article/details/ggajzdomk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.sjlbkw.cn/Article/details/gnhwqayzr.sHtML

[U36] Py：定时任务
来源：http://blog.yfazqb.com/Article/details/gdardywjh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.sjlbkw.cn/Article/details/gagjwyfvr.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/gyyffyngg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gfyytmsbg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.vehdjk.com/Article/details/gfvuupfpa.sHtML

Path(__file__).resolve().parent
来源：http://baike.bbcook.cn/Article/details/gqwazirtl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.yfazqb.com/Article/details/gxsfejeel.sHtML

sys.stdout.isatty()
来源：http://www.share.epnwcf.com/Article/details/gsspvzatk.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/gvqymukje.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gvgrxewwe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/gutskalno.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fktsv.cn/Article/details/gtepfxomp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.tarul.cn/Article/details/gzbjpzrnb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.bbcook.cn/Article/details/gkwjigwjt.sHtML

[U43] PHP：声明命名空间
来源：http://wap.epnwcf.com/Article/details/ggcmbntne.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/gxtnatndq.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/gpfktkcip.sHtML

declare(strict_types=1);
来源：http://mobile.fktsv.cn/Article/details/gbkzfrtmv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/gwxfzbtuk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gvgeucsyk.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gkkblldor.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gzoomuigf.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gcevtkcli.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gxcjlncwl.sHtML

[U48] PHP：纯枚举
来源：http://3g.tarul.cn/Article/details/gbjkpixcp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.tarul.cn/Article/details/gxcnjmlfz.sHtML


<!-- 参考信息 -->