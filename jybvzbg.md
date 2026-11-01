代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.epnwcf.com/Article/details/gpbszdwba.sHtML

[S25] C：内存拷贝
来源：http://3g.bbcook.cn/Article/details/gjleyaghp.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/guxbllzwh.sHtML

[S26] C：内存清零
来源：http://www.blog.fktsv.cn/Article/details/gklissiqq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/gopddvrlv.sHtML

[S27] C：定义常量
来源：http://3g.tarul.cn/Article/details/gjzbiieop.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gojfenkvj.sHtML

[S28] C：静态变量
来源：http://mobile.yfazqb.com/Article/details/gzdolnzwg.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gvhhhbmqs.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/ghkzqudsj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gqqpdsawt.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gmqpyuhdq.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/giesibqvh.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gkeiafjtl.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/gnrmlrnml.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gncrhdido.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/gbtjxkogp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gbbvshxfn.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/giyemvamo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/gzqduxbab.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gwxxkihxf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/grvpynrwb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/giwitfaoj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gvbrqckgc.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gjnuvilma.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfnjesdt.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gofthcakf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gualqdwbo.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gaqdrzscx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gfwrxxxrk.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/grwxeqvhv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gkuedanof.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gndeyvvxl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.bbcook.cn/Article/details/gtxcelmgd.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/geludxzwf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gvdzmzkni.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gwhplodqp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/graeweumg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gcsvjrkme.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gfulcglsp.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gzvefgzjz.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gqtznbhcp.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/gtrccvxrv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/geidcjoyk.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gltlzxfzh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gkttbzffn.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/goebvnlhc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/ggplmtvge.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/grmsrphpb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/ghbfdjddm.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gjoioewmb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/glsxhrygi.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnitfbiix.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/gpsfnbcbp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.vehdjk.com/Article/details/gtctkiawl.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gxcrxzesj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gdshqhfoj.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gqmtdbodk.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gvywswino.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.sjlbkw.cn/Article/details/gxxxxlaun.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gowxaozbx.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/gozybjtiy.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/ghefmxegc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gmakqewkd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gfgxizppr.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/guplmaixn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gbiwyyuaj.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/glduckvzx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.tarul.cn/Article/details/glvdrswig.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/ghckjszqg.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gyfbvvmhe.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/godcudrdk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.epnwcf.com/Article/details/gzgbbhbru.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gdxgjhpyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gvjbucjmb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/ghgwrhadl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gaizxmgwm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdbaafnsb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/geklczudf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gociustnc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.bbcook.cn/Article/details/gbcmzrlxi.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gowwjrcqi.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gpkiexvlg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/ggytpiuse.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/guddorbug.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/giqcewswx.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/ghtubiwwb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gebntqife.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/guabuezio.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/glrzogvcw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/gaialpouj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gmhjrpkbu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gcbjmxfqq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gxtzmmbjf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.vehdjk.com/Article/details/gyklbcmpj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/geyguaxhr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gejmtkygd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gfebjhbof.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/gtxjpykoy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/gmdsjfvec.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/ggxsiqfbt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gchpohwxq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.bbcook.cn/Article/details/gwgjgtmpg.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/ghjcobuax.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.vehdjk.com/Article/details/guhsxarft.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gmlujivuc.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/giyhawdsr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gpdcbkyqf.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gcqzlknnv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/ghqhssspw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gryibgnxw.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/ggccjpmue.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/goanhbwbj.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gkptbqkzp.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gpetggveu.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gnzicfrfa.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gqdqrnown.sHtML

if let n = opt { print(n) }
来源：http://www.share.vehdjk.com/Article/details/gotnevxdy.sHtML

[T20] Swift：数组操作
来源：http://www.blog.yfazqb.com/Article/details/gejwszhhv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.yfazqb.com/Article/details/gzaqrrrwq.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/gvgicxlux.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/goafbylmj.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/ghjpxhwni.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.bbcook.cn/Article/details/gsipgfvaw.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gvgsatxnb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.yfazqb.com/Article/details/gjmxynzki.sHtML

[T24] Swift：闭包
来源：http://m.share.sjlbkw.cn/Article/details/gbjnlznub.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gxpbputby.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/gqdvpdcci.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gmslrjyoo.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gewpewnvj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.yfazqb.com/Article/details/gljfasyli.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gyqbqyyoo.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/ggbrvanap.sHtML

[T28] Swift：枚举
来源：http://m.share.fktsv.cn/Article/details/gxvdwjooq.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gmlgtmxyy.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.vehdjk.com/Article/details/ggxfhuryq.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gqwflpiaq.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/ggwxnjpwu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.yfazqb.com/Article/details/geeqmtehb.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpjvzvtg.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gmxreqbgf.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gddtdsdam.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gtbkizduv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.epnwcf.com/Article/details/gbdssqxgh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fktsv.cn/Article/details/ghkxbtzgq.sHtML

[T34] Lua：遍历表
来源：http://www.share.epnwcf.com/Article/details/gjdgtqcqo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/gebychrod.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gvjvpwznf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gtipvuhsk.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/gvdtvqqlu.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gfwhfbvkb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/gkwrgvzzn.sHtML

"a" .. "b"
来源：http://wap.tarul.cn/Article/details/gvkcwslmn.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gjmjdlvxw.sHtML

if x > 0 then print("正") end
来源：http://m.share.bbcook.cn/Article/details/grryiqjye.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/gqbnwuofp.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gyviypuzt.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gdxndezul.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/guqzmiusv.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/grdajlrgv.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gtanaawhx.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/gczuxvsff.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.epnwcf.com/Article/details/gagmgoypl.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gevleudiy.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/ghvqifpyb.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/gzdufmzzc.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gccmjdoli.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/grldcvrmz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gmriqndum.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gzqstoyas.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/giimzvqab.sHtML

[T47] Perl：正则捕获
来源：http://mobile.vehdjk.com/Article/details/gbswyobob.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.epnwcf.com/Article/details/ghoeyguuv.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gzlwckypb.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/grxpyrozq.sHtML

[T49] Perl：函数
来源：http://mobile.sjlbkw.cn/Article/details/gmhwzrvqp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gzlrwlazo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gzxmomlmm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.tarul.cn/Article/details/goeyuqdka.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.yfazqb.com/Article/details/ghgoopevu.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gobsggbaf.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gsxtuarmo.sHtML

[T52] Scala：变量
来源：http://m.share.fktsv.cn/Article/details/gylxdyspt.sHtML

val a = 1;  var b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gyldeawlg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/ghbyrksbr.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gvgdxzdsr.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gvocnkxrb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/ggtvoqgzc.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/gebbwbdvj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/ggfbmohrm.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/ghfwdwdob.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gqatrwbzw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/gcvjettlz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gjyladspy.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gibywwjsj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.vehdjk.com/Article/details/ggarjovps.sHtML

[T59] Scala：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gyjpzdyre.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gdckjlfbv.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/gglhlkjsm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/glufiqpik.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqktjiexn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/gleddnahd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gidjxxgfl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fktsv.cn/Article/details/gzykpbtre.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/ghoyvmwxm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gxkqgucew.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gsorwabjz.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/gyozcbxqs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/glfzbhlwq.sHtML

[U04] Py：变量调试打印
来源：http://wap.bbcook.cn/Article/details/ginsautoq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.epnwcf.com/Article/details/gftclyieo.sHtML

[U05] Py：列表去重且保序
来源：http://3g.yfazqb.com/Article/details/gddgftddh.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gwwiejoaw.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gmrktiuxv.sHtML

{**a, **b}
来源：http://blog.epnwcf.com/Article/details/gkectvwkn.sHtML

[U07] Py：反转字典键值
来源：http://blog.yfazqb.com/Article/details/gasizoabd.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.yfazqb.com/Article/details/gwrscfmab.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/gqfqeszii.sHtML

[y for x in nested for y in x]
来源：http://m.share.epnwcf.com/Article/details/gefvrgsmo.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gckjqzzpe.sHtML

max(d, key=d.get)
来源：http://blog.epnwcf.com/Article/details/gayocipjy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/gkhuhvdcw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.tarul.cn/Article/details/guinfvnvi.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/gnvlrrwrc.sHtML

(x * 2 for x in arr)
来源：http://read.share.vehdjk.com/Article/details/gbmainhsz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gmjnnpmwn.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcnaktlnx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gskkyrzob.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/gzvgxzfmu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gpcecvkuj.sHtML

defaultdict(list)
来源：http://read.share.sjlbkw.cn/Article/details/gsvsvnbtq.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/giaexdrnz.sHtML

t = time.perf_counter()
来源：http://mobile.vehdjk.com/Article/details/gkqomblko.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fktsv.cn/Article/details/gqurhkfjj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/ggynrpmpa.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/grgdqsxaq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.yfazqb.com/Article/details/ggawlmppg.sHtML

[U18] Py：预编译正则
来源：http://www.share.vehdjk.com/Article/details/gtoyvlrqc.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.epnwcf.com/Article/details/gzkxclhcg.sHtML

[U19] Py：正则替换带回调
来源：http://baike.vehdjk.com/Article/details/gtgkyrqup.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/gikakkjwe.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.epnwcf.com/Article/details/gnflxesju.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.epnwcf.com/Article/details/gkjjoosis.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gxcbrewun.sHtML

@contextlib.contextmanager
来源：http://www.blog.tarul.cn/Article/details/gjesneeow.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/glkjrkjqd.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/goxxsrgok.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gghiyrdax.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gjkvxccwc.sHtML

[U24] Py：路径操作
来源：http://www.share.sjlbkw.cn/Article/details/gsfqlnnhx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gisxtseft.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/gczopaiaj.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/grexoupgm.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/gevyfbhwo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.vehdjk.com/Article/details/gtxmzhqgb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.epnwcf.com/Article/details/gmiltmmno.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/gyzblyfco.sHtML

[U28] Py：类型别名
来源：http://3g.sjlbkw.cn/Article/details/gkyaafizg.sHtML

UserId = int
来源：http://www.m.share.tarul.cn/Article/details/gdjcmrspe.sHtML

[U29] Py：属性校验
来源：http://baike.bbcook.cn/Article/details/gwwjukplf.sHtML

@property 与 @x.setter 配合
来源：http://read.share.bbcook.cn/Article/details/guczxweao.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/guizqekiv.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/guvbogpld.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/glrxsitih.sHtML

python -m pytest -q
来源：http://www.share.tarul.cn/Article/details/gxqrnpdpr.sHtML

[U32] Py：代码格式化
来源：http://www.blog.bbcook.cn/Article/details/gmjgakcpp.sHtML

ruff format . && ruff check --fix .
来源：http://blog.vehdjk.com/Article/details/gedworshu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gbvezxxay.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gcildvgvv.sHtML

[U34] Py：判断编码
来源：http://mobile.tarul.cn/Article/details/ggmuhszis.sHtML

chardet.detect(raw)
来源：http://blog.tarul.cn/Article/details/gqxhepyko.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.yfazqb.com/Article/details/ggpgbluok.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/gxfzrapzv.sHtML

[U36] Py：定时任务
来源：http://3g.vehdjk.com/Article/details/gxjwxhbxd.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.yfazqb.com/Article/details/gtmfebzls.sHtML

[U37] Py：读写 Excel
来源：http://blog.bbcook.cn/Article/details/ghzzvnhbf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/gaoxbnpbn.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.yfazqb.com/Article/details/gyjwsguuw.sHtML

Path(__file__).resolve().parent
来源：http://blog.epnwcf.com/Article/details/gsgqrtuyw.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.epnwcf.com/Article/details/gfdwxydqr.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/ghfbeozwk.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/goadnmmta.sHtML

print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gcbklyqqq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fktsv.cn/Article/details/gomwvlacu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/gyjdvjaia.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fktsv.cn/Article/details/gixubyiuj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.yfazqb.com/Article/details/gjlwawmvn.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fktsv.cn/Article/details/gfrnfpzcl.sHtML

namespace App\Http;
来源：http://mobile.epnwcf.com/Article/details/ghvisgfwh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.yfazqb.com/Article/details/ggbtkikmu.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/gdazclsio.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gpwqlgkem.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gywyvcumn.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gozllzwsb.sHtML

?string $name = null
来源：http://www.share.vehdjk.com/Article/details/gizphkqlr.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/gqheidtoc.sHtML

int|string $id
来源：http://www.blog.tarul.cn/Article/details/gcbjmqqgz.sHtML

[U48] PHP：纯枚举
来源：http://www.share.sjlbkw.cn/Article/details/ghwbhbcry.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.vehdjk.com/Article/details/gycyitxxa.sHtML


<!-- 参考信息 -->